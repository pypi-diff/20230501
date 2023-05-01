# Comparing `tmp/recon_lw-2.0.0.dev4849753051.tar.gz` & `tmp/recon_lw-2.0.0.dev4850623410.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/recon_lw-2.0.0.dev4849753051.tar", last modified: Mon May  1 08:27:41 2023, max compression
+gzip compressed data, was "dist/recon_lw-2.0.0.dev4850623410.tar", last modified: Mon May  1 11:03:52 2023, max compression
```

## Comparing `recon_lw-2.0.0.dev4849753051.tar` & `recon_lw-2.0.0.dev4850623410.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 08:27:41.000000 recon_lw-2.0.0.dev4849753051/
--rw-r--r--   0 runner    (1001) docker     (122)       69 2023-05-01 08:26:54.000000 recon_lw-2.0.0.dev4849753051/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-05-01 08:27:41.000000 recon_lw-2.0.0.dev4849753051/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-05-01 08:26:54.000000 recon_lw-2.0.0.dev4849753051/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       76 2023-05-01 08:27:19.000000 recon_lw-2.0.0.dev4849753051/package_info.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 08:27:41.000000 recon_lw-2.0.0.dev4849753051/recon_lw/
--rw-r--r--   0 runner    (1001) docker     (122)     1432 2023-05-01 08:26:54.000000 recon_lw-2.0.0.dev4849753051/recon_lw/EventsSaver.py
--rw-r--r--   0 runner    (1001) docker     (122)     2748 2023-05-01 08:26:54.000000 recon_lw-2.0.0.dev4849753051/recon_lw/TimeCacheMatcher.py
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-05-01 08:26:54.000000 recon_lw-2.0.0.dev4849753051/recon_lw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12849 2023-05-01 08:26:54.000000 recon_lw-2.0.0.dev4849753051/recon_lw/recon_lw.py
--rw-r--r--   0 runner    (1001) docker     (122)    20315 2023-05-01 08:26:54.000000 recon_lw-2.0.0.dev4849753051/recon_lw/recon_ob.py
--rw-r--r--   0 runner    (1001) docker     (122)    14371 2023-05-01 08:26:54.000000 recon_lw-2.0.0.dev4849753051/recon_lw/recon_ob_cross_stream.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 08:27:41.000000 recon_lw-2.0.0.dev4849753051/recon_lw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-05-01 08:27:41.000000 recon_lw-2.0.0.dev4849753051/recon_lw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      374 2023-05-01 08:27:41.000000 recon_lw-2.0.0.dev4849753051/recon_lw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-01 08:27:41.000000 recon_lw-2.0.0.dev4849753051/recon_lw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      219 2023-05-01 08:27:41.000000 recon_lw-2.0.0.dev4849753051/recon_lw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-05-01 08:27:41.000000 recon_lw-2.0.0.dev4849753051/recon_lw.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      275 2023-05-01 08:26:54.000000 recon_lw-2.0.0.dev4849753051/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-01 08:27:41.000000 recon_lw-2.0.0.dev4849753051/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-05-01 08:26:54.000000 recon_lw-2.0.0.dev4849753051/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 11:03:52.000000 recon_lw-2.0.0.dev4850623410/
+-rw-r--r--   0 runner    (1001) docker     (122)       69 2023-05-01 11:03:10.000000 recon_lw-2.0.0.dev4850623410/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-05-01 11:03:52.000000 recon_lw-2.0.0.dev4850623410/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-05-01 11:03:10.000000 recon_lw-2.0.0.dev4850623410/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       76 2023-05-01 11:03:32.000000 recon_lw-2.0.0.dev4850623410/package_info.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 11:03:52.000000 recon_lw-2.0.0.dev4850623410/recon_lw/
+-rw-r--r--   0 runner    (1001) docker     (122)     1871 2023-05-01 11:03:10.000000 recon_lw-2.0.0.dev4850623410/recon_lw/EventsSaver.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2748 2023-05-01 11:03:10.000000 recon_lw-2.0.0.dev4850623410/recon_lw/TimeCacheMatcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-05-01 11:03:10.000000 recon_lw-2.0.0.dev4850623410/recon_lw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13010 2023-05-01 11:03:10.000000 recon_lw-2.0.0.dev4850623410/recon_lw/recon_lw.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20378 2023-05-01 11:03:10.000000 recon_lw-2.0.0.dev4850623410/recon_lw/recon_ob.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14809 2023-05-01 11:03:10.000000 recon_lw-2.0.0.dev4850623410/recon_lw/recon_ob_cross_stream.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 11:03:52.000000 recon_lw-2.0.0.dev4850623410/recon_lw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-05-01 11:03:52.000000 recon_lw-2.0.0.dev4850623410/recon_lw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      374 2023-05-01 11:03:52.000000 recon_lw-2.0.0.dev4850623410/recon_lw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-01 11:03:52.000000 recon_lw-2.0.0.dev4850623410/recon_lw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      219 2023-05-01 11:03:52.000000 recon_lw-2.0.0.dev4850623410/recon_lw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-05-01 11:03:52.000000 recon_lw-2.0.0.dev4850623410/recon_lw.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      275 2023-05-01 11:03:10.000000 recon_lw-2.0.0.dev4850623410/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-01 11:03:52.000000 recon_lw-2.0.0.dev4850623410/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-05-01 11:03:10.000000 recon_lw-2.0.0.dev4850623410/setup.py
```

### Comparing `recon_lw-2.0.0.dev4849753051/recon_lw/EventsSaver.py` & `recon_lw-2.0.0.dev4850623410/recon_lw/EventsSaver.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,28 +2,36 @@
 from datetime import datetime, timedelta
 from th2_data_services.data import Data
 
 
 class EventsSaver:
     def __init__(self, path):
         self._event_sequence = {"name": "recon_lw", "stamp": str(datetime.now().timestamp()), "n": 0}
-        self._buffer = []
+        self._scopes_buffers = {}
         self._path = path
 
     def flush(self):
-        if self._buffer:
-            events = Data(self._buffer)
-            events_file = self._path / (self._buffer[0]["eventId"] + ".pickle")
+        for scope in self._scopes_buffers.keys():
+            self.flush_scope(scope)
+
+    def flush_scope(self, scope):
+        if scope in self._scopes_buffers:
+            events = Data(self._scopes_buffers[scope])
+            events_file = self._path / (scope + "_" + self._scopes_buffers[scope][0]["eventId"] + ".pickle")
             events.build_cache(events_file)
-            self._buffer.clear()
+            self._scopes_buffers[scope].clear()
 
     def save_events(self, batch):
-        self._buffer.extend(batch)
-        if len(self._buffer) > 50000:
-            self.flush()
+        for e in batch:
+            scope = e["scope"] if "scope" in e else "default"
+            if scope not in self._scopes_buffers:
+                self._scopes_buffers[scope] = []
+            self._scopes_buffers[scope].append(e)
+            if len(self._scopes_buffers[scope]) > 50000:
+                self.flush_scope(scope)
 
     def create_event(self, name, type, ok=True, body=None, parentId=None):
         ts = datetime.now()
         e = {"eventId": self._create_event_id(),
              "successful": ok,
              "eventName": name,
              "eventType": type,
```

### Comparing `recon_lw-2.0.0.dev4849753051/recon_lw/TimeCacheMatcher.py` & `recon_lw-2.0.0.dev4850623410/recon_lw/TimeCacheMatcher.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev4849753051/recon_lw/recon_lw.py` & `recon_lw-2.0.0.dev4850623410/recon_lw/recon_lw.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from datetime import datetime, timedelta
 from sortedcontainers import SortedKeyList
 from th2_data_services.data import Data
 from th2_data_services.utils.message_utils import message_utils
 from os import listdir
 from os import path
+from recon_lw.EventsSaver import EventsSaver
 
 
 def time_stamp_key(ts):
     nanos_str = str(ts["nano"]).zfill(9)
     return str(ts["epochSecond"]) + "." + nanos_str
 
 
@@ -148,27 +149,14 @@
 
 
 def create_event_id(event_sequence):
     event_sequence["n"] += 1
     return event_sequence["name"] + "_" + event_sequence["stamp"] +"-" +str(event_sequence["n"])
 
 
-def save_events_standalone(new_chunk, buffer, result_events_path):
-    buffer.extend(new_chunk)
-    if len(buffer) > 50000:
-        dump_buffer(buffer,result_events_path)
-
-
-def dump_buffer(buffer, result_events_path):
-    events = Data(buffer)
-    events_file = result_events_path + "/" + buffer[0]["eventId"] + ".pickle"
-    events.build_cache(events_file)
-    buffer.clear()
-
-
 def create_event(name, type, event_sequence, ok=True, body=None, parentId=None):
     ts = datetime.now()
     e = {"eventId": create_event_id(event_sequence),
          "successful": ok,
          "eventName": name,
          "eventType": type,
          "body": body,
@@ -178,59 +166,56 @@
     return e
 
 
 #{"first_key_func":..., "second_key_func",... "interpret_func"}
 def execute_standalone(message_pickle_path, sessions_list, result_events_path, rules_settings_dict):
     events_buffer = []
     box_ts = datetime.now()
+    events_saver = EventsSaver(result_events_path)
     event_sequence = {"name": "recon_lw", "stamp": str(box_ts.timestamp()), "n": 0}
     root_event = create_event("recon_lw " + box_ts.isoformat(), "Microservice", event_sequence)
 
-    save_events_standalone([root_event], events_buffer, result_events_path)
+    events_saver.save_events([root_event])
     for rule_key, rule_settings in rules_settings_dict.items():
         rule_settings["rule_root_event"] = create_event(rule_key, "LwReconRule",
                                                         event_sequence, parentId=root_event["eventId"])
         if "init_func" not in rule_settings:
             rule_settings["init_func"] = init_matcher
         if "collect_func" not in rule_settings:
             rule_settings["collect_func"] = collect_matcher
         if "flush_func" not in rule_settings:
             rule_settings["flush_func"] = flush_matcher
         rule_settings["init_func"](rule_settings)
 
-    save_events_standalone([r["rule_root_event"] for r in rules_settings_dict.values()],
-                           events_buffer,result_events_path)
+    events_saver.save_events([r["rule_root_event"] for r in rules_settings_dict.values()])
     if sessions_list is not None and len(sessions_list):
         sessions_set = set(sessions_list)
         streams = open_streams(message_pickle_path,
                                lambda n: n[:n.rfind('_')] in sessions_set)
     else:
         streams = open_streams(message_pickle_path)
 
     message_buffer = [None]*100
     buffer_len = 100
     while len(streams)>0:
-        next_batch_len = get_next_batch(streams, message_buffer, buffer_len)
+        next_batch_len = get_next_batch(streams, message_buffer, buffer_len, lambda m: m["timestamp"])
         buffer_to_process = message_buffer
         if next_batch_len < buffer_len:
             buffer_to_process = message_buffer[:next_batch_len]
         for rule_settings in rules_settings_dict.values():
             rule_settings["collect_func"](buffer_to_process, rule_settings)
             ts = buffer_to_process[len(buffer_to_process)-1]["timestamp"]
             rule_settings["flush_func"](ts, rule_settings, event_sequence,
-                                        lambda ev_batch: save_events_standalone(ev_batch, events_buffer,
-                                                                                result_events_path))
+                                        lambda ev_batch: events_saver.save_events(ev_batch))
     #final flush
     for rule_settings in rules_settings_dict.values():
         rule_settings["flush_func"](None, rule_settings, event_sequence,
-                                    lambda ev_batch: save_events_standalone(ev_batch, events_buffer,
-                                                                            result_events_path))
+                                    lambda ev_batch: events_saver.save_events(ev_batch))
     #one final flush
-    if len(events_buffer) > 0:
-        dump_buffer(events_buffer,result_events_path)
+    events_saver.flush()
 
 
 def init_matcher(rule_settings):
     rule_settings["match_index"] = {}
     rule_settings["time_index"] = SortedKeyList(key=lambda t: time_stamp_key(t[0]))
     rule_settings["message_cache"] = {}
 
@@ -298,14 +283,35 @@
     if len(m["body"]) == 0:
         return "error"
     if "protocol" not in m["body"]["metadata"]:
         return "not_defined"
     return m["body"]["metadata"]["protocol"]
 
 
+def open_scoped_events_streams(streams_path, name_filter=None):
+    streams = SortedKeyList(key=lambda t: time_stamp_key(t[0]))
+    files = listdir(streams_path)
+    files.sort()
+    scopes_streams = {}
+    for f in files:
+        if ".pickle" not in f:
+            continue
+        if name_filter is not None and not name_filter(f):
+            continue
+        scope = f[:f.index("_")]
+        if scope not in scopes_streams:
+            scopes_streams[scope] = Data.from_cache_file(path.join(streams_path, f))
+        else:
+            scopes_streams[scope] += Data.from_cache_file(path.join(streams_path, f))
+    for strm in scopes_streams.values():
+        ts0 = {"epochSecond": 0, "nano": 0}
+        streams.add((ts0, iter(strm), None))
+    return streams
+
+
 def open_streams(streams_path, name_filter=None):
     streams = SortedKeyList(key=lambda t: time_stamp_key(t[0]))
     files = listdir(streams_path)
     for f in files:
         if ".pickle" not in f:
             continue
         if name_filter is not None and not name_filter(f):
@@ -313,22 +319,22 @@
         stream = Data.from_cache_file(path.join(streams_path, f))
         ts0 = {"epochSecond": 0, "nano": 0}
         streams.add((ts0, iter(stream), None))
 
     return streams
 
 
-def get_next_batch(streams, batch, b_len):
+def get_next_batch(streams, batch, b_len, get_timestamp_func):
     batch_pos = 0
     batch_len = b_len #len(batch)
     while batch_pos < batch_len and len(streams) > 0:
         next_stream = streams.pop(0)
         try:
             if next_stream[2] is not None:
                 batch[batch_pos] = next_stream[2]
                 batch_pos += 1
-            m = next(next_stream[1])
-            streams.add((m["timestamp"],next_stream[1], m))
+            o = next(next_stream[1])
+            streams.add((get_timestamp_func(o), next_stream[1], o))
         except StopIteration as e:
             continue
     return batch_pos
```

### Comparing `recon_lw-2.0.0.dev4849753051/recon_lw/recon_ob.py` & `recon_lw-2.0.0.dev4850623410/recon_lw/recon_ob.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,14 +112,15 @@
                         log_event = recon_lw.create_event("OrderBook:" + mess["sessionId"],
                                                           "OrderBook",
                                                           event_sequence,
                                                           ok=True,
                                                           body=log_book,
                                                           parentId=parent_event["eventId"])
                         log_event["attachedMessageIds"] = [mess["messageId"]]
+                        log_event["scope"] = mess["sessionId"]
                         events.append(log_event)
 
             results = check_book_rule(book, event_sequence)
             if results is not None:
                 for r in results:
                     if not r["successful"]:
                         r["body"]["operation_params"] = initial_parameters
```

### Comparing `recon_lw-2.0.0.dev4849753051/recon_lw/recon_ob_cross_stream.py` & `recon_lw-2.0.0.dev4850623410/recon_lw/recon_ob_cross_stream.py`

 * *Files 3% similar despite different names*

```diff
@@ -173,15 +173,15 @@
         piece = list(islice(iterable, n))
         if not piece:
             break
         yield piece
 
 
 #{"horizon_dely": 180, full_session: "aaa", aggr_session: "bbb", top_session: "ccc"}
-def ob_compare_streams(source_events, results_path, rules_dict):
+def ob_compare_streams(source_events_path, results_path, rules_dict):
     events_saver = EventsSaver(results_path)
     processors = []
     root_event = events_saver.create_event("recon_lw_ob_streams " + datetime.now().isoformat(), "Microservice")
     events_saver.save_events([root_event])
     for rule_name, rule_params in rules_dict.items():
         rule_root_event = events_saver.create_event(rule_name,"OBStreamsCompareRule", parentId=root_event["eventId"])
         events_saver.save_events([rule_root_event])
@@ -211,20 +211,27 @@
                                                                                                        ok,
                                                                                                        body,
                                                                                                        parentId=rule_root_event["eventId"]),
                                              lambda ev_batch: events_saver.save_events(ev_batch)
                                              )
             processors.append(processor_top)
 
-    order_books_events = source_events.filter(lambda e: e["eventType"] == "OrderBook")
+    #order_books_events = source_events.filter(lambda e: e["eventType"] == "OrderBook")
 
-    buffers = split_every(100, order_books_events)
-    for buffer in buffers:
+    #buffers = split_every(100, order_books_events)
+    streams = recon_lw.open_scoped_events_streams(source_events_path, lambda n: "default_" not in n)
+    message_buffer = [None]*100
+    buffer_len = 100
+    while len(streams)>0:
+        next_batch_len = recon_lw.get_next_batch(streams, message_buffer, buffer_len, lambda e: e["body"]["timestamp"])
+        buffer_to_process = message_buffer
+        if next_batch_len < buffer_len:
+            buffer_to_process = message_buffer[:next_batch_len]
         for p in processors:
-            p.process_objects_batch(buffer)
+            p.process_objects_batch(buffer_to_process)
 
     for p in processors:
         p.flush_all()
 
     events_saver.flush()
```

### Comparing `recon_lw-2.0.0.dev4849753051/setup.py` & `recon_lw-2.0.0.dev4850623410/setup.py`

 * *Files identical despite different names*

