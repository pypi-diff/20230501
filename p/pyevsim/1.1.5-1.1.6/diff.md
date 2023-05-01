# Comparing `tmp/pyevsim-1.1.5.tar.gz` & `tmp/pyevsim-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyevsim-1.1.5.tar", last modified: Sun Apr  9 09:11:01 2023, max compression
+gzip compressed data, was "pyevsim-1.1.6.tar", last modified: Mon May  1 17:01:42 2023, max compression
```

## Comparing `pyevsim-1.1.5.tar` & `pyevsim-1.1.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-04-09 09:11:01.382464 pyevsim-1.1.5/
--rw-rw-rw-   0        0        0     1091 2022-08-27 18:53:45.000000 pyevsim-1.1.5/LICENSE
--rw-rw-rw-   0        0        0      541 2023-04-09 09:11:01.382464 pyevsim-1.1.5/PKG-INFO
--rw-rw-rw-   0        0        0       58 2022-08-27 18:53:45.000000 pyevsim-1.1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-09 09:11:01.365463 pyevsim-1.1.5/pyevsim/
--rw-rw-rw-   0        0        0     1950 2022-08-27 18:53:45.000000 pyevsim-1.1.5/pyevsim/__init__.py
--rw-rw-rw-   0        0        0     3656 2023-04-09 08:46:51.000000 pyevsim-1.1.5/pyevsim/behavior_model.py
--rw-rw-rw-   0        0        0     2477 2022-08-27 18:53:45.000000 pyevsim-1.1.5/pyevsim/behavior_model_executor.py
--rw-rw-rw-   0        0        0      603 2022-08-27 18:53:45.000000 pyevsim-1.1.5/pyevsim/default_message_catcher.py
--rw-rw-rw-   0        0        0     2496 2023-04-09 08:46:51.000000 pyevsim-1.1.5/pyevsim/definition.py
--rw-rw-rw-   0        0        0     5884 2023-04-09 09:06:40.000000 pyevsim-1.1.5/pyevsim/gen.py
--rw-rw-rw-   0        0        0     1796 2022-08-27 18:53:45.000000 pyevsim-1.1.5/pyevsim/structural_model.py
--rw-rw-rw-   0        0        0    14720 2023-04-09 08:46:51.000000 pyevsim-1.1.5/pyevsim/system_executor.py
--rw-rw-rw-   0        0        0      842 2022-08-27 18:53:45.000000 pyevsim-1.1.5/pyevsim/system_message.py
--rw-rw-rw-   0        0        0      726 2022-08-27 18:53:45.000000 pyevsim-1.1.5/pyevsim/system_object.py
--rw-rw-rw-   0        0        0     1524 2023-04-09 08:46:51.000000 pyevsim-1.1.5/pyevsim/system_simulator.py
--rw-rw-rw-   0        0        0      524 2022-08-27 18:53:45.000000 pyevsim-1.1.5/pyevsim/termination_manager.py
-drwxrwxrwx   0        0        0        0 2023-04-09 09:11:01.380463 pyevsim-1.1.5/pyevsim.egg-info/
--rw-rw-rw-   0        0        0      541 2023-04-09 09:11:01.000000 pyevsim-1.1.5/pyevsim.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      468 2023-04-09 09:11:01.000000 pyevsim-1.1.5/pyevsim.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-09 09:11:01.000000 pyevsim-1.1.5/pyevsim.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-04-09 09:11:01.000000 pyevsim-1.1.5/pyevsim.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-09 09:11:01.382464 pyevsim-1.1.5/setup.cfg
--rw-rw-rw-   0        0        0      596 2023-04-09 08:57:52.000000 pyevsim-1.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 17:01:42.289058 pyevsim-1.1.6/
+-rw-rw-rw-   0        0        0     1091 2022-08-27 18:53:45.000000 pyevsim-1.1.6/LICENSE
+-rw-rw-rw-   0        0        0      541 2023-05-01 17:01:42.288056 pyevsim-1.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0       58 2022-08-27 18:53:45.000000 pyevsim-1.1.6/README.md
+drwxrwxrwx   0        0        0        0 2023-05-01 17:01:42.276055 pyevsim-1.1.6/pyevsim/
+-rw-rw-rw-   0        0        0     1950 2022-08-27 18:53:45.000000 pyevsim-1.1.6/pyevsim/__init__.py
+-rw-rw-rw-   0        0        0     3656 2023-04-09 08:46:51.000000 pyevsim-1.1.6/pyevsim/behavior_model.py
+-rw-rw-rw-   0        0        0     2477 2022-08-27 18:53:45.000000 pyevsim-1.1.6/pyevsim/behavior_model_executor.py
+-rw-rw-rw-   0        0        0      603 2022-08-27 18:53:45.000000 pyevsim-1.1.6/pyevsim/default_message_catcher.py
+-rw-rw-rw-   0        0        0     2496 2023-04-09 08:46:51.000000 pyevsim-1.1.6/pyevsim/definition.py
+-rw-rw-rw-   0        0        0     5922 2023-05-01 17:00:28.000000 pyevsim-1.1.6/pyevsim/gen.py
+-rw-rw-rw-   0        0        0     1796 2022-08-27 18:53:45.000000 pyevsim-1.1.6/pyevsim/structural_model.py
+-rw-rw-rw-   0        0        0    14720 2023-04-09 08:46:51.000000 pyevsim-1.1.6/pyevsim/system_executor.py
+-rw-rw-rw-   0        0        0      842 2022-08-27 18:53:45.000000 pyevsim-1.1.6/pyevsim/system_message.py
+-rw-rw-rw-   0        0        0      726 2022-08-27 18:53:45.000000 pyevsim-1.1.6/pyevsim/system_object.py
+-rw-rw-rw-   0        0        0     1524 2023-04-09 08:46:51.000000 pyevsim-1.1.6/pyevsim/system_simulator.py
+-rw-rw-rw-   0        0        0      524 2022-08-27 18:53:45.000000 pyevsim-1.1.6/pyevsim/termination_manager.py
+drwxrwxrwx   0        0        0        0 2023-05-01 17:01:42.287057 pyevsim-1.1.6/pyevsim.egg-info/
+-rw-rw-rw-   0        0        0      541 2023-05-01 17:01:42.000000 pyevsim-1.1.6/pyevsim.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      468 2023-05-01 17:01:42.000000 pyevsim-1.1.6/pyevsim.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 17:01:42.000000 pyevsim-1.1.6/pyevsim.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-01 17:01:42.000000 pyevsim-1.1.6/pyevsim.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-01 17:01:42.289058 pyevsim-1.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      596 2023-05-01 17:00:28.000000 pyevsim-1.1.6/setup.py
```

### Comparing `pyevsim-1.1.5/LICENSE` & `pyevsim-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyevsim-1.1.5/PKG-INFO` & `pyevsim-1.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pyevsim
-Version: 1.1.5
+Version: 1.1.6
 Summary: A library that provides a Modeling & Simulation Environment for Discrete Event System Formalism
 Home-page: https://github.com/eventsim/pyevsim
 Author: Changbeom Choi
 Author-email: me@cbchoi.info
 License: MIT
 Description: # evsim
         Discrete Event Simulation Engine using Python
```

### Comparing `pyevsim-1.1.5/pyevsim/__init__.py` & `pyevsim-1.1.6/pyevsim/__init__.py`

 * *Files identical despite different names*

### Comparing `pyevsim-1.1.5/pyevsim/behavior_model.py` & `pyevsim-1.1.6/pyevsim/behavior_model.py`

 * *Files identical despite different names*

### Comparing `pyevsim-1.1.5/pyevsim/behavior_model_executor.py` & `pyevsim-1.1.6/pyevsim/behavior_model_executor.py`

 * *Files identical despite different names*

### Comparing `pyevsim-1.1.5/pyevsim/default_message_catcher.py` & `pyevsim-1.1.6/pyevsim/default_message_catcher.py`

 * *Files identical despite different names*

### Comparing `pyevsim-1.1.5/pyevsim/definition.py` & `pyevsim-1.1.6/pyevsim/definition.py`

 * *Files identical despite different names*

### Comparing `pyevsim-1.1.5/pyevsim/gen.py` & `pyevsim-1.1.6/pyevsim/gen.py`

 * *Files 0% similar despite different names*

```diff
@@ -155,22 +155,23 @@
 
 types of example:
    periodic:\t Prints event log periodically
    relay: \t A model sends a output event and other model receives the event
    multi: \t Mupltiple simulation engine interacts with each other
 """
 import sys
-
-if sys.argv[1] == "relay":
+if len(sys.argv) != 2:
+    print(usage)
+elif sys.argv[1] == "relay":
     f = open("example_replay.py", "w")
     f.write(relay_example)
     pass
 elif sys.argv[1] == "multi":
     f = open("example_multi_thread.py", "w")
     f.write(multi_example)
     pass
 elif sys.argv[1] == "periodic":
-    f = open("example_multi_thread.py", "w")
+    f = open("example_periodic.py", "w")
     f.write(periodic_example)
     pass
 else:
     print(usage)
```

### Comparing `pyevsim-1.1.5/pyevsim/structural_model.py` & `pyevsim-1.1.6/pyevsim/structural_model.py`

 * *Files identical despite different names*

### Comparing `pyevsim-1.1.5/pyevsim/system_executor.py` & `pyevsim-1.1.6/pyevsim/system_executor.py`

 * *Files identical despite different names*

### Comparing `pyevsim-1.1.5/pyevsim/system_message.py` & `pyevsim-1.1.6/pyevsim/system_message.py`

 * *Files identical despite different names*

### Comparing `pyevsim-1.1.5/pyevsim/system_object.py` & `pyevsim-1.1.6/pyevsim/system_object.py`

 * *Files identical despite different names*

### Comparing `pyevsim-1.1.5/pyevsim/system_simulator.py` & `pyevsim-1.1.6/pyevsim/system_simulator.py`

 * *Files identical despite different names*

### Comparing `pyevsim-1.1.5/pyevsim/termination_manager.py` & `pyevsim-1.1.6/pyevsim/termination_manager.py`

 * *Files identical despite different names*

### Comparing `pyevsim-1.1.5/pyevsim.egg-info/PKG-INFO` & `pyevsim-1.1.6/pyevsim.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pyevsim
-Version: 1.1.5
+Version: 1.1.6
 Summary: A library that provides a Modeling & Simulation Environment for Discrete Event System Formalism
 Home-page: https://github.com/eventsim/pyevsim
 Author: Changbeom Choi
 Author-email: me@cbchoi.info
 License: MIT
 Description: # evsim
         Discrete Event Simulation Engine using Python
```

### Comparing `pyevsim-1.1.5/setup.py` & `pyevsim-1.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="pyevsim",
-    version="1.1.5",
+    version="1.1.6",
     license='MIT',
     author="Changbeom Choi",
     author_email="me@cbchoi.info",
     description="A library that provides a Modeling & Simulation Environment for Discrete Event System Formalism",
     long_description=open('README.md').read(),
     url="https://github.com/eventsim/pyevsim",
     packages=setuptools.find_packages(),
```

