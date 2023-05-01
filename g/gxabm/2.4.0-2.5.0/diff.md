# Comparing `tmp/gxabm-2.4.0.tar.gz` & `tmp/gxabm-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gxabm-2.4.0.tar", last modified: Sat Apr 29 23:25:16 2023, max compression
+gzip compressed data, was "gxabm-2.5.0.tar", last modified: Mon May  1 01:44:13 2023, max compression
```

## Comparing `gxabm-2.4.0.tar` & `gxabm-2.5.0.tar`

### file list

```diff
@@ -1,41 +1,42 @@
-drwxr-xr-x   0 suderman   (502) staff       (20)        0 2023-04-29 23:25:16.546042 gxabm-2.4.0/
--rw-r--r--   0 suderman   (502) staff       (20)       42 2022-03-07 12:56:12.000000 gxabm-2.4.0/MANIFEST.in
--rw-r--r--   0 suderman   (502) staff       (20)    19487 2023-04-29 23:25:16.545859 gxabm-2.4.0/PKG-INFO
--rw-r--r--   0 suderman   (502) staff       (20)    16395 2022-03-22 19:06:33.000000 gxabm-2.4.0/README.md
-drwxr-xr-x   0 suderman   (502) staff       (20)        0 2023-04-29 23:25:16.537356 gxabm-2.4.0/abm/
--rw-r--r--   0 suderman   (502) staff       (20)        6 2023-04-29 23:24:17.000000 gxabm-2.4.0/abm/VERSION
--rw-r--r--   0 suderman   (502) staff       (20)      290 2022-03-07 12:56:12.000000 gxabm-2.4.0/abm/__init__.py
--rw-r--r--   0 suderman   (502) staff       (20)     8362 2023-04-24 20:24:38.000000 gxabm-2.4.0/abm/__main__.py
-drwxr-xr-x   0 suderman   (502) staff       (20)        0 2023-04-29 23:25:16.542893 gxabm-2.4.0/abm/lib/
--rw-r--r--   0 suderman   (502) staff       (20)      447 2022-03-07 12:56:12.000000 gxabm-2.4.0/abm/lib/__init__.py
--rw-r--r--   0 suderman   (502) staff       (20)    18434 2023-04-27 20:18:52.000000 gxabm-2.4.0/abm/lib/benchmark.py
--rw-r--r--   0 suderman   (502) staff       (20)     7812 2022-10-19 17:36:24.000000 gxabm-2.4.0/abm/lib/cloudlaunch.py
--rw-r--r--   0 suderman   (502) staff       (20)     7556 2023-04-29 23:23:52.000000 gxabm-2.4.0/abm/lib/common.py
--rw-r--r--   0 suderman   (502) staff       (20)     5433 2022-10-19 17:36:24.000000 gxabm-2.4.0/abm/lib/config.py
--rw-r--r--   0 suderman   (502) staff       (20)     6483 2023-04-27 20:18:52.000000 gxabm-2.4.0/abm/lib/dataset.py
--rw-r--r--   0 suderman   (502) staff       (20)     7661 2023-04-29 03:35:40.000000 gxabm-2.4.0/abm/lib/experiment.py
--rw-r--r--   0 suderman   (502) staff       (20)      883 2022-03-07 12:56:12.000000 gxabm-2.4.0/abm/lib/folder.py
--rw-r--r--   0 suderman   (502) staff       (20)     4185 2022-10-27 02:48:01.000000 gxabm-2.4.0/abm/lib/helm.py
--rw-r--r--   0 suderman   (502) staff       (20)      282 2022-03-07 12:56:12.000000 gxabm-2.4.0/abm/lib/histories.yml
--rw-r--r--   0 suderman   (502) staff       (20)    10348 2023-04-29 23:23:52.000000 gxabm-2.4.0/abm/lib/history.py
--rw-r--r--   0 suderman   (502) staff       (20)     3610 2023-04-29 23:23:52.000000 gxabm-2.4.0/abm/lib/job.py
--rw-r--r--   0 suderman   (502) staff       (20)     1264 2022-03-07 12:56:12.000000 gxabm-2.4.0/abm/lib/kubectl.py
--rw-r--r--   0 suderman   (502) staff       (20)     2518 2023-04-24 20:08:21.000000 gxabm-2.4.0/abm/lib/library.py
--rw-r--r--   0 suderman   (502) staff       (20)    11618 2023-04-29 23:23:52.000000 gxabm-2.4.0/abm/lib/menu.yml
--rw-r--r--   0 suderman   (502) staff       (20)     3480 2022-10-19 17:36:24.000000 gxabm-2.4.0/abm/lib/users.py
--rw-r--r--   0 suderman   (502) staff       (20)     7524 2023-04-29 23:23:52.000000 gxabm-2.4.0/abm/lib/workflow.py
-drwxr-xr-x   0 suderman   (502) staff       (20)        0 2023-04-29 23:25:16.543797 gxabm-2.4.0/gxabm.egg-info/
--rw-r--r--   0 suderman   (502) staff       (20)    19487 2023-04-29 23:25:16.000000 gxabm-2.4.0/gxabm.egg-info/PKG-INFO
--rw-r--r--   0 suderman   (502) staff       (20)      669 2023-04-29 23:25:16.000000 gxabm-2.4.0/gxabm.egg-info/SOURCES.txt
--rw-r--r--   0 suderman   (502) staff       (20)        1 2023-04-29 23:25:16.000000 gxabm-2.4.0/gxabm.egg-info/dependency_links.txt
--rw-r--r--   0 suderman   (502) staff       (20)       49 2023-04-29 23:25:16.000000 gxabm-2.4.0/gxabm.egg-info/entry_points.txt
--rw-r--r--   0 suderman   (502) staff       (20)       48 2023-04-29 23:25:16.000000 gxabm-2.4.0/gxabm.egg-info/requires.txt
--rw-r--r--   0 suderman   (502) staff       (20)        9 2023-04-29 23:25:16.000000 gxabm-2.4.0/gxabm.egg-info/top_level.txt
--rw-r--r--   0 suderman   (502) staff       (20)       38 2023-04-29 23:25:16.546102 gxabm-2.4.0/setup.cfg
--rw-r--r--   0 suderman   (502) staff       (20)     1036 2022-10-19 17:36:24.000000 gxabm-2.4.0/setup.py
-drwxr-xr-x   0 suderman   (502) staff       (20)        0 2023-04-29 23:25:16.545476 gxabm-2.4.0/test/
--rw-r--r--   0 suderman   (502) staff       (20)      147 2022-03-07 12:56:12.000000 gxabm-2.4.0/test/__init__.py
--rwxr-xr-x   0 suderman   (502) staff       (20)     8684 2022-12-23 17:29:52.000000 gxabm-2.4.0/test/check_tools.py
--rw-r--r--   0 suderman   (502) staff       (20)     2160 2022-10-27 04:03:53.000000 gxabm-2.4.0/test/metrics.py
--rw-r--r--   0 suderman   (502) staff       (20)      298 2022-03-07 12:56:12.000000 gxabm-2.4.0/test/test_environments.py
--rw-r--r--   0 suderman   (502) staff       (20)      272 2023-03-14 21:04:32.000000 gxabm-2.4.0/test/workflow.py
+drwxr-xr-x   0 suderman   (502) staff       (20)        0 2023-05-01 01:44:13.432145 gxabm-2.5.0/
+-rw-r--r--   0 suderman   (502) staff       (20)       42 2022-03-07 12:56:12.000000 gxabm-2.5.0/MANIFEST.in
+-rw-r--r--   0 suderman   (502) staff       (20)    19487 2023-05-01 01:44:13.431951 gxabm-2.5.0/PKG-INFO
+-rw-r--r--   0 suderman   (502) staff       (20)    16395 2022-03-22 19:06:33.000000 gxabm-2.5.0/README.md
+drwxr-xr-x   0 suderman   (502) staff       (20)        0 2023-05-01 01:44:13.421832 gxabm-2.5.0/abm/
+-rw-r--r--   0 suderman   (502) staff       (20)        5 2023-05-01 01:43:54.000000 gxabm-2.5.0/abm/VERSION
+-rw-r--r--   0 suderman   (502) staff       (20)      290 2022-03-07 12:56:12.000000 gxabm-2.5.0/abm/__init__.py
+-rw-r--r--   0 suderman   (502) staff       (20)     8374 2023-05-01 01:43:54.000000 gxabm-2.5.0/abm/__main__.py
+drwxr-xr-x   0 suderman   (502) staff       (20)        0 2023-05-01 01:44:13.429092 gxabm-2.5.0/abm/lib/
+-rw-r--r--   0 suderman   (502) staff       (20)      447 2022-03-07 12:56:12.000000 gxabm-2.5.0/abm/lib/__init__.py
+-rw-r--r--   0 suderman   (502) staff       (20)    18434 2023-04-27 20:18:52.000000 gxabm-2.5.0/abm/lib/benchmark.py
+-rw-r--r--   0 suderman   (502) staff       (20)     7812 2022-10-19 17:36:24.000000 gxabm-2.5.0/abm/lib/cloudlaunch.py
+-rw-r--r--   0 suderman   (502) staff       (20)     7552 2023-05-01 01:43:54.000000 gxabm-2.5.0/abm/lib/common.py
+-rw-r--r--   0 suderman   (502) staff       (20)     5433 2022-10-19 17:36:24.000000 gxabm-2.5.0/abm/lib/config.py
+-rw-r--r--   0 suderman   (502) staff       (20)     6483 2023-04-27 20:18:52.000000 gxabm-2.5.0/abm/lib/dataset.py
+-rw-r--r--   0 suderman   (502) staff       (20)     7661 2023-04-29 03:35:40.000000 gxabm-2.5.0/abm/lib/experiment.py
+-rw-r--r--   0 suderman   (502) staff       (20)      883 2022-03-07 12:56:12.000000 gxabm-2.5.0/abm/lib/folder.py
+-rw-r--r--   0 suderman   (502) staff       (20)     4185 2022-10-27 02:48:01.000000 gxabm-2.5.0/abm/lib/helm.py
+-rw-r--r--   0 suderman   (502) staff       (20)      282 2022-03-07 12:56:12.000000 gxabm-2.5.0/abm/lib/histories.yml
+-rw-r--r--   0 suderman   (502) staff       (20)    10348 2023-04-29 23:23:52.000000 gxabm-2.5.0/abm/lib/history.py
+-rw-r--r--   0 suderman   (502) staff       (20)     1217 2023-05-01 01:43:54.000000 gxabm-2.5.0/abm/lib/invocation.py
+-rw-r--r--   0 suderman   (502) staff       (20)     3610 2023-04-29 23:23:52.000000 gxabm-2.5.0/abm/lib/job.py
+-rw-r--r--   0 suderman   (502) staff       (20)     1264 2022-03-07 12:56:12.000000 gxabm-2.5.0/abm/lib/kubectl.py
+-rw-r--r--   0 suderman   (502) staff       (20)     2518 2023-04-24 20:08:21.000000 gxabm-2.5.0/abm/lib/library.py
+-rw-r--r--   0 suderman   (502) staff       (20)    12004 2023-05-01 01:43:54.000000 gxabm-2.5.0/abm/lib/menu.yml
+-rw-r--r--   0 suderman   (502) staff       (20)     3480 2022-10-19 17:36:24.000000 gxabm-2.5.0/abm/lib/users.py
+-rw-r--r--   0 suderman   (502) staff       (20)     7817 2023-05-01 01:43:54.000000 gxabm-2.5.0/abm/lib/workflow.py
+drwxr-xr-x   0 suderman   (502) staff       (20)        0 2023-05-01 01:44:13.430218 gxabm-2.5.0/gxabm.egg-info/
+-rw-r--r--   0 suderman   (502) staff       (20)    19487 2023-05-01 01:44:13.000000 gxabm-2.5.0/gxabm.egg-info/PKG-INFO
+-rw-r--r--   0 suderman   (502) staff       (20)      691 2023-05-01 01:44:13.000000 gxabm-2.5.0/gxabm.egg-info/SOURCES.txt
+-rw-r--r--   0 suderman   (502) staff       (20)        1 2023-05-01 01:44:13.000000 gxabm-2.5.0/gxabm.egg-info/dependency_links.txt
+-rw-r--r--   0 suderman   (502) staff       (20)       49 2023-05-01 01:44:13.000000 gxabm-2.5.0/gxabm.egg-info/entry_points.txt
+-rw-r--r--   0 suderman   (502) staff       (20)       48 2023-05-01 01:44:13.000000 gxabm-2.5.0/gxabm.egg-info/requires.txt
+-rw-r--r--   0 suderman   (502) staff       (20)        9 2023-05-01 01:44:13.000000 gxabm-2.5.0/gxabm.egg-info/top_level.txt
+-rw-r--r--   0 suderman   (502) staff       (20)       38 2023-05-01 01:44:13.432272 gxabm-2.5.0/setup.cfg
+-rw-r--r--   0 suderman   (502) staff       (20)     1036 2022-10-19 17:36:24.000000 gxabm-2.5.0/setup.py
+drwxr-xr-x   0 suderman   (502) staff       (20)        0 2023-05-01 01:44:13.431516 gxabm-2.5.0/test/
+-rw-r--r--   0 suderman   (502) staff       (20)      147 2022-03-07 12:56:12.000000 gxabm-2.5.0/test/__init__.py
+-rwxr-xr-x   0 suderman   (502) staff       (20)     8684 2022-12-23 17:29:52.000000 gxabm-2.5.0/test/check_tools.py
+-rw-r--r--   0 suderman   (502) staff       (20)     2160 2022-10-27 04:03:53.000000 gxabm-2.5.0/test/metrics.py
+-rw-r--r--   0 suderman   (502) staff       (20)      298 2022-03-07 12:56:12.000000 gxabm-2.5.0/test/test_environments.py
+-rw-r--r--   0 suderman   (502) staff       (20)      272 2023-03-14 21:04:32.000000 gxabm-2.5.0/test/workflow.py
```

### Comparing `gxabm-2.4.0/PKG-INFO` & `gxabm-2.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gxabm
-Version: 2.4.0
+Version: 2.5.0
 Summary: Opinionated Benchmarking Automatation in Galaxy
 Home-page: https://github.com/galaxyproject/gxabm
 Author: Keith Suderman
 Author-email: suderman@jhu.edu
 License: MIT
 Description: # Automated Benchmarking in Galaxy
         An opinionated Python Bioblend script for automating benchmarking tasks in Galaxy.
```

### Comparing `gxabm-2.4.0/README.md` & `gxabm-2.5.0/README.md`

 * *Files identical despite different names*

### Comparing `gxabm-2.4.0/abm/__main__.py` & `gxabm-2.5.0/abm/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 import logging
 from lib.common import Context
 from pprint import pprint
 from abm import getVersion
 
 # These imports are required because we need Python to be load them to the
 # symbol table so the parse_menu method can find them in globals()
-from lib import job, dataset, workflow, history, library, folder, benchmark, helm, kubectl, config, experiment, users, cloudlaunch
+from lib import job, dataset, workflow, history, library, folder, benchmark, helm, kubectl, config, experiment, users, cloudlaunch, invocation
 
 log = logging.getLogger('abm')
 handler = logging.StreamHandler()
 formatter = logging.Formatter('%(asctime)s - %(levelname)s - %(message)s')
 
 log.setLevel(logging.ERROR)
 handler.setLevel(logging.ERROR)
```

### Comparing `gxabm-2.4.0/abm/lib/benchmark.py` & `gxabm-2.5.0/abm/lib/benchmark.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.4.0/abm/lib/cloudlaunch.py` & `gxabm-2.5.0/abm/lib/cloudlaunch.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.4.0/abm/lib/common.py` & `gxabm-2.5.0/abm/lib/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -196,20 +196,20 @@
     "workflow_id",
     "cpuacct.usage",
     # "end_epoch",
     "galaxy_memory_mb",
     "galaxy_slots",
     # "memory.failcnt",
     "memory.limit_in_bytes",
-    # "memory.max_usage_in_bytes",
+    "memory.max_usage_in_bytes",
     # "memory.memsw.limit_in_bytes",
     # "memory.memsw.max_usage_in_bytes",
     # "memory.oom_control.oom_kill_disable",
     # "memory.oom_control.under_oom",
-    # "memory.soft_limit_in_bytes",
+    "memory.soft_limit_in_bytes",
     "memtotal",
     "processor_count",
     "runtime_seconds",
     # "start_epoch",
     # "swaptotal",
     # "uname"
     ]
```

### Comparing `gxabm-2.4.0/abm/lib/config.py` & `gxabm-2.5.0/abm/lib/config.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.4.0/abm/lib/dataset.py` & `gxabm-2.5.0/abm/lib/dataset.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.4.0/abm/lib/experiment.py` & `gxabm-2.5.0/abm/lib/experiment.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.4.0/abm/lib/folder.py` & `gxabm-2.5.0/abm/lib/folder.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.4.0/abm/lib/helm.py` & `gxabm-2.5.0/abm/lib/helm.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.4.0/abm/lib/history.py` & `gxabm-2.5.0/abm/lib/history.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.4.0/abm/lib/job.py` & `gxabm-2.5.0/abm/lib/job.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.4.0/abm/lib/kubectl.py` & `gxabm-2.5.0/abm/lib/kubectl.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.4.0/abm/lib/library.py` & `gxabm-2.5.0/abm/lib/library.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.4.0/abm/lib/menu.yml` & `gxabm-2.5.0/abm/lib/menu.yml`

 * *Files 2% similar despite different names*

```diff
@@ -239,14 +239,25 @@
       help: summarize metrics to a CSV or TSV file.
       handler: experiment.summarize
       params: "[-c, --csv, -t, --tsv]"
     - name: [test]
       help: playground code
       handler: experiment.test
       params: [VARIES]
+- name: [invocation, inv, invocations]
+  help: get information about job and workflow invocations
+  menu:
+    - name: [list, ls]
+      help: list all invocations.
+      handler: invocation.doList
+      params: "[-w|--workflow ID] [-h|--history ID]"
+    - name: [summarize]
+      help: generate a CSV of job metrics for an invocation
+      params: ID
+      handler: invocation.summarize
 - name: [helm]
   help: execute a helm command
   menu:
     - name: [update, upgrade, up]
       help: update the container mapper rules for memory and cpu limits
       handler: helm.update_cli
       params: RULES
```

### Comparing `gxabm-2.4.0/abm/lib/users.py` & `gxabm-2.5.0/abm/lib/users.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.4.0/abm/lib/workflow.py` & `gxabm-2.5.0/abm/lib/workflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -178,16 +178,23 @@
         print("ERROR: No workflow ID provided")
         return
     # if invocation_id is None:
     #     print("ERROR: No invocation ID provided")
     #     return
     gi = connect(context)
     # result = gi.workflows.show_invocation(workflow_id, invocation_id)
-    result = gi.invocations.get_invocations(workflow_id=workflow_id, view='element', step_details=True)
-    print(json.dumps(result, indent=4))
+    invocations = gi.invocations.get_invocations(workflow_id=workflow_id, view='element', step_details=True)
+    # print(json.dumps(result, indent=4))
+    print('ID\tState\tWorkflow\tHistory')
+    for invocation in invocations:
+        id = invocation['id']
+        state = invocation['state']
+        workflow = invocation['workflow_id']
+        history = invocation['history_id']
+        print(f'{id}\t{state}\t{workflow}\t{history}')
 
 
 def find(context: Context, args: list):
     if len(args) == 0:
         print("ERROR: no workflow name given")
         return
     gi = connect(context)
```

### Comparing `gxabm-2.4.0/gxabm.egg-info/PKG-INFO` & `gxabm-2.5.0/gxabm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gxabm
-Version: 2.4.0
+Version: 2.5.0
 Summary: Opinionated Benchmarking Automatation in Galaxy
 Home-page: https://github.com/galaxyproject/gxabm
 Author: Keith Suderman
 Author-email: suderman@jhu.edu
 License: MIT
 Description: # Automated Benchmarking in Galaxy
         An opinionated Python Bioblend script for automating benchmarking tasks in Galaxy.
```

### Comparing `gxabm-2.4.0/gxabm.egg-info/SOURCES.txt` & `gxabm-2.5.0/gxabm.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 abm/lib/config.py
 abm/lib/dataset.py
 abm/lib/experiment.py
 abm/lib/folder.py
 abm/lib/helm.py
 abm/lib/histories.yml
 abm/lib/history.py
+abm/lib/invocation.py
 abm/lib/job.py
 abm/lib/kubectl.py
 abm/lib/library.py
 abm/lib/menu.yml
 abm/lib/users.py
 abm/lib/workflow.py
 gxabm.egg-info/PKG-INFO
```

### Comparing `gxabm-2.4.0/setup.py` & `gxabm-2.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.4.0/test/check_tools.py` & `gxabm-2.5.0/test/check_tools.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.4.0/test/metrics.py` & `gxabm-2.5.0/test/metrics.py`

 * *Files identical despite different names*

