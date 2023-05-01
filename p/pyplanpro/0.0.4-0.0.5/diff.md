# Comparing `tmp/pyplanpro-0.0.4.tar.gz` & `tmp/pyplanpro-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyplanpro-0.0.4.tar", last modified: Fri Apr 28 07:53:27 2023, max compression
+gzip compressed data, was "pyplanpro-0.0.5.tar", last modified: Mon May  1 14:44:17 2023, max compression
```

## Comparing `pyplanpro-0.0.4.tar` & `pyplanpro-0.0.5.tar`

### file list

```diff
@@ -1,29 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:53:27.014474 pyplanpro-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-04-28 07:53:14.000000 pyplanpro-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-04-28 07:53:27.014474 pyplanpro-0.0.4/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:53:27.010474 pyplanpro-0.0.4/PyPlanPro/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-28 07:53:14.000000 pyplanpro-0.0.4/PyPlanPro/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:53:27.010474 pyplanpro-0.0.4/PyPlanPro/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 07:53:14.000000 pyplanpro-0.0.4/PyPlanPro/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-04-28 07:53:14.000000 pyplanpro-0.0.4/PyPlanPro/models/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-28 07:53:14.000000 pyplanpro-0.0.4/PyPlanPro/models/resource_group.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-28 07:53:14.000000 pyplanpro-0.0.4/PyPlanPro/models/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:53:27.010474 pyplanpro-0.0.4/PyPlanPro/scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 07:53:14.000000 pyplanpro-0.0.4/PyPlanPro/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-28 07:53:14.000000 pyplanpro-0.0.4/PyPlanPro/scheduler/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     9081 2023-04-28 07:53:14.000000 pyplanpro-0.0.4/PyPlanPro/scheduler/heuristic_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)    12129 2023-04-28 07:53:14.000000 pyplanpro-0.0.4/PyPlanPro/scheduler/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-04-28 07:53:14.000000 pyplanpro-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:53:27.014474 pyplanpro-0.0.4/pyplanpro.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-04-28 07:53:26.000000 pyplanpro-0.0.4/pyplanpro.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-04-28 07:53:26.000000 pyplanpro-0.0.4/pyplanpro.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 07:53:26.000000 pyplanpro-0.0.4/pyplanpro.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-28 07:53:26.000000 pyplanpro-0.0.4/pyplanpro.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-28 07:53:26.000000 pyplanpro-0.0.4/pyplanpro.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 07:53:27.014474 pyplanpro-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-28 07:53:14.000000 pyplanpro-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:53:27.014474 pyplanpro-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 07:53:14.000000 pyplanpro-0.0.4/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:53:27.014474 pyplanpro-0.0.4/tests/stress/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 07:53:14.000000 pyplanpro-0.0.4/tests/stress/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 07:53:14.000000 pyplanpro-0.0.4/tests/stress/test_stress_scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 14:44:17.001349 pyplanpro-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-05-01 14:44:05.000000 pyplanpro-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-05-01 14:44:17.001349 pyplanpro-0.0.5/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 14:44:16.997349 pyplanpro-0.0.5/PyPlanPro/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-01 14:44:05.000000 pyplanpro-0.0.5/PyPlanPro/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 14:44:16.997349 pyplanpro-0.0.5/PyPlanPro/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 14:44:05.000000 pyplanpro-0.0.5/PyPlanPro/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-05-01 14:44:05.000000 pyplanpro-0.0.5/PyPlanPro/models/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-01 14:44:05.000000 pyplanpro-0.0.5/PyPlanPro/models/resource_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-05-01 14:44:05.000000 pyplanpro-0.0.5/PyPlanPro/models/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 14:44:16.997349 pyplanpro-0.0.5/PyPlanPro/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 14:44:05.000000 pyplanpro-0.0.5/PyPlanPro/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-01 14:44:05.000000 pyplanpro-0.0.5/PyPlanPro/scheduler/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9633 2023-05-01 14:44:05.000000 pyplanpro-0.0.5/PyPlanPro/scheduler/heuristic_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12129 2023-05-01 14:44:05.000000 pyplanpro-0.0.5/PyPlanPro/scheduler/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-05-01 14:44:05.000000 pyplanpro-0.0.5/PyPlanPro/scheduler/scheduler_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-01 14:44:05.000000 pyplanpro-0.0.5/PyPlanPro/scheduler/visualizations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-05-01 14:44:05.000000 pyplanpro-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 14:44:16.997349 pyplanpro-0.0.5/pyplanpro.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-05-01 14:44:16.000000 pyplanpro-0.0.5/pyplanpro.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-01 14:44:16.000000 pyplanpro-0.0.5/pyplanpro.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 14:44:16.000000 pyplanpro-0.0.5/pyplanpro.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-01 14:44:16.000000 pyplanpro-0.0.5/pyplanpro.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-01 14:44:16.000000 pyplanpro-0.0.5/pyplanpro.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 14:44:17.001349 pyplanpro-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-05-01 14:44:05.000000 pyplanpro-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 14:44:17.001349 pyplanpro-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 14:44:05.000000 pyplanpro-0.0.5/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 14:44:17.001349 pyplanpro-0.0.5/tests/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 14:44:05.000000 pyplanpro-0.0.5/tests/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-05-01 14:44:05.000000 pyplanpro-0.0.5/tests/scheduler/test_heuristic_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 14:44:05.000000 pyplanpro-0.0.5/tests/scheduler/test_scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 14:44:17.001349 pyplanpro-0.0.5/tests/stress/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 14:44:05.000000 pyplanpro-0.0.5/tests/stress/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 14:44:05.000000 pyplanpro-0.0.5/tests/stress/test_stress_scheduler.py
```

### Comparing `pyplanpro-0.0.4/LICENSE` & `pyplanpro-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyplanpro-0.0.4/PKG-INFO` & `pyplanpro-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyplanpro
-Version: 0.0.4
+Version: 0.0.5
 Summary: Task scheduler for python
 Home-page: https://github.com/Oestergaard-A-S/PyPlanPro
 Author: Jacob Østergaard Nielsen
 Author-email: jaoe@oestergaard-as.dk
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyplanpro-0.0.4/PyPlanPro/models/resource_group.py` & `pyplanpro-0.0.5/PyPlanPro/models/resource_group.py`

 * *Files identical despite different names*

### Comparing `pyplanpro-0.0.4/PyPlanPro/models/task.py` & `pyplanpro-0.0.5/PyPlanPro/models/task.py`

 * *Files identical despite different names*

### Comparing `pyplanpro-0.0.4/PyPlanPro/scheduler/heuristic_solver.py` & `pyplanpro-0.0.5/PyPlanPro/scheduler/heuristic_solver.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,45 +8,60 @@
 
     def solve(self):
         task_ids_ordered = self._get_task_order(self.tasks)
         task_dict = {task.id: task for task in self.tasks}
         task_vars = {task.id: {} for task in self.tasks}
         resource_interval_trees = self._get_resource_interval_trees(self.resources)
 
-        for task_id in task_ids_ordered:
+        unscheduled_tasks = []
+        for i, task_id in enumerate(task_ids_ordered):
             task = task_dict[task_id]
             # get max_start_time from max predecessors end
             max_start_time = max((task_vars[pred.id].get('task_end',0) for pred in task.predecessors), default=0)
             
             # find the resource who completes the task first
             fastest_resource = self._get_fastest_resource(task,resource_interval_trees, max_start_time)
             if fastest_resource is None:
-                print(f"No resource could be found for task_id = {task.id}")
+                unscheduled_tasks.append(task.id)
+                self._update_task_vars_unscheduled(task_vars, task)
                 continue
-            # update task_vars with assigned resource, task_start and task_end
-            
-            task_values = {
-                "assigned_resource": fastest_resource["resource"], 
-                "task_start": fastest_resource["start_time"],
-                "task_end" : fastest_resource["end_time"],
-                "task_intervals" : fastest_resource["interval_tree"]
-                }
-            
-            task_vars[task.id].update(task_values)
+
+            self._update_task_vars_scheduled(task_vars, task, fastest_resource)
 
             # update resource_intervals
-            resource_interval_trees = self._update_resource_interval_trees(
+            self._update_resource_interval_trees(
                 resource_interval_trees= resource_interval_trees,
                 resource_id= fastest_resource["resource"].id,
                 interval_tree_index= fastest_resource["interval_index"],
-                task_start= fastest_resource["start_time"],
-                task_end= fastest_resource["end_time"]
+                task_start= fastest_resource["task_start"],
+                task_end= fastest_resource["task_end"]
             )
-        return task_vars
+
+        return list(task_vars.values()) # Return values of the dictionary as a list
     
+    def _update_task_vars_unscheduled(self, task_vars, task):
+        task_values = {
+            "task_id": task.id,
+            "assigned_resource_id": None,
+            "task_start": None,
+            "task_end": None,
+            "task_intervals": None
+        }
+        task_vars[task.id] = task_values
+
+    def _update_task_vars_scheduled(self, task_vars, task, fastest_resource):
+        task_values = {
+            "task_id": task.id,
+            "assigned_resource_id": fastest_resource["resource"].id,
+            "task_start": fastest_resource["task_start"],
+            "task_end": fastest_resource["task_end"],
+            "task_intervals": [(interval.begin, interval.end) for interval in sorted(fastest_resource["task_interval_tree"])]
+        }
+        task_vars[task.id] = task_values
+
     def _get_task_order(self, tasks):
         """
         Returns a list of task IDs in the order required to complete them as quickly as possible while considering task priorities.
 
         :param tasks: List of tasks with durations, predecessors, and priorities.
         :return: List of task IDs in the order required to complete them as quickly as possible while considering task priorities.
         """
@@ -118,41 +133,40 @@
         """Returns the resource with the earliest end time for a task."""
         resource_start_ends = []
         for resource in task.get_resources():
             resource_interval = resource_intervals[resource.id]
             for interval_index, interval in enumerate(resource_interval):
                 if interval["duration"] < task.duration:
                     continue
-                start, end, interval_tree = self._get_task_earliest_start_end(interval["slots"], task.duration, max_start_time)
-                if start is not None:
+                task_start, task_end, task_interval_tree = self._get_task_earliest_start_end(interval["slots"], task.duration, max_start_time)
+                if task_start is not None:
                     resource_start_ends.append({
                         "resource": resource,
                         "interval_index": interval_index,
-                        "start_time": start,
-                        "end_time": end,
-                        "interval_tree" : interval_tree 
+                        "task_start": task_start,
+                        "task_end": task_end,
+                        "task_interval_tree" : task_interval_tree 
                     })
         if not resource_start_ends:
             return None
-        return min(resource_start_ends, key=lambda x: x['end_time']) 
+        return min(resource_start_ends, key=lambda x: x['task_end']) 
 
     def _update_resource_interval_trees(self, resource_interval_trees, resource_id, interval_tree_index, task_start, task_end):
         interval_tree = resource_interval_trees[resource_id].pop(interval_tree_index)
         new_intervals_slots = self._chop_and_split_interval_tree(interval_tree["slots"], task_start, task_end)
         for interval_slots in new_intervals_slots:
             if interval_slots:
                 new_interval = self._create_resource_interval_tree(interval_slots)
                 resource_interval_trees[resource_id].insert(interval_tree_index, new_interval)
-        return resource_interval_trees
     
     def _get_task_earliest_start_end(self, interval_tree, task_duration, latest_start_time=0):
         remaining_duration = task_duration
         interval_tree.chop(0,latest_start_time)
         task_start = interval_tree.begin()
-        for interval in interval_tree:
+        for interval in sorted(interval_tree):
             start, end = interval.begin, interval.end
             interval_duration = end-start
             if interval_duration >= remaining_duration:
                 task_end = end - (interval_duration - remaining_duration)
                 task_interval_tree = self._get_task_interval_tree(interval_tree, task_start, task_end)
                 return (task_start, task_end, task_interval_tree) 
             remaining_duration -= interval_duration
```

### Comparing `pyplanpro-0.0.4/PyPlanPro/scheduler/optimizer.py` & `pyplanpro-0.0.5/PyPlanPro/scheduler/optimizer.py`

 * *Files identical despite different names*

### Comparing `pyplanpro-0.0.4/README.md` & `pyplanpro-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `pyplanpro-0.0.4/pyplanpro.egg-info/PKG-INFO` & `pyplanpro-0.0.5/pyplanpro.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyplanpro
-Version: 0.0.4
+Version: 0.0.5
 Summary: Task scheduler for python
 Home-page: https://github.com/Oestergaard-A-S/PyPlanPro
 Author: Jacob Østergaard Nielsen
 Author-email: jaoe@oestergaard-as.dk
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyplanpro-0.0.4/pyplanpro.egg-info/SOURCES.txt` & `pyplanpro-0.0.5/pyplanpro.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -6,15 +6,20 @@
 PyPlanPro/models/resource.py
 PyPlanPro/models/resource_group.py
 PyPlanPro/models/task.py
 PyPlanPro/scheduler/__init__.py
 PyPlanPro/scheduler/core.py
 PyPlanPro/scheduler/heuristic_solver.py
 PyPlanPro/scheduler/optimizer.py
+PyPlanPro/scheduler/scheduler_result.py
+PyPlanPro/scheduler/visualizations.py
 pyplanpro.egg-info/PKG-INFO
 pyplanpro.egg-info/SOURCES.txt
 pyplanpro.egg-info/dependency_links.txt
 pyplanpro.egg-info/requires.txt
 pyplanpro.egg-info/top_level.txt
 tests/__init__.py
+tests/scheduler/__init__.py
+tests/scheduler/test_heuristic_solver.py
+tests/scheduler/test_scheduler.py
 tests/stress/__init__.py
 tests/stress/test_stress_scheduler.py
```

### Comparing `pyplanpro-0.0.4/setup.py` & `pyplanpro-0.0.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         line.strip()
         for line in read(path).split("\n")
         if not line.startswith(('"', "#", "-", "git+"))
     ]
 
 setup(
     name='pyplanpro',
-    version='0.0.4',
+    version='0.0.5',
     author='Jacob Østergaard Nielsen',
     author_email='jaoe@oestergaard-as.dk',
     description='Task scheduler for python',
     long_description=read("README.md"),
     long_description_content_type='text/markdown',
     url='https://github.com/Oestergaard-A-S/PyPlanPro',
     install_requires= read_requirements("requirements.txt"),
```

