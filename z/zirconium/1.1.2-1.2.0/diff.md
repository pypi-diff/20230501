# Comparing `tmp/zirconium-1.1.2.tar.gz` & `tmp/zirconium-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zirconium-1.1.2.tar", last modified: Tue Apr 18 11:57:41 2023, max compression
+gzip compressed data, was "zirconium-1.2.0.tar", last modified: Mon May  1 14:53:10 2023, max compression
```

## Comparing `zirconium-1.1.2.tar` & `zirconium-1.2.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 11:57:41.146935 zirconium-1.1.2/
--rw-rw-rw-   0        0        0     1058 2023-04-18 11:50:52.000000 zirconium-1.1.2/LICENSE
--rw-rw-rw-   0        0        0     5115 2023-04-18 11:57:41.146935 zirconium-1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     4570 2023-04-18 11:50:54.000000 zirconium-1.1.2/README.md
--rw-rw-rw-   0        0        0       88 2023-01-23 19:45:58.000000 zirconium-1.1.2/pyproject.toml
--rw-rw-rw-   0        0        0      684 2023-04-18 11:57:41.146935 zirconium-1.1.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-18 11:57:41.115708 zirconium-1.1.2/src/
-drwxrwxrwx   0        0        0        0 2023-04-18 11:57:41.131286 zirconium-1.1.2/src/zirconium/
--rw-rw-rw-   0        0        0      240 2023-04-18 11:57:30.000000 zirconium-1.1.2/src/zirconium/__init__.py
--rw-rw-rw-   0        0        0    16476 2023-04-18 11:55:45.000000 zirconium-1.1.2/src/zirconium/config.py
--rw-rw-rw-   0        0        0     5155 2023-04-18 11:50:54.000000 zirconium-1.1.2/src/zirconium/parsers.py
--rw-rw-rw-   0        0        0     1148 2023-04-18 11:50:54.000000 zirconium-1.1.2/src/zirconium/sproviders.py
--rw-rw-rw-   0        0        0     5447 2023-01-30 20:11:22.000000 zirconium-1.1.2/src/zirconium/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-18 11:57:41.146935 zirconium-1.1.2/src/zirconium.egg-info/
--rw-rw-rw-   0        0        0     5115 2023-04-18 11:57:41.000000 zirconium-1.1.2/src/zirconium.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      360 2023-04-18 11:57:41.000000 zirconium-1.1.2/src/zirconium.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 11:57:41.000000 zirconium-1.1.2/src/zirconium.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-04-18 11:57:41.000000 zirconium-1.1.2/src/zirconium.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-18 11:57:41.146935 zirconium-1.1.2/tests/
--rw-rw-rw-   0        0        0    15708 2023-04-18 11:54:13.000000 zirconium-1.1.2/tests/test_config.py
--rw-rw-rw-   0        0        0    12057 2023-04-18 11:50:54.000000 zirconium-1.1.2/tests/test_handlers.py
+drwxrwxrwx   0        0        0        0 2023-05-01 14:53:10.944916 zirconium-1.2.0/
+-rw-rw-rw-   0        0        0     1058 2023-04-28 14:59:36.000000 zirconium-1.2.0/LICENSE
+-rw-rw-rw-   0        0        0    10353 2023-05-01 14:53:10.944916 zirconium-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     9808 2023-05-01 14:51:42.000000 zirconium-1.2.0/README.md
+-rw-rw-rw-   0        0        0       88 2023-04-28 14:59:36.000000 zirconium-1.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0      684 2023-05-01 14:53:10.945940 zirconium-1.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-01 14:53:10.916950 zirconium-1.2.0/src/
+drwxrwxrwx   0        0        0        0 2023-05-01 14:53:10.932915 zirconium-1.2.0/src/zirconium/
+-rw-rw-rw-   0        0        0      313 2023-05-01 14:48:04.000000 zirconium-1.2.0/src/zirconium/__init__.py
+-rw-rw-rw-   0        0        0    22477 2023-05-01 14:36:14.000000 zirconium-1.2.0/src/zirconium/config.py
+-rw-rw-rw-   0        0        0     5155 2023-04-28 14:59:36.000000 zirconium-1.2.0/src/zirconium/parsers.py
+-rw-rw-rw-   0        0        0     1148 2023-04-28 14:59:36.000000 zirconium-1.2.0/src/zirconium/sproviders.py
+-rw-rw-rw-   0        0        0     9581 2023-05-01 14:52:23.000000 zirconium-1.2.0/src/zirconium/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-01 14:53:10.937960 zirconium-1.2.0/src/zirconium.egg-info/
+-rw-rw-rw-   0        0        0    10353 2023-05-01 14:53:10.000000 zirconium-1.2.0/src/zirconium.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      360 2023-05-01 14:53:10.000000 zirconium-1.2.0/src/zirconium.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 14:53:10.000000 zirconium-1.2.0/src/zirconium.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-05-01 14:53:10.000000 zirconium-1.2.0/src/zirconium.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-01 14:53:10.942928 zirconium-1.2.0/tests/
+-rw-rw-rw-   0        0        0    22343 2023-05-01 14:35:06.000000 zirconium-1.2.0/tests/test_config.py
+-rw-rw-rw-   0        0        0    12057 2023-04-28 14:59:36.000000 zirconium-1.2.0/tests/test_handlers.py
```

### Comparing `zirconium-1.1.2/LICENSE` & `zirconium-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zirconium-1.1.2/setup.cfg` & `zirconium-1.2.0/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 207a 6972 636f 6e69 756d 0d0a 7665   = zirconium..ve
-00000020: 7273 696f 6e20 3d20 312e 312e 320d 0a61  rsion = 1.1.2..a
+00000020: 7273 696f 6e20 3d20 312e 322e 300d 0a61  rsion = 1.2.0..a
 00000030: 7574 686f 7220 3d20 4572 696e 2054 7572  uthor = Erin Tur
 00000040: 6e62 756c 6c0d 0a61 7574 686f 725f 656d  nbull..author_em
 00000050: 6169 6c20 3d20 6572 696e 2e61 2e74 7572  ail = erin.a.tur
 00000060: 6e62 756c 6c40 676d 6169 6c2e 636f 6d0d  nbull@gmail.com.
 00000070: 0a64 6573 6372 6970 7469 6f6e 203d 2045  .description = E
 00000080: 7863 656c 6c65 6e74 2063 6f6e 6669 6775  xcellent configu
 00000090: 7261 7469 6f6e 206d 616e 6167 656d 656e  ration managemen
```

### Comparing `zirconium-1.1.2/src/zirconium/config.py` & `zirconium-1.2.0/src/zirconium/config.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import os
 import decimal
 import datetime
 import threading
 import sys
+import time
 from pathlib import Path
 import zirconium.sproviders as sp
 import logging
 import typing as t
 
 
 from autoinject import injector, CacheStrategy
 from .parsers import JsonConfigParser, IniConfigParser, YamlConfigParser, TomlConfigParser, CfgConfigParser
-from .utils import MutableDeepDict, _AppConfigHooks
+from .utils import MutableDeepDict, _AppConfigHooks, convert_to_timedelta, convert_to_bytes, parse_for_units
 
 # Metadata entrypoint support depends on Python version
 import importlib.util
 if importlib.util.find_spec("importlib.metadata"):
     # Python 3.10 supports entry_points(group=?)
     if sys.version_info.minor >= 10:
         from importlib.metadata import entry_points
@@ -33,14 +34,64 @@
                 return []
 
 # Backwards support for Python 3.7
 else:
     from importlib_metadata import entry_points
 
 
+VT = t.TypeVar("VT")
+
+
+class _ConfigRef(t.Generic[VT]):
+
+    def __init__(self, cfg_obj, cb_method, key, **kwargs):
+        self.config = cfg_obj
+        self.cb_method = cb_method
+        self.key = key
+        self.kwargs = kwargs
+        self._cached = None
+        self._cache_identifier = None
+
+    def _ensure_cache(self) -> t.Optional[VT]:
+        if self._cache_identifier is None or self._cache_identifier != self.config.cache_identifier:
+            self._cache_identifier = self.config.cache_identifier
+            self._cached = getattr(self.config, self.cb_method)(self.key, **self.kwargs)
+        return self._cached
+
+    def __eq__(self, other) -> bool:
+        if isinstance(other, _ConfigRef):
+            return self.raw_value() == other.raw_value()
+        else:
+            return self.raw_value() == other
+
+    def raw_value(self) -> t.Optional[VT]:
+        return self._ensure_cache()
+
+    def is_none(self) -> bool:
+        return self._ensure_cache() is None
+
+    def __getattr__(self, item):
+        c = self._ensure_cache()
+        if c:
+            return getattr(c, item)
+        return None
+
+    def __bool__(self) -> bool:
+        return bool(self._ensure_cache())
+
+    def __str__(self) -> str:
+        return str(self._ensure_cache())
+
+    def __int__(self) -> int:
+        return int(self._ensure_cache())
+
+    def __float__(self) -> float:
+        return float(self._ensure_cache())
+
+
 @injector.register("zirconium.config.ApplicationConfig", caching_strategy=CacheStrategy.GLOBAL_CACHE)
 class ApplicationConfig(MutableDeepDict):
 
     ach: _AppConfigHooks = None
 
     @injector.construct
     def __init__(self, manual_init=False):
@@ -61,46 +112,49 @@
             "defaults": [],
             "regulars": [],
             "environment": [],
         }
         self.secrets_env_map = {}
         self.secrets_map = {}
         self.environment_map = {}
+        self._default_config = {}
+        self._on_load = []
         self.loaded_files = []
         self._init_flag = False
+        self.cache_identifier = None
         self._cached_gets = {}
         self.registry_lock = threading.RLock()
         self.cache_lock = threading.RLock()
         if not manual_init:
             auto_register = entry_points(group="zirconium.parsers")
             for ep in auto_register:
                 self.parsers.append(ep.load()(self))
             auto_register = entry_points(group="zirconium.config")
             for ep in auto_register:
                 registrar_func = ep.load()
                 registrar_func(self)
             self.ach.execute_hooks(self)
             self.init()
 
+    def on_load(self, cb):
+        self._on_load.append(cb)
+
     def get(self, *key, default=None, coerce=None, blank_to_none=False, raw=False, raise_error=False):
         key = self._expand_key(key)
-        full_key = ".".join([str(x) for x in key]) + (str(coerce) if coerce else "")
-        if full_key in self._cached_gets:
-            return self._cached_gets[full_key]
-        with self.cache_lock:
-            if full_key not in self._cached_gets:
-                value = super().get(*key, default=default, raise_error=raise_error)
-                if blank_to_none and value == "":
-                    value = None
-                if (not raw) and isinstance(value, str):
-                    value = self.resolve_environment_references(value)
-                if coerce and value is not None:
-                    value = coerce(value)
-                self._cached_gets[full_key] = value
-            return self._cached_gets[full_key]
+        value = super().get(*key, default=default, raise_error=raise_error)
+        if blank_to_none and value == "":
+            value = None
+        if (not raw) and isinstance(value, str):
+            value = self.resolve_environment_references(value)
+        if coerce and value is not None:
+            value = coerce(value)
+        return value
+
+    def get_ref(self, *key, **kwargs) -> _ConfigRef[t.Any]:
+        return _ConfigRef[t.Any](self, 'get', key, **kwargs)
 
     def resolve_environment_references(self, value: str) -> str:
         pos = 0
         # Escape rule for $ is dollar signs that precede a bracket
         # ${var}
         # $${not_a_var}, equivalent to string ${not_a_var}
         # $$${var}, equivalent to "${}".format(os.environ["var"])
@@ -174,27 +228,56 @@
 
     def get_secret(self, secret_path, secret_provider):
         if secret_provider not in self._secret_providers:
             self.log.warning(f"Secret provider {secret_provider} not found")
             return None
         return self._secret_providers[secret_provider](secret_path)
 
+    def as_bytes(self, key: t.Union[t.Iterable, t.AnyStr], default=None, default_units: str = "b", allow_metric: bool = False, raw: bool = False) -> t.Union[int, float]:
+        val = self.get(key, default=default, blank_to_none=True, raw=raw)
+        if val is None:
+            return val
+        elif isinstance(val, int) or isinstance(val, float):
+            return convert_to_bytes(val, default_units, not allow_metric)
+        else:
+            val, units = parse_for_units(str(val), 3, default_units)
+            return convert_to_bytes(val, units, not allow_metric)
+
+    def as_bytes_ref(self, key: t.Union[t.Iterable, t.AnyStr], default=None, default_units="s", raw=False) -> _ConfigRef[t.Union[int, float]]:
+        return _ConfigRef[t.Union[int, float]](self, 'as_bytes', key, default=default, default_units=default_units, raw=raw)
+
+    def as_timedelta(self, key: t.Union[t.Iterable, t.AnyStr], default=None, default_units: str = "s", raw: bool = False) -> t.Optional[datetime.timedelta]:
+        val = self.get(key, default=default, blank_to_none=True, raw=raw)
+        if val is None or isinstance(val, datetime.timedelta):
+            return val
+        elif isinstance(val, int) or isinstance(val, float):
+            return convert_to_timedelta(val, default_units)
+        else:
+            val, units = parse_for_units(str(val), 2, default_units)
+            return convert_to_timedelta(val, units)
+
+    def as_timedelta_ref(self, key: t.Union[t.Iterable, t.AnyStr], default=None, default_units="s", raw=False) -> _ConfigRef[datetime.timedelta]:
+        return _ConfigRef[datetime.timedelta](self, 'as_timedelta', key, default=default, default_units=default_units, raw=raw)
+
     def as_date(self, key: t.Union[t.Iterable, t.AnyStr], default=None, raw=False) -> t.Optional[datetime.date]:
         dt = self.get(key, default=default, blank_to_none=True, raw=raw)
         if isinstance(dt, datetime.datetime):
             return datetime.date(dt.year, dt.month, dt.day)
         elif dt is None or isinstance(dt, datetime.date):
             return dt
         else:
             try:
                 return datetime.date.fromisoformat(dt)
             except ValueError:
                 dt = datetime.datetime.fromisoformat(dt)
                 return datetime.date(dt.year, dt.month, dt.day)
 
+    def as_date_ref(self, key: t.Union[t.Iterable, t.AnyStr], default=None, raw=False) -> _ConfigRef[datetime.date]:
+        return _ConfigRef[datetime.date](self, 'as_date', key, default=default, raw=raw)
+
     def as_datetime(self, key: t.Union[t.Iterable, t.AnyStr], default=None, tzinfo=None, raw=False) -> t.Optional[datetime.datetime]:
         dt = self.get(key, default=default, blank_to_none=True, raw=raw)
         if dt is None:
             return None
         if isinstance(dt, datetime.datetime):
             if dt.tzinfo is None and tzinfo is not None:
                 return datetime.datetime(
@@ -221,45 +304,77 @@
                     dt.minute,
                     dt.second,
                     dt.microsecond,
                     tzinfo
                 )
             return dt
 
+    def as_datetime_ref(self, key: t.Union[t.Iterable, t.AnyStr], default=None, tzinfo=None, raw=False) -> _ConfigRef[datetime.datetime]:
+        return _ConfigRef[datetime.datetime](self, 'as_datetime', key, default=default, tzinfo=tzinfo, raw=raw)
+
     def as_int(self, key: t.Union[t.Iterable, t.AnyStr], default=None, raw=False) -> t.Optional[int]:
         return self.get(key, default=default, coerce=int, blank_to_none=True, raw=raw)
 
+    def as_int_ref(self, key: t.Union[t.Iterable, t.AnyStr], default=None, raw=False) -> _ConfigRef[int]:
+        return _ConfigRef[int](self, 'as_int', key, default=default, raw=raw)
+
     def as_float(self, key: t.Union[t.Iterable, t.AnyStr], default=None, raw=False) -> t.Optional[float]:
         return self.get(key, default=default, coerce=float, blank_to_none=True, raw=raw)
 
+    def as_float_ref(self, key: t.Union[t.Iterable, t.AnyStr], default=None, raw=False) -> _ConfigRef[float]:
+        return _ConfigRef[float](self, 'as_float', key, default=default, raw=raw)
+
     def as_decimal(self, key: t.Union[t.Iterable, t.AnyStr], default=None, raw=False) -> t.Optional[decimal.Decimal]:
         return self.get(key, default=default, coerce=decimal.Decimal, blank_to_none=True, raw=raw)
 
+    def as_decimal_ref(self, key: t.Union[t.Iterable, t.AnyStr], default=None, raw=False) -> _ConfigRef[decimal.Decimal]:
+        return _ConfigRef[decimal.Decimal](self, 'as_decimal', key, default=default, raw=raw)
+
     def as_str(self, key: t.Union[t.Iterable, t.AnyStr], default=None, raw=False) -> t.Optional[str]:
         return self.get(key, default=default, coerce=str, raw=raw)
 
+    def as_str_ref(self, key: t.Union[t.Iterable, t.AnyStr], default=None, raw=False) -> _ConfigRef[str]:
+        return _ConfigRef[str](self, 'as_float', key, default=default, raw=raw)
+
     def as_bool(self, key: t.Union[t.Iterable, t.AnyStr], default=None, raw=False) -> t.Optional[bool]:
         return bool(self.get(key, default=default, raw=raw))
 
+    def as_bool_ref(self, key: t.Union[t.Iterable, t.AnyStr], default=None, raw=False) -> _ConfigRef[bool]:
+        return _ConfigRef[bool](self, 'as_bool', key, default=default, raw=raw)
+
     def as_path(self, key: t.Union[t.Iterable, t.AnyStr], default=None, raw=False) -> t.Optional[Path]:
         return self.get(key, default=default, coerce=Path, blank_to_none=True, raw=raw)
 
+    def as_path_ref(self, key: t.Union[t.Iterable, t.AnyStr], default=None, raw=False) -> _ConfigRef[Path]:
+        return _ConfigRef[Path](self, 'as_path', key, default=default, raw=raw)
+
     def as_set(self, key: t.Union[t.Iterable, t.AnyStr], default=None) -> t.Optional[set]:
         return self.get(key, default=default, coerce=set, blank_to_none=True, raw=True)
 
+    def as_set_ref(self, key: t.Union[t.Iterable, t.AnyStr], default=None) -> _ConfigRef[set]:
+        return _ConfigRef[set](self, 'as_set', key, default=default)
+
     def as_list(self, key: t.Union[t.Iterable, t.AnyStr], default=None) -> t.Optional[list]:
         return self.get(key, default=default, coerce=list, blank_to_none=True, raw=True)
 
+    def as_list_ref(self, key: t.Union[t.Iterable, t.AnyStr], default=None) -> _ConfigRef[list]:
+        return _ConfigRef[list](self, 'as_list', key, default=default)
+
     def as_dict(self, key: t.Union[t.Iterable, t.AnyStr], default=None) -> t.Optional[dict]:
         return self.get(key, default=default, coerce=MutableDeepDict, blank_to_none=True, raw=True)
 
+    def as_dict_ref(self, key: t.Union[t.Iterable, t.AnyStr], default=None) -> _ConfigRef[dict]:
+        return _ConfigRef[dict](self, 'as_dict', key, default=default)
+
     def set_default_encoding(self, enc):
         self.encoding = enc
 
     def is_truthy(self, key: t.Union[t.Iterable, t.AnyStr]) -> bool:
+        if not self._init_flag:
+            self.init()
         parent, k = self._navigate_to_item(key)
         return parent is not None and k in parent and bool(parent[k])
 
     def register_parser(self, parser):
         self.parsers.append(parser)
 
     def register_secret_provider(self, name, callback):
@@ -298,79 +413,96 @@
         if self.file_registry[key]:
             return max(x[1] for x in self.file_registry[key]) + 1
         return 0
 
     def register_environ_var(self, env_var_name, *target_config):
         self.environment_map[env_var_name] = target_config
 
+    def register_environ_map(self, env_map):
+        self.environment_map.update(env_map)
+
     def reload_config(self):
         # We take all three locks to prevent any weird multi-threaded behaviour from happening. All writes are blocked until we are done the re-load except our own.
         with self.lock:
             with self.registry_lock:
                 with self.cache_lock:
                     self._cached_gets = {}
+                    self.loaded_files = []
                     self._init_flag = False
                     self.clear()
                     self.init()
 
     def register_secret_as_environ_var(self, secret_path, secret_provider, env_var_name):
         self.secrets_env_map[env_var_name] = (secret_path, secret_provider)
 
     def register_secret_config(self, secret_path, secret_provider, *target_config):
         secret_provider = secret_provider.lower()
         self.secrets_map[f"{secret_path}{secret_provider}"] = (secret_path, secret_provider, target_config)
 
     def init(self):
         with self.registry_lock:
             if not self._init_flag:
+                new_conf = MutableDeepDict()
+                new_conf.deep_update(self._default_config)
                 self.file_registry["defaults"].sort(key=lambda x: x[1])
                 for file, weight, parser, enc in self.file_registry["defaults"]:
-                    self.load_file(file, parser, enc)
+                    self.load_file(new_conf, file, parser, enc)
                 self.file_registry["regulars"].sort(key=lambda x: x[1])
                 for file, weight, parser, enc in self.file_registry["regulars"]:
-                    self.load_file(file, parser, enc)
+                    self.load_file(new_conf, file, parser, enc)
                 self.file_registry["environment"].sort(key=lambda x: x[1])
                 for env_name, weight, parser, enc in self.file_registry["environment"]:
                     env_val = self.get_env_var(env_name)
                     if env_val:
-                        self.load_file(env_val, parser, enc)
+                        self.load_file(new_conf, env_val, parser, enc)
                 for env_name, target_config in self.environment_map:
                     env_val = self.get_env_var(env_name)
                     if env_val is not None:
                         self.log.info(f"Setting config from environment variable {env_name}")
-                        self.config[target_config] = env_val
+                        new_conf[target_config] = env_val
                     else:
                         self.log.debug(f"No environment variable set for {env_name}")
                 for key in self.secrets_map:
                     spath, sprovider, target_config = self._secret_providers[key]
                     secret_val = self.get_secret(sprovider, spath)
                     if secret_val is not None:
                         self.log.info(f"Loading secret from {sprovider} {spath}")
-                        self.config[target_config] = secret_val
+                        new_conf[target_config] = secret_val
+                self.d = new_conf.d
                 self._init_flag = True
+                if self.cache_identifier is None:
+                    self.cache_identifier = 1
+                else:
+                    self.cache_identifier += 1
+                for cb in self._on_load:
+                    cb(self)
 
-    def load_file(self, file_path, parser=None, encoding=None):
+    def load_file(self, new_conf, file_path, parser=None, encoding=None):
         with self.registry_lock:
             if encoding is None:
                 encoding = self.encoding
             file_path = Path(file_path).expanduser().absolute()
             if file_path in self.loaded_files:
                 return
             if file_path.exists():
                 if parser:
                     self.log.info(f"Loading config file {file_path}")
-                    self.load_from_dict(parser.read_dict(file_path, encoding))
+                    new_conf.deep_update(parser.read_dict(file_path, encoding))
                     self.loaded_files.append(file_path)
                 else:
                     for parser in self.parsers:
                         if parser.handles(file_path.name):
                             self.log.info(f"Loading config file {file_path}")
-                            self.load_from_dict(parser.read_dict(file_path, encoding))
+                            new_conf.deep_update(parser.read_dict(file_path, encoding))
                             self.loaded_files.append(file_path)
                             break
                     else:
                         self.log.warning(f"No parser found for {file_path}")
             else:
                 self.log.info(f"No config file found at {file_path}")
 
+    def set_defaults(self, d):
+        self._default_config.update(d)
+
     def load_from_dict(self, d):
         self.deep_update(d)
+
```

### Comparing `zirconium-1.1.2/src/zirconium/parsers.py` & `zirconium-1.2.0/src/zirconium/parsers.py`

 * *Files identical despite different names*

### Comparing `zirconium-1.1.2/src/zirconium/sproviders.py` & `zirconium-1.2.0/src/zirconium/sproviders.py`

 * *Files identical despite different names*

### Comparing `zirconium-1.1.2/tests/test_config.py` & `zirconium-1.2.0/tests/test_config.py`

 * *Files 18% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         self.assertIsInstance(config["twelve"], list)
         self.assertEqual(config["seventeen"], datetime.datetime(2020, 1, 1, 1, 2, 3))
 
     def test_two_files(self):
         path = Path(__file__).parent / "example_configs/basic.yaml"
         path2 = Path(__file__).parent / "example_configs/override.toml"
         config = zirconium.ApplicationConfig(True)
-        config.load_from_dict({
+        config.set_defaults({
             "base": "one"
         })
         config.register_file(path)
         config.register_file(path2)
         config.init()
         self.assertEqual(config["base"], "one")
         self.assertTrue("one" in config)
@@ -67,14 +67,15 @@
             "middle_replace": "VN ${VAR_NAME} VN",
             "lower_var": "${LOWER_VAR}",
             "upper_var": "${var_name}",
             "complex_inner": r"${${INNER\}}",
             "weird_bracket": r"${\}end}",
             "weird_bracket_default": r"${\}end2=bar}"
         })
+
         self.assertEqual(config["simple_replace"], "var")
         self.assertEqual(config["default_use"], "test")
         self.assertEqual(config["complex_replace"], "$$var")
         self.assertEqual(config["complex_noreplace"], "$${VAR_NAME}")
         self.assertEqual(config["no_replace"], "${VAR_NAME}")
         self.assertEqual(config["no_end"], "${VAR_NAME_NO_END")
         self.assertEqual(config["lower_var"], "var2")
@@ -109,14 +110,34 @@
         config.load_from_dict({
             1: "one"
         })
         self.assertTrue(1 in config)
         self.assertFalse(2 in config)
         self.assertEqual(config[1], "one")
 
+    def test_get_ref(self):
+        config = zirconium.ApplicationConfig(True)
+        config.set_defaults({
+            1: "one"
+        })
+        config.init()
+        r = config.get_ref(1)
+        self.assertIsInstance(r, zirconium.config._ConfigRef)
+        self.assertEqual(r.raw_value(), "one")
+        self.assertEqual(r.raw_value(), "one")
+        config.load_from_dict({
+            1: "two"
+        })
+        self.assertEqual(r.raw_value(), "one")
+        config.reload_config()
+        config.load_from_dict({
+            1: "two"
+        })
+        self.assertEqual(r.raw_value(), "two")
+
     def test_clear(self):
         config = zirconium.ApplicationConfig(True)
         config.load_from_dict({
             1: "one",
             2: "two"
         })
         self.assertTrue(1 in config)
@@ -231,14 +252,107 @@
                 "two": "three"
             }
         })
         self.assertTrue("one" in config)
         self.assertTrue(("one" ,"two") in config)
         self.assertEqual(config["one", "two"], "three")
 
+    def test_bytes_coerce(self):
+        config = zirconium.ApplicationConfig(True)
+        config.load_from_dict({
+            "raw": 512,
+            "raw_str": "512",
+            "for_def": 512,
+            "bits": "512bit",
+            "bytes": "512b",
+            "kib": "2kib",
+            "mib": "2mib",
+            "gib": "2gib",
+            "tib": "2tib",
+            "pib": "2pib",
+            "eib": "2eib",
+            "k": "2K",
+            "m": "2M",
+            "g": "2G",
+            "t": "2T",
+            "p": "2P",
+            "e": "2E",
+            "kb": "2KB",
+            "mb": "2MB",
+            "gb": "2GB",
+            "tb": "2TB",
+            "pb": "2PB",
+            "eb": "2EB",
+            "no": "2WB",
+            "very_no": "Foobar"
+        })
+        self.assertEqual(config.as_bytes("raw"), 512)
+        self.assertEqual(config.as_bytes("for_def", default_units="kib"), 512 * 1024)
+        self.assertEqual(config.as_bytes("raw_str"), 512)
+        self.assertEqual(config.as_bytes("bits"), 64.0)
+        self.assertEqual(config.as_bytes("bytes"), 512)
+        self.assertEqual(config.as_bytes("kib"), 1024 * 2)
+        self.assertEqual(config.as_bytes("mib"), 1024 * 1024 * 2)
+        self.assertEqual(config.as_bytes("gib"), 1024 * 1024 * 1024 * 2)
+        self.assertEqual(config.as_bytes("tib"), 1024 * 1024 * 1024 * 1024 * 2)
+        self.assertEqual(config.as_bytes("pib"), 1024 * 1024 * 1024 * 1024 * 1024 * 2)
+        self.assertEqual(config.as_bytes("eib"), 1024 * 1024 * 1024 * 1024 * 1024 * 1024 * 2)
+        self.assertEqual(config.as_bytes("k"), 1024 * 2)
+        self.assertEqual(config.as_bytes("m"), 1024 * 1024 * 2)
+        self.assertEqual(config.as_bytes("g"), 1024 * 1024 * 1024 * 2)
+        self.assertEqual(config.as_bytes("t"), 1024 * 1024 * 1024 * 1024 * 2)
+        self.assertEqual(config.as_bytes("p"), 1024 * 1024 * 1024 * 1024 * 1024 * 2)
+        self.assertEqual(config.as_bytes("e"), 1024 * 1024 * 1024 * 1024 * 1024 * 1024 * 2)
+        self.assertEqual(config.as_bytes("kb"), 1024 * 2)
+        self.assertEqual(config.as_bytes("mb"), 1024 * 1024 * 2)
+        self.assertEqual(config.as_bytes("gb"), 1024 * 1024 * 1024 * 2)
+        self.assertEqual(config.as_bytes("tb"), 1024 * 1024 * 1024 * 1024 * 2)
+        self.assertEqual(config.as_bytes("pb"), 1024 * 1024 * 1024 * 1024 * 1024 * 2)
+        self.assertEqual(config.as_bytes("eb"), 1024 * 1024 * 1024 * 1024 * 1024 * 1024 * 2)
+        self.assertEqual(config.as_bytes("kb", allow_metric=True), 1000 * 2)
+        self.assertEqual(config.as_bytes("mb", allow_metric=True), 1000 * 1000 * 2)
+        self.assertEqual(config.as_bytes("gb", allow_metric=True), 1000 * 1000 * 1000 * 2)
+        self.assertEqual(config.as_bytes("tb", allow_metric=True), 1000 * 1000 * 1000 * 1000 * 2)
+        self.assertEqual(config.as_bytes("pb", allow_metric=True), 1000 * 1000 * 1000 * 1000 * 1000 * 2)
+        self.assertEqual(config.as_bytes("eb", allow_metric=True), 1000 * 1000 * 1000 * 1000 * 1000 * 1000 * 2)
+
+    def test_timedelta_coerce(self):
+        config = zirconium.ApplicationConfig(True)
+        config.load_from_dict({
+            "def": 234,
+            "def_min": 234,
+            "test_s": "23s",
+            "test_m": "23m",
+            "test_h": "23h",
+            "test_d": "23d",
+            "test_w": "23w",
+            "test_w1s": "23 w",
+            "test_w3s": "   23     w  ",
+            "test_us": "23us",
+            "test_ms": "23ms",
+            "test_str_no": "23",
+            "test_err": "23n",
+            "test_big_err": "foobar"
+        })
+        self.assertEqual(config.as_timedelta("def"), datetime.timedelta(seconds=234))
+        self.assertEqual(config.as_timedelta("def_min", default_units="m"), datetime.timedelta(minutes=234))
+        self.assertEqual(config.as_timedelta("test_s"), datetime.timedelta(seconds=23))
+        self.assertEqual(config.as_timedelta("test_m"), datetime.timedelta(minutes=23))
+        self.assertEqual(config.as_timedelta("test_h"), datetime.timedelta(hours=23))
+        self.assertEqual(config.as_timedelta("test_d"), datetime.timedelta(days=23))
+        self.assertEqual(config.as_timedelta("test_w"), datetime.timedelta(weeks=23))
+        self.assertEqual(config.as_timedelta("test_w1s"), datetime.timedelta(weeks=23))
+        self.assertEqual(config.as_timedelta("test_w3s"), datetime.timedelta(weeks=23))
+        self.assertEqual(config.as_timedelta("test_us"), datetime.timedelta(microseconds=23))
+        self.assertEqual(config.as_timedelta("test_ms"), datetime.timedelta(milliseconds=23))
+        self.assertEqual(config.as_timedelta("test_str_no"), datetime.timedelta(seconds=23))
+        self.assertRaises(ValueError, config.as_timedelta, "test_err")
+        self.assertRaises(ValueError, config.as_timedelta, "test_big_err")
+
+
     def test_int_coerce(self):
         config = zirconium.ApplicationConfig(True)
         config.load_from_dict({
             "str": "1234",
             "int": 12,
             "bad": "modern general",
             "nope": None,
@@ -246,14 +360,38 @@
         })
         self.assertEqual(config.as_int("str"), 1234)
         self.assertEqual(config.as_int("int"), 12)
         self.assertIsNone(config.as_int("nope"))
         self.assertIsNone(config.as_int("blank"))
         self.assertRaises(ValueError, config.as_int, "bad")
 
+    def test_int_ref_coerce(self):
+        config = zirconium.ApplicationConfig(True)
+        config.load_from_dict({
+            "str": "1234",
+            "str_int": 1234,
+            "int": 12,
+            "falsy": 0,
+            "bad": "modern general",
+            "nope": None,
+            "blank": "",
+        })
+        self.assertEqual(config.as_int_ref("str"), config.as_int_ref("str_int"))
+        self.assertNotEqual(config.as_int_ref("str"), config.as_int_ref("int"))
+        self.assertEqual(config.as_int_ref("str"), 1234)
+        self.assertEqual(config.as_int_ref("int"), 12)
+        self.assertIsNone(config.as_int_ref("nope").raw_value())
+        self.assertIsNone(config.as_int_ref("blank").raw_value())
+        self.assertTrue(config.as_int_ref("nope").is_none())
+        self.assertTrue(config.as_int_ref("blank").is_none())
+        self.assertFalse(config.as_int_ref("str").is_none())
+        self.assertRaises(ValueError, config.as_int_ref("bad").raw_value)
+        self.assertTrue(config.as_int_ref("int"))
+        self.assertFalse(config.as_int_ref("falsy"))
+
     def test_cache_by_type(self):
         config = zirconium.ApplicationConfig(True)
         config.load_from_dict({
             "int": 12,
         })
         self.assertEqual(config.as_str("int"), "12")
         self.assertEqual(config.as_int("int"), 12)
```

### Comparing `zirconium-1.1.2/tests/test_handlers.py` & `zirconium-1.2.0/tests/test_handlers.py`

 * *Files identical despite different names*

