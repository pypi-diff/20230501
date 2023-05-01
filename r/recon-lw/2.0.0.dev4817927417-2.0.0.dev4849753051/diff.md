# Comparing `tmp/recon_lw-2.0.0.dev4817927417.tar.gz` & `tmp/recon_lw-2.0.0.dev4849753051.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/recon_lw-2.0.0.dev4817927417.tar", last modified: Thu Apr 27 09:00:42 2023, max compression
+gzip compressed data, was "dist/recon_lw-2.0.0.dev4849753051.tar", last modified: Mon May  1 08:27:41 2023, max compression
```

## Comparing `recon_lw-2.0.0.dev4817927417.tar` & `recon_lw-2.0.0.dev4849753051.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 09:00:42.000000 recon_lw-2.0.0.dev4817927417/
--rw-r--r--   0 runner    (1001) docker     (122)       69 2023-04-27 08:59:55.000000 recon_lw-2.0.0.dev4817927417/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-04-27 09:00:42.000000 recon_lw-2.0.0.dev4817927417/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-04-27 08:59:55.000000 recon_lw-2.0.0.dev4817927417/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       76 2023-04-27 09:00:12.000000 recon_lw-2.0.0.dev4817927417/package_info.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 09:00:42.000000 recon_lw-2.0.0.dev4817927417/recon_lw/
--rw-r--r--   0 runner    (1001) docker     (122)     1432 2023-04-27 08:59:55.000000 recon_lw-2.0.0.dev4817927417/recon_lw/EventsSaver.py
--rw-r--r--   0 runner    (1001) docker     (122)     2748 2023-04-27 08:59:55.000000 recon_lw-2.0.0.dev4817927417/recon_lw/TimeCacheMatcher.py
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-04-27 08:59:55.000000 recon_lw-2.0.0.dev4817927417/recon_lw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12849 2023-04-27 08:59:55.000000 recon_lw-2.0.0.dev4817927417/recon_lw/recon_lw.py
--rw-r--r--   0 runner    (1001) docker     (122)    20312 2023-04-27 08:59:55.000000 recon_lw-2.0.0.dev4817927417/recon_lw/recon_ob.py
--rw-r--r--   0 runner    (1001) docker     (122)    14282 2023-04-27 08:59:55.000000 recon_lw-2.0.0.dev4817927417/recon_lw/recon_ob_cross_stream.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 09:00:42.000000 recon_lw-2.0.0.dev4817927417/recon_lw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-04-27 09:00:42.000000 recon_lw-2.0.0.dev4817927417/recon_lw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      374 2023-04-27 09:00:42.000000 recon_lw-2.0.0.dev4817927417/recon_lw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-27 09:00:42.000000 recon_lw-2.0.0.dev4817927417/recon_lw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      219 2023-04-27 09:00:42.000000 recon_lw-2.0.0.dev4817927417/recon_lw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-04-27 09:00:42.000000 recon_lw-2.0.0.dev4817927417/recon_lw.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      275 2023-04-27 08:59:55.000000 recon_lw-2.0.0.dev4817927417/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-27 09:00:42.000000 recon_lw-2.0.0.dev4817927417/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-04-27 08:59:55.000000 recon_lw-2.0.0.dev4817927417/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 08:27:41.000000 recon_lw-2.0.0.dev4849753051/
+-rw-r--r--   0 runner    (1001) docker     (122)       69 2023-05-01 08:26:54.000000 recon_lw-2.0.0.dev4849753051/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-05-01 08:27:41.000000 recon_lw-2.0.0.dev4849753051/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-05-01 08:26:54.000000 recon_lw-2.0.0.dev4849753051/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       76 2023-05-01 08:27:19.000000 recon_lw-2.0.0.dev4849753051/package_info.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 08:27:41.000000 recon_lw-2.0.0.dev4849753051/recon_lw/
+-rw-r--r--   0 runner    (1001) docker     (122)     1432 2023-05-01 08:26:54.000000 recon_lw-2.0.0.dev4849753051/recon_lw/EventsSaver.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2748 2023-05-01 08:26:54.000000 recon_lw-2.0.0.dev4849753051/recon_lw/TimeCacheMatcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-05-01 08:26:54.000000 recon_lw-2.0.0.dev4849753051/recon_lw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12849 2023-05-01 08:26:54.000000 recon_lw-2.0.0.dev4849753051/recon_lw/recon_lw.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20315 2023-05-01 08:26:54.000000 recon_lw-2.0.0.dev4849753051/recon_lw/recon_ob.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14371 2023-05-01 08:26:54.000000 recon_lw-2.0.0.dev4849753051/recon_lw/recon_ob_cross_stream.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 08:27:41.000000 recon_lw-2.0.0.dev4849753051/recon_lw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-05-01 08:27:41.000000 recon_lw-2.0.0.dev4849753051/recon_lw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      374 2023-05-01 08:27:41.000000 recon_lw-2.0.0.dev4849753051/recon_lw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-01 08:27:41.000000 recon_lw-2.0.0.dev4849753051/recon_lw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      219 2023-05-01 08:27:41.000000 recon_lw-2.0.0.dev4849753051/recon_lw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-05-01 08:27:41.000000 recon_lw-2.0.0.dev4849753051/recon_lw.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      275 2023-05-01 08:26:54.000000 recon_lw-2.0.0.dev4849753051/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-01 08:27:41.000000 recon_lw-2.0.0.dev4849753051/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-05-01 08:26:54.000000 recon_lw-2.0.0.dev4849753051/setup.py
```

### Comparing `recon_lw-2.0.0.dev4817927417/recon_lw/EventsSaver.py` & `recon_lw-2.0.0.dev4849753051/recon_lw/EventsSaver.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev4817927417/recon_lw/TimeCacheMatcher.py` & `recon_lw-2.0.0.dev4849753051/recon_lw/TimeCacheMatcher.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev4817927417/recon_lw/recon_lw.py` & `recon_lw-2.0.0.dev4849753051/recon_lw/recon_lw.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev4817927417/recon_lw/recon_ob.py` & `recon_lw-2.0.0.dev4849753051/recon_lw/recon_ob.py`

 * *Files 0% similar despite different names*

```diff
@@ -198,15 +198,15 @@
                                      ok=False,
                                      body={"seq_num": item[0]},
                                      parentId=rule_settings["rule_root_event"]["eventId"])
         d_ev["attachedMessageIds"] = [item[1], item[2]]
         dupl_events.append(d_ev)
     save_events_func(dupl_events)
     duplicates.clear()
-    flush_sequence_clear_cache(n_processed,rule_settings["sequence_cache"])
+    flush_sequence_clear_cache(len(seq_batch),rule_settings["sequence_cache"])
 
 
 def init_aggr_seq(order_book):
     order_book["aggr_seq"] = {"top_v": 0, "top_delta": 0, "limit_v": 0, "limit_delta": 0}
 
 
 def reflect_price_update_in_version(side, price, order_book):
```

### Comparing `recon_lw-2.0.0.dev4817927417/recon_lw/recon_ob_cross_stream.py` & `recon_lw-2.0.0.dev4849753051/recon_lw/recon_ob_cross_stream.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,15 +26,15 @@
             full_levels.sort(reverse=True)
         aggr_levels = aggr_book[side + "_aggr"]
         for i in range(aggr_book["aggr_max_levels"]):
             if i < len(full_levels) and i < len(aggr_levels):
                 price_condition = full_levels[i] == aggr_levels[i]["price"]
                 num_orders_condition = len(full_book[side][full_levels[i]]) == \
                                        (aggr_levels[i]["real_num_orders"] + aggr_levels[i]["impl_num_orders"])
-                size_condition = sum(full_book[side][full_levels[i]].vales()) == \
+                size_condition = sum(full_book[side][full_levels[i]].values()) == \
                                  (aggr_levels[i]["real_qty"] + aggr_levels[i]["impl_qty"])
                 if not (price_condition and num_orders_condition and size_condition):
                     problems.append({"synopsys": synopsys(price_condition, num_orders_condition, size_condition),
                                      "side": side,
                                      "level": i+1})
             elif i >= len(full_levels) and i >= len(aggr_levels):
                 break
@@ -128,15 +128,15 @@
         save_events([error_event])
     elif match[1] is not None:
         error_event = create_event("StreamMismatchNoFull",
                                    "StreamMismatchNoFull",
                                    False,
                                    {"aggr_book_event": match[1]["eventId"],
                                     "book_id": match[1]["body"]["book_id"],
-                                    "version": match[1]["body"]["aggr_seq"]["limit_v"]})
+                                    "version": match[1]["body"]["aggr_seq"]["limit_v"], "sessionId": match[1]["body"]["sessionId"]})
         save_events([error_event])
 
 
 def ob_compare_interpret_match_top(match, custom_settings, create_event, save_events):
     if match[0] is not None and match[1] is not None:
         comp_res = compare_full_vs_top(match[0]["body"],match[1]["body"])
         if len(comp_res) > 0:
@@ -159,15 +159,15 @@
         save_events([error_event])
     elif match[1] is not None:
         error_event = create_event("StreamMismatchNoFull",
                                    "StreamMismatchNoFull",
                                    False,
                                    {"top_book_event": match[1]["eventId"],
                                     "book_id": match[1]["body"]["book_id"],
-                                    "version": match[1]["body"]["aggr_seq"]["limit_v"]})
+                                    "version": match[1]["body"]["aggr_seq"]["limit_v"], "sessionId": match[1]["body"]["sessionId"]})
         save_events([error_event])
 
 
 def split_every(n, data):
     iterable = iter(data)
     while 1:
         piece = list(islice(iterable, n))
```

### Comparing `recon_lw-2.0.0.dev4817927417/setup.py` & `recon_lw-2.0.0.dev4849753051/setup.py`

 * *Files identical despite different names*

