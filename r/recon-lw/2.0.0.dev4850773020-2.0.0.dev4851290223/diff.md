# Comparing `tmp/recon_lw-2.0.0.dev4850773020.tar.gz` & `tmp/recon_lw-2.0.0.dev4851290223.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/recon_lw-2.0.0.dev4850773020.tar", last modified: Mon May  1 11:28:10 2023, max compression
+gzip compressed data, was "dist/recon_lw-2.0.0.dev4851290223.tar", last modified: Mon May  1 12:55:30 2023, max compression
```

## Comparing `recon_lw-2.0.0.dev4850773020.tar` & `recon_lw-2.0.0.dev4851290223.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 11:28:10.000000 recon_lw-2.0.0.dev4850773020/
--rw-r--r--   0 runner    (1001) docker     (122)       69 2023-05-01 11:27:30.000000 recon_lw-2.0.0.dev4850773020/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-05-01 11:28:10.000000 recon_lw-2.0.0.dev4850773020/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-05-01 11:27:30.000000 recon_lw-2.0.0.dev4850773020/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       76 2023-05-01 11:27:52.000000 recon_lw-2.0.0.dev4850773020/package_info.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 11:28:10.000000 recon_lw-2.0.0.dev4850773020/recon_lw/
--rw-r--r--   0 runner    (1001) docker     (122)     1871 2023-05-01 11:27:30.000000 recon_lw-2.0.0.dev4850773020/recon_lw/EventsSaver.py
--rw-r--r--   0 runner    (1001) docker     (122)     2748 2023-05-01 11:27:30.000000 recon_lw-2.0.0.dev4850773020/recon_lw/TimeCacheMatcher.py
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-05-01 11:27:30.000000 recon_lw-2.0.0.dev4850773020/recon_lw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13010 2023-05-01 11:27:30.000000 recon_lw-2.0.0.dev4850773020/recon_lw/recon_lw.py
--rw-r--r--   0 runner    (1001) docker     (122)    20404 2023-05-01 11:27:30.000000 recon_lw-2.0.0.dev4850773020/recon_lw/recon_ob.py
--rw-r--r--   0 runner    (1001) docker     (122)    14809 2023-05-01 11:27:30.000000 recon_lw-2.0.0.dev4850773020/recon_lw/recon_ob_cross_stream.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 11:28:10.000000 recon_lw-2.0.0.dev4850773020/recon_lw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-05-01 11:28:10.000000 recon_lw-2.0.0.dev4850773020/recon_lw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      374 2023-05-01 11:28:10.000000 recon_lw-2.0.0.dev4850773020/recon_lw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-01 11:28:10.000000 recon_lw-2.0.0.dev4850773020/recon_lw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      219 2023-05-01 11:28:10.000000 recon_lw-2.0.0.dev4850773020/recon_lw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-05-01 11:28:10.000000 recon_lw-2.0.0.dev4850773020/recon_lw.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      275 2023-05-01 11:27:30.000000 recon_lw-2.0.0.dev4850773020/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-01 11:28:10.000000 recon_lw-2.0.0.dev4850773020/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-05-01 11:27:30.000000 recon_lw-2.0.0.dev4850773020/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 12:55:30.000000 recon_lw-2.0.0.dev4851290223/
+-rw-r--r--   0 runner    (1001) docker     (122)       69 2023-05-01 12:54:30.000000 recon_lw-2.0.0.dev4851290223/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-05-01 12:55:30.000000 recon_lw-2.0.0.dev4851290223/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-05-01 12:54:30.000000 recon_lw-2.0.0.dev4851290223/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       76 2023-05-01 12:55:02.000000 recon_lw-2.0.0.dev4851290223/package_info.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 12:55:30.000000 recon_lw-2.0.0.dev4851290223/recon_lw/
+-rw-r--r--   0 runner    (1001) docker     (122)     1877 2023-05-01 12:54:30.000000 recon_lw-2.0.0.dev4851290223/recon_lw/EventsSaver.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2748 2023-05-01 12:54:30.000000 recon_lw-2.0.0.dev4851290223/recon_lw/TimeCacheMatcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-05-01 12:54:30.000000 recon_lw-2.0.0.dev4851290223/recon_lw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13016 2023-05-01 12:54:30.000000 recon_lw-2.0.0.dev4851290223/recon_lw/recon_lw.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20404 2023-05-01 12:54:30.000000 recon_lw-2.0.0.dev4851290223/recon_lw/recon_ob.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14809 2023-05-01 12:54:30.000000 recon_lw-2.0.0.dev4851290223/recon_lw/recon_ob_cross_stream.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 12:55:30.000000 recon_lw-2.0.0.dev4851290223/recon_lw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-05-01 12:55:30.000000 recon_lw-2.0.0.dev4851290223/recon_lw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      374 2023-05-01 12:55:30.000000 recon_lw-2.0.0.dev4851290223/recon_lw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-01 12:55:30.000000 recon_lw-2.0.0.dev4851290223/recon_lw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      219 2023-05-01 12:55:30.000000 recon_lw-2.0.0.dev4851290223/recon_lw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-05-01 12:55:30.000000 recon_lw-2.0.0.dev4851290223/recon_lw.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      275 2023-05-01 12:54:30.000000 recon_lw-2.0.0.dev4851290223/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-01 12:55:30.000000 recon_lw-2.0.0.dev4851290223/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-05-01 12:54:30.000000 recon_lw-2.0.0.dev4851290223/setup.py
```

### Comparing `recon_lw-2.0.0.dev4850773020/recon_lw/EventsSaver.py` & `recon_lw-2.0.0.dev4851290223/recon_lw/EventsSaver.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     def flush(self):
         for scope in self._scopes_buffers.keys():
             self.flush_scope(scope)
 
     def flush_scope(self, scope):
         if scope in self._scopes_buffers:
             events = Data(self._scopes_buffers[scope])
-            events_file = self._path / (scope + "_" + self._scopes_buffers[scope][0]["eventId"] + ".pickle")
+            events_file = self._path / (scope + "_scope_" + self._scopes_buffers[scope][0]["eventId"] + ".pickle")
             events.build_cache(events_file)
             self._scopes_buffers[scope].clear()
 
     def save_events(self, batch):
         for e in batch:
             scope = e["scope"] if "scope" in e else "default"
             if scope not in self._scopes_buffers:
```

### Comparing `recon_lw-2.0.0.dev4850773020/recon_lw/TimeCacheMatcher.py` & `recon_lw-2.0.0.dev4851290223/recon_lw/TimeCacheMatcher.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev4850773020/recon_lw/recon_lw.py` & `recon_lw-2.0.0.dev4851290223/recon_lw/recon_lw.py`

 * *Files 0% similar despite different names*

```diff
@@ -293,15 +293,15 @@
     files.sort()
     scopes_streams = {}
     for f in files:
         if ".pickle" not in f:
             continue
         if name_filter is not None and not name_filter(f):
             continue
-        scope = f[:f.index("_")]
+        scope = f[:f.index("_scope_")]
         if scope not in scopes_streams:
             scopes_streams[scope] = Data.from_cache_file(path.join(streams_path, f))
         else:
             scopes_streams[scope] += Data.from_cache_file(path.join(streams_path, f))
     for strm in scopes_streams.values():
         ts0 = {"epochSecond": 0, "nano": 0}
         streams.add((ts0, iter(strm), None))
```

### Comparing `recon_lw-2.0.0.dev4850773020/recon_lw/recon_ob.py` & `recon_lw-2.0.0.dev4851290223/recon_lw/recon_ob.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev4850773020/recon_lw/recon_ob_cross_stream.py` & `recon_lw-2.0.0.dev4851290223/recon_lw/recon_ob_cross_stream.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev4850773020/setup.py` & `recon_lw-2.0.0.dev4851290223/setup.py`

 * *Files identical despite different names*

