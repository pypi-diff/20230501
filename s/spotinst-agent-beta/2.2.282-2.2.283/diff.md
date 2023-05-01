# Comparing `tmp/spotinst-agent-beta-2.2.282.tar.gz` & `tmp/spotinst-agent-beta-2.2.283.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotinst-agent-beta-2.2.282.tar", last modified: Sun Apr 30 13:42:03 2023, max compression
+gzip compressed data, was "spotinst-agent-beta-2.2.283.tar", last modified: Mon May  1 09:17:50 2023, max compression
```

## Comparing `spotinst-agent-beta-2.2.282.tar` & `spotinst-agent-beta-2.2.283.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-30 13:42:03.600473 spotinst-agent-beta-2.2.282/
--rw-r--r--   0 ayeletc    (502) staff       (20)     1065 2023-03-12 08:32:58.000000 spotinst-agent-beta-2.2.282/LICENSE
--rw-r--r--   0 ayeletc    (502) staff       (20)      181 2023-03-12 08:32:58.000000 spotinst-agent-beta-2.2.282/MANIFEST.in
--rw-r--r--   0 ayeletc    (502) staff       (20)     1940 2023-04-30 13:42:03.600281 spotinst-agent-beta-2.2.282/PKG-INFO
--rw-r--r--   0 ayeletc    (502) staff       (20)     1287 2023-03-12 08:32:58.000000 spotinst-agent-beta-2.2.282/README.rst
--rw-r--r--   0 ayeletc    (502) staff       (20)       38 2023-04-30 13:42:03.600529 spotinst-agent-beta-2.2.282/setup.cfg
--rw-r--r--   0 ayeletc    (502) staff       (20)     1392 2023-04-30 13:42:01.000000 spotinst-agent-beta-2.2.282/setup.py
-drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-30 13:42:03.598104 spotinst-agent-beta-2.2.282/spotinst_agent/
--rw-r--r--   0 ayeletc    (502) staff       (20)    13173 2023-04-30 12:55:13.000000 spotinst-agent-beta-2.2.282/spotinst_agent/__init__.py
--rw-r--r--   0 ayeletc    (502) staff       (20)     3116 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.282/spotinst_agent/agent.py
--rw-r--r--   0 ayeletc    (502) staff       (20)     9604 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.282/spotinst_agent/agentinit.py
--rw-r--r--   0 ayeletc    (502) staff       (20)     1129 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.282/spotinst_agent/basemodule.py
-drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-30 13:42:03.594657 spotinst-agent-beta-2.2.282/spotinst_agent/data/
-drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-30 13:42:03.598520 spotinst-agent-beta-2.2.282/spotinst_agent/data/configuration/
--rw-r--r--   0 ayeletc    (502) staff       (20)      180 2023-03-12 08:32:58.000000 spotinst-agent-beta-2.2.282/spotinst_agent/data/configuration/basemodule.yml
--rw-r--r--   0 ayeletc    (502) staff       (20)      727 2023-04-27 08:56:57.000000 spotinst-agent-beta-2.2.282/spotinst_agent/data/configuration/spotinst-agent.yml
-drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-30 13:42:03.598734 spotinst-agent-beta-2.2.282/spotinst_agent/data/installation/
--rwxr-xr-x   0 ayeletc    (502) staff       (20)     6691 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.282/spotinst_agent/data/installation/agent-init.sh
--rw-r--r--   0 ayeletc    (502) staff       (20)    21605 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.282/spotinst_agent/scheduler.py
--rw-r--r--   0 ayeletc    (502) staff       (20)    10922 2023-04-30 13:13:26.000000 spotinst-agent-beta-2.2.282/spotinst_agent/taskmanager.py
--rw-r--r--   0 ayeletc    (502) staff       (20)     9420 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.282/spotinst_agent/utils.py
-drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-30 13:42:03.600018 spotinst-agent-beta-2.2.282/spotinst_agent_beta.egg-info/
--rw-r--r--   0 ayeletc    (502) staff       (20)     1940 2023-04-30 13:42:03.000000 spotinst-agent-beta-2.2.282/spotinst_agent_beta.egg-info/PKG-INFO
--rw-r--r--   0 ayeletc    (502) staff       (20)      638 2023-04-30 13:42:03.000000 spotinst-agent-beta-2.2.282/spotinst_agent_beta.egg-info/SOURCES.txt
--rw-r--r--   0 ayeletc    (502) staff       (20)        1 2023-04-30 13:42:03.000000 spotinst-agent-beta-2.2.282/spotinst_agent_beta.egg-info/dependency_links.txt
--rw-r--r--   0 ayeletc    (502) staff       (20)       55 2023-04-30 13:42:03.000000 spotinst-agent-beta-2.2.282/spotinst_agent_beta.egg-info/entry_points.txt
--rw-r--r--   0 ayeletc    (502) staff       (20)       16 2023-04-30 13:42:03.000000 spotinst-agent-beta-2.2.282/spotinst_agent_beta.egg-info/requires.txt
--rw-r--r--   0 ayeletc    (502) staff       (20)       15 2023-04-30 13:42:03.000000 spotinst-agent-beta-2.2.282/spotinst_agent_beta.egg-info/top_level.txt
+drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-05-01 09:17:50.087512 spotinst-agent-beta-2.2.283/
+-rw-r--r--   0 ayeletc    (502) staff       (20)     1065 2023-03-12 08:32:58.000000 spotinst-agent-beta-2.2.283/LICENSE
+-rw-r--r--   0 ayeletc    (502) staff       (20)      181 2023-03-12 08:32:58.000000 spotinst-agent-beta-2.2.283/MANIFEST.in
+-rw-r--r--   0 ayeletc    (502) staff       (20)     1940 2023-05-01 09:17:50.087328 spotinst-agent-beta-2.2.283/PKG-INFO
+-rw-r--r--   0 ayeletc    (502) staff       (20)     1287 2023-03-12 08:32:58.000000 spotinst-agent-beta-2.2.283/README.rst
+-rw-r--r--   0 ayeletc    (502) staff       (20)       38 2023-05-01 09:17:50.087558 spotinst-agent-beta-2.2.283/setup.cfg
+-rw-r--r--   0 ayeletc    (502) staff       (20)     1392 2023-05-01 09:17:45.000000 spotinst-agent-beta-2.2.283/setup.py
+drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-05-01 09:17:50.079723 spotinst-agent-beta-2.2.283/spotinst_agent/
+-rw-r--r--   0 ayeletc    (502) staff       (20)    13173 2023-04-30 12:55:13.000000 spotinst-agent-beta-2.2.283/spotinst_agent/__init__.py
+-rw-r--r--   0 ayeletc    (502) staff       (20)     3116 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.283/spotinst_agent/agent.py
+-rw-r--r--   0 ayeletc    (502) staff       (20)     9604 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.283/spotinst_agent/agentinit.py
+-rw-r--r--   0 ayeletc    (502) staff       (20)     1129 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.283/spotinst_agent/basemodule.py
+drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-05-01 09:17:50.070591 spotinst-agent-beta-2.2.283/spotinst_agent/data/
+drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-05-01 09:17:50.081147 spotinst-agent-beta-2.2.283/spotinst_agent/data/configuration/
+-rw-r--r--   0 ayeletc    (502) staff       (20)      180 2023-03-12 08:32:58.000000 spotinst-agent-beta-2.2.283/spotinst_agent/data/configuration/basemodule.yml
+-rw-r--r--   0 ayeletc    (502) staff       (20)      727 2023-04-27 08:56:57.000000 spotinst-agent-beta-2.2.283/spotinst_agent/data/configuration/spotinst-agent.yml
+drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-05-01 09:17:50.081521 spotinst-agent-beta-2.2.283/spotinst_agent/data/installation/
+-rwxr-xr-x   0 ayeletc    (502) staff       (20)     6691 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.283/spotinst_agent/data/installation/agent-init.sh
+-rw-r--r--   0 ayeletc    (502) staff       (20)    21605 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.283/spotinst_agent/scheduler.py
+-rw-r--r--   0 ayeletc    (502) staff       (20)    10922 2023-05-01 09:17:32.000000 spotinst-agent-beta-2.2.283/spotinst_agent/taskmanager.py
+-rw-r--r--   0 ayeletc    (502) staff       (20)     9420 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.283/spotinst_agent/utils.py
+drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-05-01 09:17:50.086925 spotinst-agent-beta-2.2.283/spotinst_agent_beta.egg-info/
+-rw-r--r--   0 ayeletc    (502) staff       (20)     1940 2023-05-01 09:17:50.000000 spotinst-agent-beta-2.2.283/spotinst_agent_beta.egg-info/PKG-INFO
+-rw-r--r--   0 ayeletc    (502) staff       (20)      638 2023-05-01 09:17:50.000000 spotinst-agent-beta-2.2.283/spotinst_agent_beta.egg-info/SOURCES.txt
+-rw-r--r--   0 ayeletc    (502) staff       (20)        1 2023-05-01 09:17:50.000000 spotinst-agent-beta-2.2.283/spotinst_agent_beta.egg-info/dependency_links.txt
+-rw-r--r--   0 ayeletc    (502) staff       (20)       55 2023-05-01 09:17:50.000000 spotinst-agent-beta-2.2.283/spotinst_agent_beta.egg-info/entry_points.txt
+-rw-r--r--   0 ayeletc    (502) staff       (20)       16 2023-05-01 09:17:50.000000 spotinst-agent-beta-2.2.283/spotinst_agent_beta.egg-info/requires.txt
+-rw-r--r--   0 ayeletc    (502) staff       (20)       15 2023-05-01 09:17:50.000000 spotinst-agent-beta-2.2.283/spotinst_agent_beta.egg-info/top_level.txt
```

### Comparing `spotinst-agent-beta-2.2.282/LICENSE` & `spotinst-agent-beta-2.2.283/LICENSE`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.282/PKG-INFO` & `spotinst-agent-beta-2.2.283/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotinst-agent-beta
-Version: 2.2.282
+Version: 2.2.283
 Summary: Spectrum instance spotinst-agent that is able to run remote scripts, collect data, deploy applications and more.
 Home-page: https://github.com/spotinst/spotinst-spectrum-agent
 Author: Spotinst
 Author-email: service@spotinst.com
 License: MIT
 Keywords: spotinst agent infrastructure monitoring execution deployment
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `spotinst-agent-beta-2.2.282/README.rst` & `spotinst-agent-beta-2.2.283/README.rst`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.282/setup.py` & `spotinst-agent-beta-2.2.283/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # Get the long description from the README file
 with open(path.join(here, 'README.rst'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='spotinst-agent-beta',
 
-    version="2.2.282",
+    version="2.2.283",
 
     description='Spectrum instance spotinst-agent that is able to run remote scripts, collect data, deploy applications and more.',
 
     long_description=description,
 
     # The project's main homepage.
     url='https://github.com/spotinst/spotinst-spectrum-agent',
```

### Comparing `spotinst-agent-beta-2.2.282/spotinst_agent/__init__.py` & `spotinst-agent-beta-2.2.283/spotinst_agent/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.282/spotinst_agent/agent.py` & `spotinst-agent-beta-2.2.283/spotinst_agent/agent.py`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.282/spotinst_agent/agentinit.py` & `spotinst-agent-beta-2.2.283/spotinst_agent/agentinit.py`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.282/spotinst_agent/basemodule.py` & `spotinst-agent-beta-2.2.283/spotinst_agent/basemodule.py`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.282/spotinst_agent/data/configuration/spotinst-agent.yml` & `spotinst-agent-beta-2.2.283/spotinst_agent/data/configuration/spotinst-agent.yml`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.282/spotinst_agent/data/installation/agent-init.sh` & `spotinst-agent-beta-2.2.283/spotinst_agent/data/installation/agent-init.sh`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.282/spotinst_agent/scheduler.py` & `spotinst-agent-beta-2.2.283/spotinst_agent/scheduler.py`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.282/spotinst_agent/taskmanager.py` & `spotinst-agent-beta-2.2.283/spotinst_agent/taskmanager.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         self.reload_interval = reload_interval
         self.scheduler = ThreadedScheduler()
         self.running = True
         self.tasks = {}
         self.instance_details = instance_details
 
     def start(self):
-        time.sleep(20)
+        time.sleep(45)
         initiators_folder = '/etc/spotinst/agent/initiators/modules'
         self.log.debug("service is %s" % self.enable)
 
         # Search for initiators in folder
         initiators = self.load_modules(initiators_folder)
 
         # Setup Modules
```

### Comparing `spotinst-agent-beta-2.2.282/spotinst_agent/utils.py` & `spotinst-agent-beta-2.2.283/spotinst_agent/utils.py`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.282/spotinst_agent_beta.egg-info/PKG-INFO` & `spotinst-agent-beta-2.2.283/spotinst_agent_beta.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotinst-agent-beta
-Version: 2.2.282
+Version: 2.2.283
 Summary: Spectrum instance spotinst-agent that is able to run remote scripts, collect data, deploy applications and more.
 Home-page: https://github.com/spotinst/spotinst-spectrum-agent
 Author: Spotinst
 Author-email: service@spotinst.com
 License: MIT
 Keywords: spotinst agent infrastructure monitoring execution deployment
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `spotinst-agent-beta-2.2.282/spotinst_agent_beta.egg-info/SOURCES.txt` & `spotinst-agent-beta-2.2.283/spotinst_agent_beta.egg-info/SOURCES.txt`

 * *Files identical despite different names*

