# Comparing `tmp/turbo_queue-0.7.2.tar.gz` & `tmp/turbo_queue-0.7.3.tar.gz`

## Comparing `turbo_queue-0.7.2.tar` & `turbo_queue-0.7.3.tar`

### file list

```diff
@@ -1,14 +1,18 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 turbo_queue-0.7.2/.DS_Store
--rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 turbo_queue-0.7.2/CHANGELOG.md
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 turbo_queue-0.7.2/requirements.txt
--rw-r--r--   0        0        0     3940 2020-02-02 00:00:00.000000 turbo_queue-0.7.2/docs/how_it_works.md
--rw-r--r--   0        0        0   412842 2020-02-02 00:00:00.000000 turbo_queue-0.7.2/docs/monitor_queue.gif
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 turbo_queue-0.7.2/src/turbo_queue/__init__.py
--rw-r--r--   0        0        0    15226 2020-02-02 00:00:00.000000 turbo_queue-0.7.2/src/turbo_queue/_turbo_queue_kafka.py
--rw-r--r--   0        0        0     3493 2020-02-02 00:00:00.000000 turbo_queue-0.7.2/src/turbo_queue/_turbo_queue_multi_task.py
--rw-r--r--   0        0        0    21382 2020-02-02 00:00:00.000000 turbo_queue-0.7.2/src/turbo_queue/turbo_queue.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 turbo_queue-0.7.2/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 turbo_queue-0.7.2/LICENSE
--rw-r--r--   0        0        0     4175 2020-02-02 00:00:00.000000 turbo_queue-0.7.2/README.md
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 turbo_queue-0.7.2/pyproject.toml
--rw-r--r--   0        0        0     4715 2020-02-02 00:00:00.000000 turbo_queue-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 turbo_queue-0.7.3/CHANGELOG.md
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 turbo_queue-0.7.3/requirements.txt
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 turbo_queue-0.7.3/docs/examples.md
+-rw-r--r--   0        0        0     3940 2020-02-02 00:00:00.000000 turbo_queue-0.7.3/docs/how_it_works.md
+-rw-r--r--   0        0        0   412842 2020-02-02 00:00:00.000000 turbo_queue-0.7.3/docs/monitor_queue.gif
+-rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 turbo_queue-0.7.3/docs/examples/kafka_data_pipeline/src/consumer.py
+-rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 turbo_queue-0.7.3/docs/examples/kafka_data_pipeline/src/main.py
+-rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 turbo_queue-0.7.3/docs/examples/kafka_data_pipeline/src/producer.py
+-rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 turbo_queue-0.7.3/docs/examples/kafka_data_pipeline/src/worker.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 turbo_queue-0.7.3/src/turbo_queue/__init__.py
+-rw-r--r--   0        0        0    15226 2020-02-02 00:00:00.000000 turbo_queue-0.7.3/src/turbo_queue/_turbo_queue_kafka.py
+-rw-r--r--   0        0        0     3493 2020-02-02 00:00:00.000000 turbo_queue-0.7.3/src/turbo_queue/_turbo_queue_multi_task.py
+-rw-r--r--   0        0        0    21910 2020-02-02 00:00:00.000000 turbo_queue-0.7.3/src/turbo_queue/turbo_queue.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 turbo_queue-0.7.3/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 turbo_queue-0.7.3/LICENSE
+-rw-r--r--   0        0        0     4251 2020-02-02 00:00:00.000000 turbo_queue-0.7.3/README.md
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 turbo_queue-0.7.3/pyproject.toml
+-rw-r--r--   0        0        0     4791 2020-02-02 00:00:00.000000 turbo_queue-0.7.3/PKG-INFO
```

### Comparing `turbo_queue-0.7.2/CHANGELOG.md` & `turbo_queue-0.7.3/CHANGELOG.md`

 * *Files 16% similar despite different names*

```diff
@@ -4,14 +4,19 @@
 
 ## [Unreleased]
 - improve logging
 - improve documentation
 - examples
 - process specific connectors
 
+## [0.7.3] - 2023-05-01
+
+### Added
+- Add capability for Dequeue to properly resume after pause in process
+
 ## [0.7.2] - 2023-04-20
 
 ### Fixed
 - Update class names in Kafka connector
 
 ## [0.7.1] - 2023-04-20
```

### Comparing `turbo_queue-0.7.2/docs/how_it_works.md` & `turbo_queue-0.7.3/docs/how_it_works.md`

 * *Files identical despite different names*

### Comparing `turbo_queue-0.7.2/docs/monitor_queue.gif` & `turbo_queue-0.7.3/docs/monitor_queue.gif`

 * *Files identical despite different names*

### Comparing `turbo_queue-0.7.2/src/turbo_queue/_turbo_queue_kafka.py` & `turbo_queue-0.7.3/src/turbo_queue/_turbo_queue_kafka.py`

 * *Files identical despite different names*

### Comparing `turbo_queue-0.7.2/src/turbo_queue/_turbo_queue_multi_task.py` & `turbo_queue-0.7.3/src/turbo_queue/_turbo_queue_multi_task.py`

 * *Files identical despite different names*

### Comparing `turbo_queue-0.7.2/src/turbo_queue/turbo_queue.py` & `turbo_queue-0.7.3/src/turbo_queue/turbo_queue.py`

 * *Files 2% similar despite different names*

```diff
@@ -365,14 +365,20 @@
         self._recover_stale("loading_*", "ready")
         self._recover_stale("chosen_*", "ready")
         #
         # for upgrade < 0.2.0.0:
         self._recover_stale("avail_*", "ready")
         self._recover_stale("assigned_*", "ready")
         return
+    
+    def migrate_queue(self):
+        """Utility to move a queue to a new folder.  Can be used at startup if changing a queue name, which also changes it's location.
+
+        Placeholder - WIP
+        """
 
 
 class Enqueue(_TurboQueueBase):
     def __init__(self):
         """class with methods for load the queue"""
         super().__init__()
         self._create_epoch = 1  # default value to start
@@ -497,14 +503,15 @@
 
         """
         super().__init__()
         self.proc_num = proc_num
         self._total_gets = 0
         self._total_batch = 0
         self._auto_cleanup = True
+        self._row_count = 0
 
     #
     # auto_cleanup
     @property
     def auto_cleanup(self):
         return self._auto_cleanup
 
@@ -559,27 +566,33 @@
         """
         if self._db_path == None:
             result = self._get_unload_from_ready()
             if result == False:
                 yield None
             else:
                 self._total_batch += 1
-        # verify table:
-        listOfTables = self._db_conn.execute(
-            """SELECT name FROM sqlite_master WHERE type='table'
-            AND name='logs'; """
-        ).fetchall()
-
-        if listOfTables == []:
-            yield None
-        for row in self._db_conn.execute("SELECT log_data FROM logs"):
+                # verify table:
+                listOfTables = self._db_conn.execute(
+                    """SELECT name FROM sqlite_master WHERE type='table'
+                    AND name='logs'; """
+                ).fetchall()
+
+                if listOfTables == []:
+                    yield None
+                else:
+                    self._row_count = 0
+        if self._row_count == 0:
+            statement = "SELECT log_data FROM logs"
+        else:
+            statement = f"SELECT log_data FROM logs LIMIT -1 OFFSET {self._row_count}"
+        for row in self._db_conn.execute(statement):
             # WIP
             # self.totalMessages += 1
             # pollCount += 1
-            # rowcount += 1
+            self._row_count += 1
             data = json.loads(row[0])
             self._total_gets += 1
             yield data
         if self._auto_cleanup:
             self.clean_up()
         yield None
```

### Comparing `turbo_queue-0.7.2/LICENSE` & `turbo_queue-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `turbo_queue-0.7.2/README.md` & `turbo_queue-0.7.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 ```
 pip install turbo-queue
 ```
 #### Project Status
 WIP - Not ready for PRs yet
 
 # Turbo Queue
-High performance, multi-processing queue. Works across child processes, and even between individual Python applications!
+Build a high performance data-pipeline with Turbo Queue.  A pure Python, shared nothing, multi-processing queue, that works across child processes, and even between individual Python applications!
 
 # Contents
  - [Overview](#overview)
  - [Use Cases](#use-cases)
  - [Solution](#solution)
  - [Results](#results)
  - [Quickstart](#quickstart)
```

### Comparing `turbo_queue-0.7.2/pyproject.toml` & `turbo_queue-0.7.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "turbo-queue"
-version = "0.7.2"
+version = "0.7.3"
 authors = [
   { name="Dave Waters", email="dave@1waters.com" },
 ]
 description = "A Python module to improve performance of multiprocessing queues"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `turbo_queue-0.7.2/PKG-INFO` & `turbo_queue-0.7.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: turbo-queue
-Version: 0.7.2
+Version: 0.7.3
 Summary: A Python module to improve performance of multiprocessing queues
 Project-URL: Homepage, https://github.com/davewat/turbo-queue
 Project-URL: Bug Tracker, https://github.com/davewat/turbo-queue/issues
 Author-email: Dave Waters <dave@1waters.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -18,15 +18,15 @@
 ```
 pip install turbo-queue
 ```
 #### Project Status
 WIP - Not ready for PRs yet
 
 # Turbo Queue
-High performance, multi-processing queue. Works across child processes, and even between individual Python applications!
+Build a high performance data-pipeline with Turbo Queue.  A pure Python, shared nothing, multi-processing queue, that works across child processes, and even between individual Python applications!
 
 # Contents
  - [Overview](#overview)
  - [Use Cases](#use-cases)
  - [Solution](#solution)
  - [Results](#results)
  - [Quickstart](#quickstart)
```

