# Comparing `tmp/coppyr-0.9.2.tar.gz` & `tmp/coppyr-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coppyr-0.9.2.tar", last modified: Fri Apr 28 16:52:27 2023, max compression
+gzip compressed data, was "coppyr-0.9.3.tar", last modified: Mon May  1 18:02:45 2023, max compression
```

## Comparing `coppyr-0.9.2.tar` & `coppyr-0.9.3.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 16:52:27.066432 coppyr-0.9.2/
--rw-rw-r--   0 root         (0) root         (0)     1072 2023-04-24 19:48:14.000000 coppyr-0.9.2/LICENSE
--rw-rw-r--   0 root         (0) root         (0)       83 2023-04-24 21:42:08.000000 coppyr-0.9.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4983 2023-04-28 16:52:27.066432 coppyr-0.9.2/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     4266 2023-04-24 21:55:15.000000 coppyr-0.9.2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 16:52:27.062432 coppyr-0.9.2/coppyr/
--rw-rw-r--   0 root         (0) root         (0)      437 2023-04-28 16:48:36.000000 coppyr-0.9.2/coppyr/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 16:52:27.062432 coppyr-0.9.2/coppyr/collections/
--rw-rw-r--   0 root         (0) root         (0)       78 2023-04-24 19:49:53.000000 coppyr-0.9.2/coppyr/collections/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1091 2023-04-24 19:49:53.000000 coppyr-0.9.2/coppyr/collections/cycle.py
--rw-rw-r--   0 root         (0) root         (0)      856 2023-04-28 16:36:15.000000 coppyr-0.9.2/coppyr/collections/dotdict.py
--rw-rw-r--   0 root         (0) root         (0)     1871 2023-04-28 16:28:29.000000 coppyr-0.9.2/coppyr/config.py
--rw-rw-r--   0 root         (0) root         (0)     4319 2023-04-28 16:07:28.000000 coppyr-0.9.2/coppyr/context.py
--rw-rw-r--   0 root         (0) root         (0)     2316 2023-04-24 19:56:41.000000 coppyr-0.9.2/coppyr/daemon.py
--rw-rw-r--   0 root         (0) root         (0)     1645 2023-04-24 19:57:04.000000 coppyr-0.9.2/coppyr/error.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 16:52:27.062432 coppyr-0.9.2/coppyr/extensions/
--rw-rw-r--   0 root         (0) root         (0)       24 2023-04-24 19:49:53.000000 coppyr-0.9.2/coppyr/extensions/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     3152 2023-04-24 20:41:07.000000 coppyr-0.9.2/coppyr/extensions/load.py
--rw-rw-r--   0 root         (0) root         (0)     4735 2023-04-24 19:57:57.000000 coppyr-0.9.2/coppyr/logger.py
--rw-rw-r--   0 root         (0) root         (0)     2428 2023-04-25 15:19:57.000000 coppyr-0.9.2/coppyr/package.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 16:52:27.066432 coppyr-0.9.2/coppyr/process/
--rw-rw-r--   0 root         (0) root         (0)       24 2023-04-27 19:30:48.000000 coppyr-0.9.2/coppyr/process/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1431 2023-04-24 19:55:39.000000 coppyr-0.9.2/coppyr/process/concurrent.py
--rw-rw-r--   0 root         (0) root         (0)    10912 2023-04-24 19:58:31.000000 coppyr-0.9.2/coppyr/process/parallel.py
--rw-rw-r--   0 root         (0) root         (0)     3482 2023-04-24 19:59:29.000000 coppyr-0.9.2/coppyr/process/subp.py
--rw-rw-r--   0 root         (0) root         (0)      389 2023-04-24 19:49:53.000000 coppyr-0.9.2/coppyr/testing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 16:52:27.066432 coppyr-0.9.2/coppyr/types/
--rw-rw-r--   0 root         (0) root         (0)      179 2023-04-27 21:29:25.000000 coppyr-0.9.2/coppyr/types/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     3569 2023-04-27 23:05:32.000000 coppyr-0.9.2/coppyr/types/differ.py
--rw-rw-r--   0 root         (0) root         (0)      351 2023-04-24 19:49:53.000000 coppyr-0.9.2/coppyr/types/lazyproperty.py
--rw-rw-r--   0 root         (0) root         (0)     1187 2023-04-27 19:30:58.000000 coppyr-0.9.2/coppyr/types/singleton.py
--rw-rw-r--   0 root         (0) root         (0)      763 2023-04-27 19:56:36.000000 coppyr-0.9.2/coppyr/types/slot.py
--rw-rw-r--   0 root         (0) root         (0)     1028 2023-04-24 20:44:01.000000 coppyr-0.9.2/coppyr/web.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 16:52:27.062432 coppyr-0.9.2/coppyr.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4983 2023-04-28 16:52:27.000000 coppyr-0.9.2/coppyr.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      732 2023-04-28 16:52:27.000000 coppyr-0.9.2/coppyr.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 16:52:27.000000 coppyr-0.9.2/coppyr.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      166 2023-04-28 16:52:27.000000 coppyr-0.9.2/coppyr.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-04-28 16:52:27.000000 coppyr-0.9.2/coppyr.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)       80 2023-04-25 15:25:17.000000 coppyr-0.9.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-28 16:52:27.066432 coppyr-0.9.2/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1285 2023-04-25 15:26:56.000000 coppyr-0.9.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 18:02:45.258540 coppyr-0.9.3/
+-rw-rw-r--   0 root         (0) root         (0)     1072 2023-04-24 19:48:14.000000 coppyr-0.9.3/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)       58 2023-04-28 19:06:54.000000 coppyr-0.9.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4983 2023-05-01 18:02:45.258540 coppyr-0.9.3/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     4266 2023-04-24 21:55:15.000000 coppyr-0.9.3/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 18:02:45.254540 coppyr-0.9.3/coppyr/
+-rw-rw-r--   0 root         (0) root         (0)      437 2023-05-01 18:01:28.000000 coppyr-0.9.3/coppyr/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 18:02:45.258540 coppyr-0.9.3/coppyr/collections/
+-rw-rw-r--   0 root         (0) root         (0)       78 2023-04-24 19:49:53.000000 coppyr-0.9.3/coppyr/collections/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1091 2023-04-24 19:49:53.000000 coppyr-0.9.3/coppyr/collections/cycle.py
+-rw-rw-r--   0 root         (0) root         (0)      856 2023-04-28 16:36:15.000000 coppyr-0.9.3/coppyr/collections/dotdict.py
+-rw-rw-r--   0 root         (0) root         (0)     1871 2023-04-28 22:23:32.000000 coppyr-0.9.3/coppyr/config.py
+-rw-rw-r--   0 root         (0) root         (0)     4362 2023-05-01 18:00:33.000000 coppyr-0.9.3/coppyr/context.py
+-rw-rw-r--   0 root         (0) root         (0)     2316 2023-04-24 19:56:41.000000 coppyr-0.9.3/coppyr/daemon.py
+-rw-rw-r--   0 root         (0) root         (0)     1645 2023-04-24 19:57:04.000000 coppyr-0.9.3/coppyr/error.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 18:02:45.258540 coppyr-0.9.3/coppyr/extensions/
+-rw-rw-r--   0 root         (0) root         (0)       24 2023-04-24 19:49:53.000000 coppyr-0.9.3/coppyr/extensions/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     3152 2023-04-24 20:41:07.000000 coppyr-0.9.3/coppyr/extensions/load.py
+-rw-rw-r--   0 root         (0) root         (0)     4735 2023-05-01 00:53:09.000000 coppyr-0.9.3/coppyr/logger.py
+-rw-rw-r--   0 root         (0) root         (0)     2428 2023-04-25 15:19:57.000000 coppyr-0.9.3/coppyr/package.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 18:02:45.258540 coppyr-0.9.3/coppyr/process/
+-rw-rw-r--   0 root         (0) root         (0)       24 2023-04-27 19:30:48.000000 coppyr-0.9.3/coppyr/process/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1431 2023-04-24 19:55:39.000000 coppyr-0.9.3/coppyr/process/concurrent.py
+-rw-rw-r--   0 root         (0) root         (0)    10912 2023-04-24 19:58:31.000000 coppyr-0.9.3/coppyr/process/parallel.py
+-rw-rw-r--   0 root         (0) root         (0)     3881 2023-04-28 22:09:04.000000 coppyr-0.9.3/coppyr/process/subp.py
+-rw-rw-r--   0 root         (0) root         (0)      389 2023-04-24 19:49:53.000000 coppyr-0.9.3/coppyr/testing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 18:02:45.258540 coppyr-0.9.3/coppyr/types/
+-rw-rw-r--   0 root         (0) root         (0)      179 2023-04-27 21:29:25.000000 coppyr-0.9.3/coppyr/types/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     3569 2023-04-27 23:05:32.000000 coppyr-0.9.3/coppyr/types/differ.py
+-rw-rw-r--   0 root         (0) root         (0)      351 2023-04-24 19:49:53.000000 coppyr-0.9.3/coppyr/types/lazyproperty.py
+-rw-rw-r--   0 root         (0) root         (0)     1187 2023-04-27 19:30:58.000000 coppyr-0.9.3/coppyr/types/singleton.py
+-rw-rw-r--   0 root         (0) root         (0)      763 2023-04-27 19:56:36.000000 coppyr-0.9.3/coppyr/types/slot.py
+-rw-rw-r--   0 root         (0) root         (0)     1028 2023-04-24 20:44:01.000000 coppyr-0.9.3/coppyr/web.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 18:02:45.258540 coppyr-0.9.3/coppyr.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4983 2023-05-01 18:02:45.000000 coppyr-0.9.3/coppyr.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      732 2023-05-01 18:02:45.000000 coppyr-0.9.3/coppyr.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-01 18:02:45.000000 coppyr-0.9.3/coppyr.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      166 2023-05-01 18:02:45.000000 coppyr-0.9.3/coppyr.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-05-01 18:02:45.000000 coppyr-0.9.3/coppyr.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)      152 2023-04-28 22:20:08.000000 coppyr-0.9.3/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-01 18:02:45.258540 coppyr-0.9.3/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1285 2023-04-25 15:26:56.000000 coppyr-0.9.3/setup.py
```

### Comparing `coppyr-0.9.2/LICENSE` & `coppyr-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `coppyr-0.9.2/PKG-INFO` & `coppyr-0.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coppyr
-Version: 0.9.2
+Version: 0.9.3
 Summary: A collection of boilerplate for Python applications.
 Home-page: https://github.com/gshulegaard/coppyr
 Author: Grant Hulegaard
 Author-email: loki.labrys@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `coppyr-0.9.2/README.rst` & `coppyr-0.9.3/README.rst`

 * *Files identical despite different names*

### Comparing `coppyr-0.9.2/coppyr/collections/cycle.py` & `coppyr-0.9.3/coppyr/collections/cycle.py`

 * *Files identical despite different names*

### Comparing `coppyr-0.9.2/coppyr/collections/dotdict.py` & `coppyr-0.9.3/coppyr/collections/dotdict.py`

 * *Files identical despite different names*

### Comparing `coppyr-0.9.2/coppyr/config.py` & `coppyr-0.9.3/coppyr/config.py`

 * *Files identical despite different names*

### Comparing `coppyr-0.9.2/coppyr/context.py` & `coppyr-0.9.3/coppyr/context.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         for _, timing in enumerate(self.timings):
             name, stamp, relative, duration = timing
             profile[name] = (stamp, f"{relative:.3f}s", f"{duration:.3f}s")
 
         return profile
 
 
-class Context(Singleton):
+class BaseContext:
     """
     A simple interpreter local context that can be used as a shared memory
     space without relying on "global" or careful variable passing.
     """
     def __init__(
         self,
         app_name: Optional[str]=None,
@@ -49,15 +49,15 @@
         reinitialize: bool=False
     ):
         # skip duplicate initialization calls
         if not self._init and not reinitialize:
             return
 
         # constant vars
-        self.app_name = app_name if app_name is not None else "piston"
+        self.app_name = app_name if app_name is not None else "coppyr"
         self.pid = os.getpid()
         self.config_path = config_path
 
         # dynamic vars
         self.ids = cycle(100000, 1000000)
         self.action_id = f"{self.pid}_{next(self.ids)}"
         self.action_stamp = time.time()
@@ -162,7 +162,11 @@
         ]
 
         return fds
 
     @lazyproperty
     def timer(self):
         return TimeKeeper()
+
+
+class Context(BaseContext, Singleton):
+    pass
```

### Comparing `coppyr-0.9.2/coppyr/daemon.py` & `coppyr-0.9.3/coppyr/daemon.py`

 * *Files identical despite different names*

### Comparing `coppyr-0.9.2/coppyr/error.py` & `coppyr-0.9.3/coppyr/error.py`

 * *Files identical despite different names*

### Comparing `coppyr-0.9.2/coppyr/extensions/load.py` & `coppyr-0.9.3/coppyr/extensions/load.py`

 * *Files identical despite different names*

### Comparing `coppyr-0.9.2/coppyr/logger.py` & `coppyr-0.9.3/coppyr/logger.py`

 * *Files identical despite different names*

### Comparing `coppyr-0.9.2/coppyr/package.py` & `coppyr-0.9.3/coppyr/package.py`

 * *Files identical despite different names*

### Comparing `coppyr-0.9.2/coppyr/process/concurrent.py` & `coppyr-0.9.3/coppyr/process/concurrent.py`

 * *Files identical despite different names*

### Comparing `coppyr-0.9.2/coppyr/process/parallel.py` & `coppyr-0.9.3/coppyr/process/parallel.py`

 * *Files identical despite different names*

### Comparing `coppyr-0.9.2/coppyr/process/subp.py` & `coppyr-0.9.3/coppyr/process/subp.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,34 @@
 # -*- coding: utf-8 -*-
 import subprocess
+from logging import Logger
+
+from typing import ByteString, List, Optional, Tuple, TextIO, Union
 
 from coppyr.error import CoppyrError
 
 
 class CoppyrSubpError(CoppyrError):
     description = "An error occurred durring subp.call"
 
 
-def call(command, check=True, raw=False, fg=False, input=None,
-         stdin=None, stdout=None, stderr=None, log=None):
+def call(
+    command: str,
+    check: bool=True,
+    raw: bool=False,
+    fg: bool=False,
+    input: Optional[str]=None,
+    stdin: Optional[TextIO]=None,
+    stdout: Optional[TextIO]=None,
+    stderr: Optional[TextIO]=None,
+    log: Optional[Logger]=None
+) -> Union[
+    Tuple[int, List[str], List[str]],
+    Tuple[int, ByteString, ByteString]
+]:
     """
     Calls subprocess.run with the pass command.
 
     :param command: String
         Full shell command
     :param check: Boolean
         Check the return code or not
@@ -35,35 +50,35 @@
         subprocess.PIPE.
     :param log: logging.Logger
         Logger to send log entries to.  Can be `None` to disable logging.
         Disabled by default.
     :return: retcode int, stdout [], stderr []
     """
     subprocess_params = dict(
-        shell=True,
+        shell=True
     )
 
     if not fg:
-        stdin = subprocess.PIPE if stdin is None else stdin
-        stdout = subprocess.PIPE if stdout is None else stdout
-        stderr = subprocess.PIPE if stderr is None else stderr
+        stdin = subprocess.PIPE if stdin is None else stdin  # type: ignore
+        stdout = subprocess.PIPE if stdout is None else stdout  # type: ignore
+        stderr = subprocess.PIPE if stderr is None else stderr  # type: ignore
 
-        subprocess_params.update(dict(
+        subprocess_params.update(dict(  # type: ignore
             stdin=stdin,
             stdout=stdout,
             stderr=stderr
         ))
 
     if input:
         if 'stdin' in subprocess_params:
             del subprocess_params['stdin']
-        subprocess_params['input'] = input
+        subprocess_params['input'] = input  # type: ignore
 
     if log is not None:
-        log.debug(f"piston.subp.call: Calling \"{command}\"")
+        log.debug(f"coppyr.subp.call: Calling \"{command}\"")
 
     process = subprocess.run(command, **subprocess_params)
 
     try:
         if process.returncode != 0 and check:
             if log is not None:
                 log.error(
@@ -72,35 +87,35 @@
                 )
 
             raise CoppyrSubpError(
                 message=f"\"{command}\" returned a non-zero exit code.",
                 payload=dict(returncode=process.returncode)
             )
         elif fg:
-            return process.returncode, None, None
+            return process.returncode, [], []
         elif raw:
             return process.returncode, process.stdout, process.stderr
         else:
             # out, err are bytes objects
             out = process.stdout.decode("utf-8").split('\n')
             err = process.stderr.decode("utf-8").split('\n')
 
             if log is not None:
                 if out:
-                    log.debug("piston.subp.call: stdout:\n" + "\n".join(out) + "\n")
+                    log.debug("coppyr.subp.call: stdout:\n" + "\n".join(out) + "\n")
                 if process.stderr:
-                    log.error("piston.subp.call: stderr:\n" + "\n".join(err) + "\n")
+                    log.error("coppyr.subp.call: stderr:\n" + "\n".join(err) + "\n")
 
             return process.returncode, out, err
     except CoppyrSubpError:
         raise
     except Exception as e:
         if log is not None:
             log.error(
-                f"piston.subp.call: Caught \"{e.__class__.__name__}\" during "
+                f"coppyr.subp.call: Caught \"{e.__class__.__name__}\" during "
                 "subp.call."
             )
 
         raise CoppyrSubpError(
             f"Caught \"{e.__class__.__name__}\" during subp.call.",
             payload={"command": command},
             caught=e
```

### Comparing `coppyr-0.9.2/coppyr/types/differ.py` & `coppyr-0.9.3/coppyr/types/differ.py`

 * *Files identical despite different names*

### Comparing `coppyr-0.9.2/coppyr/types/singleton.py` & `coppyr-0.9.3/coppyr/types/singleton.py`

 * *Files identical despite different names*

### Comparing `coppyr-0.9.2/coppyr/types/slot.py` & `coppyr-0.9.3/coppyr/types/slot.py`

 * *Files identical despite different names*

### Comparing `coppyr-0.9.2/coppyr/web.py` & `coppyr-0.9.3/coppyr/web.py`

 * *Files identical despite different names*

### Comparing `coppyr-0.9.2/coppyr.egg-info/PKG-INFO` & `coppyr-0.9.3/coppyr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coppyr
-Version: 0.9.2
+Version: 0.9.3
 Summary: A collection of boilerplate for Python applications.
 Home-page: https://github.com/gshulegaard/coppyr
 Author: Grant Hulegaard
 Author-email: loki.labrys@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `coppyr-0.9.2/coppyr.egg-info/SOURCES.txt` & `coppyr-0.9.3/coppyr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `coppyr-0.9.2/setup.py` & `coppyr-0.9.3/setup.py`

 * *Files identical despite different names*

