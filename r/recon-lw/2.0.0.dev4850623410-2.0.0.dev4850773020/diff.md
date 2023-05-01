# Comparing `tmp/recon_lw-2.0.0.dev4850623410.tar.gz` & `tmp/recon_lw-2.0.0.dev4850773020.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/recon_lw-2.0.0.dev4850623410.tar", last modified: Mon May  1 11:03:52 2023, max compression
+gzip compressed data, was "dist/recon_lw-2.0.0.dev4850773020.tar", last modified: Mon May  1 11:28:10 2023, max compression
```

## Comparing `recon_lw-2.0.0.dev4850623410.tar` & `recon_lw-2.0.0.dev4850773020.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 11:03:52.000000 recon_lw-2.0.0.dev4850623410/
--rw-r--r--   0 runner    (1001) docker     (122)       69 2023-05-01 11:03:10.000000 recon_lw-2.0.0.dev4850623410/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-05-01 11:03:52.000000 recon_lw-2.0.0.dev4850623410/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-05-01 11:03:10.000000 recon_lw-2.0.0.dev4850623410/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       76 2023-05-01 11:03:32.000000 recon_lw-2.0.0.dev4850623410/package_info.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 11:03:52.000000 recon_lw-2.0.0.dev4850623410/recon_lw/
--rw-r--r--   0 runner    (1001) docker     (122)     1871 2023-05-01 11:03:10.000000 recon_lw-2.0.0.dev4850623410/recon_lw/EventsSaver.py
--rw-r--r--   0 runner    (1001) docker     (122)     2748 2023-05-01 11:03:10.000000 recon_lw-2.0.0.dev4850623410/recon_lw/TimeCacheMatcher.py
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-05-01 11:03:10.000000 recon_lw-2.0.0.dev4850623410/recon_lw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13010 2023-05-01 11:03:10.000000 recon_lw-2.0.0.dev4850623410/recon_lw/recon_lw.py
--rw-r--r--   0 runner    (1001) docker     (122)    20378 2023-05-01 11:03:10.000000 recon_lw-2.0.0.dev4850623410/recon_lw/recon_ob.py
--rw-r--r--   0 runner    (1001) docker     (122)    14809 2023-05-01 11:03:10.000000 recon_lw-2.0.0.dev4850623410/recon_lw/recon_ob_cross_stream.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 11:03:52.000000 recon_lw-2.0.0.dev4850623410/recon_lw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-05-01 11:03:52.000000 recon_lw-2.0.0.dev4850623410/recon_lw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      374 2023-05-01 11:03:52.000000 recon_lw-2.0.0.dev4850623410/recon_lw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-01 11:03:52.000000 recon_lw-2.0.0.dev4850623410/recon_lw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      219 2023-05-01 11:03:52.000000 recon_lw-2.0.0.dev4850623410/recon_lw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-05-01 11:03:52.000000 recon_lw-2.0.0.dev4850623410/recon_lw.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      275 2023-05-01 11:03:10.000000 recon_lw-2.0.0.dev4850623410/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-01 11:03:52.000000 recon_lw-2.0.0.dev4850623410/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-05-01 11:03:10.000000 recon_lw-2.0.0.dev4850623410/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 11:28:10.000000 recon_lw-2.0.0.dev4850773020/
+-rw-r--r--   0 runner    (1001) docker     (122)       69 2023-05-01 11:27:30.000000 recon_lw-2.0.0.dev4850773020/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-05-01 11:28:10.000000 recon_lw-2.0.0.dev4850773020/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-05-01 11:27:30.000000 recon_lw-2.0.0.dev4850773020/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       76 2023-05-01 11:27:52.000000 recon_lw-2.0.0.dev4850773020/package_info.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 11:28:10.000000 recon_lw-2.0.0.dev4850773020/recon_lw/
+-rw-r--r--   0 runner    (1001) docker     (122)     1871 2023-05-01 11:27:30.000000 recon_lw-2.0.0.dev4850773020/recon_lw/EventsSaver.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2748 2023-05-01 11:27:30.000000 recon_lw-2.0.0.dev4850773020/recon_lw/TimeCacheMatcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-05-01 11:27:30.000000 recon_lw-2.0.0.dev4850773020/recon_lw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13010 2023-05-01 11:27:30.000000 recon_lw-2.0.0.dev4850773020/recon_lw/recon_lw.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20404 2023-05-01 11:27:30.000000 recon_lw-2.0.0.dev4850773020/recon_lw/recon_ob.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14809 2023-05-01 11:27:30.000000 recon_lw-2.0.0.dev4850773020/recon_lw/recon_ob_cross_stream.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 11:28:10.000000 recon_lw-2.0.0.dev4850773020/recon_lw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-05-01 11:28:10.000000 recon_lw-2.0.0.dev4850773020/recon_lw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      374 2023-05-01 11:28:10.000000 recon_lw-2.0.0.dev4850773020/recon_lw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-01 11:28:10.000000 recon_lw-2.0.0.dev4850773020/recon_lw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      219 2023-05-01 11:28:10.000000 recon_lw-2.0.0.dev4850773020/recon_lw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-05-01 11:28:10.000000 recon_lw-2.0.0.dev4850773020/recon_lw.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      275 2023-05-01 11:27:30.000000 recon_lw-2.0.0.dev4850773020/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-01 11:28:10.000000 recon_lw-2.0.0.dev4850773020/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-05-01 11:27:30.000000 recon_lw-2.0.0.dev4850773020/setup.py
```

### Comparing `recon_lw-2.0.0.dev4850623410/recon_lw/EventsSaver.py` & `recon_lw-2.0.0.dev4850773020/recon_lw/EventsSaver.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev4850623410/recon_lw/TimeCacheMatcher.py` & `recon_lw-2.0.0.dev4850773020/recon_lw/TimeCacheMatcher.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev4850623410/recon_lw/recon_lw.py` & `recon_lw-2.0.0.dev4850773020/recon_lw/recon_lw.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev4850623410/recon_lw/recon_ob.py` & `recon_lw-2.0.0.dev4850773020/recon_lw/recon_ob.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,14 +141,15 @@
         seq = m[0]
         mess = m[1]
         #process gaps
         if "gap" in mess:
             gap_event = recon_lw.create_event("SeqGap:" + parent_event["eventName"],"SeqGap",event_sequence,ok=False,
                                               body={"seq_num": seq} ,parentId=parent_event["eventId"])
             events.append(gap_event)
+            n_processed += 1
             continue
         chunk = message_utils.expand_message(mess)
         for m_upd in chunk:
             process_market_data_update(m_upd, events, books_cache, get_book_id_func, update_book_rule,
                                        check_book_rule, event_sequence, parent_event, initial_book_params,
                                        log_books_filter)
         n_processed += 1
@@ -199,15 +200,15 @@
                                      ok=False,
                                      body={"seq_num": item[0]},
                                      parentId=rule_settings["rule_root_event"]["eventId"])
         d_ev["attachedMessageIds"] = [item[1], item[2]]
         dupl_events.append(d_ev)
     save_events_func(dupl_events)
     duplicates.clear()
-    flush_sequence_clear_cache(len(seq_batch),rule_settings["sequence_cache"])
+    flush_sequence_clear_cache(n_processed,rule_settings["sequence_cache"])
 
 
 def init_aggr_seq(order_book):
     order_book["aggr_seq"] = {"top_v": 0, "top_delta": 0, "limit_v": 0, "limit_delta": 0}
 
 
 def reflect_price_update_in_version(side, price, order_book):
```

### Comparing `recon_lw-2.0.0.dev4850623410/recon_lw/recon_ob_cross_stream.py` & `recon_lw-2.0.0.dev4850773020/recon_lw/recon_ob_cross_stream.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev4850623410/setup.py` & `recon_lw-2.0.0.dev4850773020/setup.py`

 * *Files identical despite different names*

