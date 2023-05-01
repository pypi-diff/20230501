# Comparing `tmp/yamcs-cli-1.4.5.tar.gz` & `tmp/yamcs-cli-1.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/yamcs-cli-1.4.5.tar", last modified: Tue Nov 22 13:57:55 2022, max compression
+gzip compressed data, was "yamcs-cli-1.4.6.tar", last modified: Mon May  1 13:47:54 2023, max compression
```

## Comparing `yamcs-cli-1.4.5.tar` & `yamcs-cli-1.4.6.tar`

### file list

```diff
@@ -1,48 +1,50 @@
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2022-11-22 13:57:55.511162 yamcs-cli-1.4.5/
--rw-r--r--   0 fdi        (503) staff       (20)     7652 2018-08-10 14:54:30.000000 yamcs-cli-1.4.5/LICENSE
--rw-r--r--   0 fdi        (503) staff       (20)       75 2022-10-22 16:16:29.000000 yamcs-cli-1.4.5/MANIFEST.in
--rw-r--r--   0 fdi        (503) staff       (20)     1423 2022-11-22 13:57:55.510713 yamcs-cli-1.4.5/PKG-INFO
--rw-r--r--   0 fdi        (503) staff       (20)      279 2019-08-30 14:25:22.000000 yamcs-cli-1.4.5/README.md
--rw-r--r--   0 fdi        (503) staff       (20)       38 2022-11-22 13:57:55.511313 yamcs-cli-1.4.5/setup.cfg
--rw-r--r--   0 fdi        (503) staff       (20)     1563 2022-11-22 13:47:50.000000 yamcs-cli-1.4.5/setup.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2022-11-22 13:57:55.279855 yamcs-cli-1.4.5/src/
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2022-11-22 13:57:55.278230 yamcs-cli-1.4.5/src/yamcs/
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2022-11-22 13:57:55.444409 yamcs-cli-1.4.5/src/yamcs/cli/
--rw-r--r--   0 fdi        (503) staff       (20)     3826 2022-10-22 11:26:28.000000 yamcs-cli-1.4.5/src/yamcs/cli/__main__.py
--rw-r--r--   0 fdi        (503) staff       (20)     1574 2022-10-22 10:54:37.000000 yamcs-cli-1.4.5/src/yamcs/cli/algorithms.py
--rw-r--r--   0 fdi        (503) staff       (20)     1032 2022-10-22 15:53:01.000000 yamcs-cli-1.4.5/src/yamcs/cli/bash_completion.sh
--rw-r--r--   0 fdi        (503) staff       (20)     1565 2022-10-22 10:54:48.000000 yamcs-cli-1.4.5/src/yamcs/cli/commands.py
--rw-r--r--   0 fdi        (503) staff       (20)     4190 2022-10-22 21:12:10.000000 yamcs-cli-1.4.5/src/yamcs/cli/completers.py
--rw-r--r--   0 fdi        (503) staff       (20)     2996 2022-10-22 09:44:43.000000 yamcs-cli-1.4.5/src/yamcs/cli/config.py
--rw-r--r--   0 fdi        (503) staff       (20)     1573 2022-10-22 10:55:49.000000 yamcs-cli-1.4.5/src/yamcs/cli/containers.py
--rw-r--r--   0 fdi        (503) staff       (20)    15260 2022-11-11 08:06:16.000000 yamcs-cli-1.4.5/src/yamcs/cli/dbshell.py
--rw-r--r--   0 fdi        (503) staff       (20)     3330 2022-10-22 12:17:29.000000 yamcs-cli-1.4.5/src/yamcs/cli/events.py
--rw-r--r--   0 fdi        (503) staff       (20)      238 2022-10-22 10:49:40.000000 yamcs-cli-1.4.5/src/yamcs/cli/exceptions.py
--rw-r--r--   0 fdi        (503) staff       (20)     2071 2022-10-22 07:42:40.000000 yamcs-cli-1.4.5/src/yamcs/cli/instances.py
--rw-r--r--   0 fdi        (503) staff       (20)     2624 2022-10-22 10:56:30.000000 yamcs-cli-1.4.5/src/yamcs/cli/links.py
--rw-r--r--   0 fdi        (503) staff       (20)     3150 2022-10-22 09:37:42.000000 yamcs-cli-1.4.5/src/yamcs/cli/login.py
--rw-r--r--   0 fdi        (503) staff       (20)      525 2022-10-22 10:47:09.000000 yamcs-cli-1.4.5/src/yamcs/cli/logout.py
--rw-r--r--   0 fdi        (503) staff       (20)     1280 2022-10-22 11:07:45.000000 yamcs-cli-1.4.5/src/yamcs/cli/parameter_archive.py
--rw-r--r--   0 fdi        (503) staff       (20)     1573 2022-10-22 10:57:14.000000 yamcs-cli-1.4.5/src/yamcs/cli/parameters.py
--rw-r--r--   0 fdi        (503) staff       (20)     1096 2022-10-22 10:57:21.000000 yamcs-cli-1.4.5/src/yamcs/cli/processors.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2022-11-22 13:57:55.474387 yamcs-cli-1.4.5/src/yamcs/cli/protobuf/
--rw-r--r--   0 fdi        (503) staff       (20)     4293 2022-10-24 20:07:08.000000 yamcs-cli-1.4.5/src/yamcs/cli/protobuf/cmdhistory_pb2.py
--rw-r--r--   0 fdi        (503) staff       (20)    15903 2022-10-24 20:07:08.000000 yamcs-cli-1.4.5/src/yamcs/cli/protobuf/db_pb2.py
--rw-r--r--   0 fdi        (503) staff       (20)    13694 2022-10-24 20:07:08.000000 yamcs-cli-1.4.5/src/yamcs/cli/protobuf/replication_pb2.py
--rw-r--r--   0 fdi        (503) staff       (20)    27760 2022-10-24 20:07:08.000000 yamcs-cli-1.4.5/src/yamcs/cli/protobuf/security_pb2.py
--rw-r--r--   0 fdi        (503) staff       (20)    35497 2022-10-24 20:07:08.000000 yamcs-cli-1.4.5/src/yamcs/cli/protobuf/tablespace_pb2.py
--rw-r--r--   0 fdi        (503) staff       (20)     5098 2022-10-24 20:07:08.000000 yamcs-cli-1.4.5/src/yamcs/cli/protobuf/timeline_pb2.py
--rw-r--r--   0 fdi        (503) staff       (20)     2123 2022-10-22 10:57:37.000000 yamcs-cli-1.4.5/src/yamcs/cli/services.py
--rw-r--r--   0 fdi        (503) staff       (20)     1645 2022-10-22 10:57:49.000000 yamcs-cli-1.4.5/src/yamcs/cli/space_systems.py
--rw-r--r--   0 fdi        (503) staff       (20)     9687 2022-10-22 08:08:00.000000 yamcs-cli-1.4.5/src/yamcs/cli/storage.py
--rw-r--r--   0 fdi        (503) staff       (20)     2344 2022-10-22 10:58:02.000000 yamcs-cli-1.4.5/src/yamcs/cli/streams.py
--rw-r--r--   0 fdi        (503) staff       (20)     7594 2022-10-22 10:58:31.000000 yamcs-cli-1.4.5/src/yamcs/cli/tables.py
--rw-r--r--   0 fdi        (503) staff       (20)     7790 2022-10-22 21:06:47.000000 yamcs-cli-1.4.5/src/yamcs/cli/utils.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2022-11-22 13:57:55.509184 yamcs-cli-1.4.5/src/yamcs_cli.egg-info/
--rw-r--r--   0 fdi        (503) staff       (20)     1423 2022-11-22 13:57:54.000000 yamcs-cli-1.4.5/src/yamcs_cli.egg-info/PKG-INFO
--rw-r--r--   0 fdi        (503) staff       (20)     1145 2022-11-22 13:57:55.000000 yamcs-cli-1.4.5/src/yamcs_cli.egg-info/SOURCES.txt
--rw-r--r--   0 fdi        (503) staff       (20)        1 2022-11-22 13:57:54.000000 yamcs-cli-1.4.5/src/yamcs_cli.egg-info/dependency_links.txt
--rw-r--r--   0 fdi        (503) staff       (20)       51 2022-11-22 13:57:54.000000 yamcs-cli-1.4.5/src/yamcs_cli.egg-info/entry_points.txt
--rw-r--r--   0 fdi        (503) staff       (20)        1 2022-05-08 20:28:16.000000 yamcs-cli-1.4.5/src/yamcs_cli.egg-info/not-zip-safe
--rw-r--r--   0 fdi        (503) staff       (20)       89 2022-11-22 13:57:55.000000 yamcs-cli-1.4.5/src/yamcs_cli.egg-info/requires.txt
--rw-r--r--   0 fdi        (503) staff       (20)        6 2022-11-22 13:57:55.000000 yamcs-cli-1.4.5/src/yamcs_cli.egg-info/top_level.txt
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2023-05-01 13:47:54.505838 yamcs-cli-1.4.6/
+-rw-r--r--   0 fdi        (503) staff       (20)     7652 2018-08-10 14:54:30.000000 yamcs-cli-1.4.6/LICENSE
+-rw-r--r--   0 fdi        (503) staff       (20)       75 2022-10-22 16:16:29.000000 yamcs-cli-1.4.6/MANIFEST.in
+-rw-r--r--   0 fdi        (503) staff       (20)     1371 2023-05-01 13:47:54.505679 yamcs-cli-1.4.6/PKG-INFO
+-rw-r--r--   0 fdi        (503) staff       (20)      279 2019-08-30 14:25:22.000000 yamcs-cli-1.4.6/README.md
+-rw-r--r--   0 fdi        (503) staff       (20)       38 2023-05-01 13:47:54.505884 yamcs-cli-1.4.6/setup.cfg
+-rw-r--r--   0 fdi        (503) staff       (20)     1613 2023-05-01 13:05:24.000000 yamcs-cli-1.4.6/setup.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2023-05-01 13:47:54.467741 yamcs-cli-1.4.6/src/
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2023-05-01 13:47:54.466941 yamcs-cli-1.4.6/src/yamcs/
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2023-05-01 13:47:54.475397 yamcs-cli-1.4.6/src/yamcs/cli/
+-rw-r--r--   0 fdi        (503) staff       (20)     4049 2023-04-16 11:04:52.000000 yamcs-cli-1.4.6/src/yamcs/cli/__main__.py
+-rw-r--r--   0 fdi        (503) staff       (20)     7063 2023-05-01 13:21:13.000000 yamcs-cli-1.4.6/src/yamcs/cli/alarms.py
+-rw-r--r--   0 fdi        (503) staff       (20)     1574 2022-10-22 10:54:37.000000 yamcs-cli-1.4.6/src/yamcs/cli/algorithms.py
+-rw-r--r--   0 fdi        (503) staff       (20)     1032 2022-10-22 15:53:01.000000 yamcs-cli-1.4.6/src/yamcs/cli/bash_completion.sh
+-rw-r--r--   0 fdi        (503) staff       (20)     6223 2023-04-14 21:28:47.000000 yamcs-cli-1.4.6/src/yamcs/cli/commands.py
+-rw-r--r--   0 fdi        (503) staff       (20)     4445 2023-04-04 09:37:18.000000 yamcs-cli-1.4.6/src/yamcs/cli/completers.py
+-rw-r--r--   0 fdi        (503) staff       (20)     2996 2022-10-22 09:44:43.000000 yamcs-cli-1.4.6/src/yamcs/cli/config.py
+-rw-r--r--   0 fdi        (503) staff       (20)     1573 2022-10-22 10:55:49.000000 yamcs-cli-1.4.6/src/yamcs/cli/containers.py
+-rw-r--r--   0 fdi        (503) staff       (20)    15255 2023-04-14 09:33:16.000000 yamcs-cli-1.4.6/src/yamcs/cli/dbshell.py
+-rw-r--r--   0 fdi        (503) staff       (20)     5321 2023-04-14 21:27:59.000000 yamcs-cli-1.4.6/src/yamcs/cli/events.py
+-rw-r--r--   0 fdi        (503) staff       (20)      238 2022-10-22 10:49:40.000000 yamcs-cli-1.4.6/src/yamcs/cli/exceptions.py
+-rw-r--r--   0 fdi        (503) staff       (20)     2071 2022-10-22 07:42:40.000000 yamcs-cli-1.4.6/src/yamcs/cli/instances.py
+-rw-r--r--   0 fdi        (503) staff       (20)     3283 2023-04-14 08:36:37.000000 yamcs-cli-1.4.6/src/yamcs/cli/links.py
+-rw-r--r--   0 fdi        (503) staff       (20)     3745 2023-04-16 09:26:32.000000 yamcs-cli-1.4.6/src/yamcs/cli/login.py
+-rw-r--r--   0 fdi        (503) staff       (20)      525 2022-10-22 10:47:09.000000 yamcs-cli-1.4.6/src/yamcs/cli/logout.py
+-rw-r--r--   0 fdi        (503) staff       (20)     2332 2023-04-16 11:02:14.000000 yamcs-cli-1.4.6/src/yamcs/cli/packets.py
+-rw-r--r--   0 fdi        (503) staff       (20)     1280 2022-10-22 11:07:45.000000 yamcs-cli-1.4.6/src/yamcs/cli/parameter_archive.py
+-rw-r--r--   0 fdi        (503) staff       (20)     4248 2023-04-16 10:31:25.000000 yamcs-cli-1.4.6/src/yamcs/cli/parameters.py
+-rw-r--r--   0 fdi        (503) staff       (20)     1941 2023-04-14 13:24:50.000000 yamcs-cli-1.4.6/src/yamcs/cli/processors.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2023-05-01 13:47:54.477284 yamcs-cli-1.4.6/src/yamcs/cli/protobuf/
+-rw-r--r--   0 fdi        (503) staff       (20)     4293 2022-10-24 20:07:08.000000 yamcs-cli-1.4.6/src/yamcs/cli/protobuf/cmdhistory_pb2.py
+-rw-r--r--   0 fdi        (503) staff       (20)    15903 2022-10-24 20:07:08.000000 yamcs-cli-1.4.6/src/yamcs/cli/protobuf/db_pb2.py
+-rw-r--r--   0 fdi        (503) staff       (20)    13694 2022-10-24 20:07:08.000000 yamcs-cli-1.4.6/src/yamcs/cli/protobuf/replication_pb2.py
+-rw-r--r--   0 fdi        (503) staff       (20)    27760 2022-10-24 20:07:08.000000 yamcs-cli-1.4.6/src/yamcs/cli/protobuf/security_pb2.py
+-rw-r--r--   0 fdi        (503) staff       (20)    35497 2022-10-24 20:07:08.000000 yamcs-cli-1.4.6/src/yamcs/cli/protobuf/tablespace_pb2.py
+-rw-r--r--   0 fdi        (503) staff       (20)     5098 2022-10-24 20:07:08.000000 yamcs-cli-1.4.6/src/yamcs/cli/protobuf/timeline_pb2.py
+-rw-r--r--   0 fdi        (503) staff       (20)     2123 2022-10-22 10:57:37.000000 yamcs-cli-1.4.6/src/yamcs/cli/services.py
+-rw-r--r--   0 fdi        (503) staff       (20)     2238 2023-04-13 12:54:51.000000 yamcs-cli-1.4.6/src/yamcs/cli/space_systems.py
+-rw-r--r--   0 fdi        (503) staff       (20)     9687 2022-10-22 08:08:00.000000 yamcs-cli-1.4.6/src/yamcs/cli/storage.py
+-rw-r--r--   0 fdi        (503) staff       (20)     2344 2022-10-22 10:58:02.000000 yamcs-cli-1.4.6/src/yamcs/cli/streams.py
+-rw-r--r--   0 fdi        (503) staff       (20)     8431 2023-04-04 09:37:20.000000 yamcs-cli-1.4.6/src/yamcs/cli/tables.py
+-rw-r--r--   0 fdi        (503) staff       (20)     8080 2023-05-01 13:05:24.000000 yamcs-cli-1.4.6/src/yamcs/cli/utils.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2023-05-01 13:47:54.505447 yamcs-cli-1.4.6/src/yamcs_cli.egg-info/
+-rw-r--r--   0 fdi        (503) staff       (20)     1371 2023-05-01 13:47:54.000000 yamcs-cli-1.4.6/src/yamcs_cli.egg-info/PKG-INFO
+-rw-r--r--   0 fdi        (503) staff       (20)     1194 2023-05-01 13:47:54.000000 yamcs-cli-1.4.6/src/yamcs_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 fdi        (503) staff       (20)        1 2023-05-01 13:47:54.000000 yamcs-cli-1.4.6/src/yamcs_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 fdi        (503) staff       (20)       50 2023-05-01 13:47:54.000000 yamcs-cli-1.4.6/src/yamcs_cli.egg-info/entry_points.txt
+-rw-r--r--   0 fdi        (503) staff       (20)        1 2022-05-08 20:28:16.000000 yamcs-cli-1.4.6/src/yamcs_cli.egg-info/not-zip-safe
+-rw-r--r--   0 fdi        (503) staff       (20)       89 2023-05-01 13:47:54.000000 yamcs-cli-1.4.6/src/yamcs_cli.egg-info/requires.txt
+-rw-r--r--   0 fdi        (503) staff       (20)        6 2023-05-01 13:47:54.000000 yamcs-cli-1.4.6/src/yamcs_cli.egg-info/top_level.txt
```

### Comparing `yamcs-cli-1.4.5/LICENSE` & `yamcs-cli-1.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `yamcs-cli-1.4.5/PKG-INFO` & `yamcs-cli-1.4.6/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,40 +1,42 @@
 Metadata-Version: 2.1
 Name: yamcs-cli
-Version: 1.4.5
+Version: 1.4.6
 Summary: Yamcs Command-Line Tools
 Home-page: https://github.com/yamcs/yamcs-cli
 Author: Space Applications Services
 Author-email: yamcs@spaceapplications.com
 License: LGPL
-Description: # Command-Line Interface
-        
-        ## Development Setup
-        
-        Install build dependencies (you may want to do this in a virtualenv):
-        
-            pip install -r requirements.txt
-        
-        
-        Install `yamcs-cli` from the source base:
-        
-            python setup.py develop
-        
-        Changes to any source file have immediate impact.
-        
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: kerberos
+License-File: LICENSE
+
+# Command-Line Interface
+
+## Development Setup
+
+Install build dependencies (you may want to do this in a virtualenv):
+
+    pip install -r requirements.txt
+
+
+Install `yamcs-cli` from the source base:
+
+    python setup.py develop
+
+Changes to any source file have immediate impact.
```

### Comparing `yamcs-cli-1.4.5/setup.py` & `yamcs-cli-1.4.6/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with io.open("README.md", encoding="utf-8") as f:
     readme = f.read()
 
 setuptools.setup(
     name="yamcs-cli",
-    version="1.4.5",
+    version="1.4.6",
     description="Yamcs Command-Line Tools",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/yamcs/yamcs-cli",
     author="Space Applications Services",
     author_email="yamcs@spaceapplications.com",
     license="LGPL",
@@ -28,15 +28,16 @@
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Operating System :: OS Independent",
     ],
     platforms="Posix; MacOS X; Windows",
-    install_requires=["argcomplete", "python-dateutil", "yamcs-client>=1.7.0"],
+    install_requires=["argcomplete", "python-dateutil", "yamcs-client>=1.9.0"],
     extras_require={"kerberos": ["yamcs-client-kerberos>=1.2.0"]},
     include_package_data=True,
     zip_safe=False,
 )
```

### Comparing `yamcs-cli-1.4.5/src/yamcs/cli/__main__.py` & `yamcs-cli-1.4.6/src/yamcs/cli/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 import argparse
 import logging
 
 import argcomplete
 import pkg_resources
+from yamcs.core.exceptions import Unauthorized
+
 from yamcs.cli import utils
+from yamcs.cli.alarms import AlarmsCommand
 from yamcs.cli.algorithms import AlgorithmsCommand
 from yamcs.cli.commands import CommandsCommand
 from yamcs.cli.completers import InstanceCompleter
 from yamcs.cli.config import ConfigCommand
 from yamcs.cli.containers import ContainersCommand
 from yamcs.cli.dbshell import DbShellCommand
 from yamcs.cli.events import EventsCommand
 from yamcs.cli.exceptions import NoInstanceError, NoServerError
 from yamcs.cli.instances import InstancesCommand
 from yamcs.cli.links import LinksCommand
 from yamcs.cli.login import LoginCommand
 from yamcs.cli.logout import LogoutCommand
+from yamcs.cli.packets import PacketsCommand
 from yamcs.cli.parameter_archive import ParameterArchiveCommand
 from yamcs.cli.parameters import ParametersCommand
 from yamcs.cli.processors import ProcessorsCommand
 from yamcs.cli.services import ServicesCommand
 from yamcs.cli.space_systems import SpaceSystemsCommand
 from yamcs.cli.storage import StorageCommand
 from yamcs.cli.streams import StreamsCommand
 from yamcs.cli.tables import TablesCommand
-from yamcs.core.exceptions import Unauthorized
 
 
 def create_subparser(subparsers, command, help_):
     # Override the default help action so that it does not show up in
     # the usage string of every command
     subparser = subparsers.add_parser(command, help=help_, add_help=False)
     subparser.add_argument(
@@ -62,24 +65,26 @@
 
     # The width of this impacts the command width of the command column :-/
     metavar = "COMMAND"
 
     subparsers = parser.add_subparsers(title="Commands", metavar=metavar)
     subparsers.required = True
 
+    AlarmsCommand(subparsers)
     AlgorithmsCommand(subparsers)
     CommandsCommand(subparsers)
     ConfigCommand(subparsers)
     ContainersCommand(subparsers)
     DbShellCommand(subparsers)
     EventsCommand(subparsers)
     InstancesCommand(subparsers)
     LinksCommand(subparsers)
     LoginCommand(subparsers)
     LogoutCommand(subparsers)
+    PacketsCommand(subparsers)
     ParameterArchiveCommand(subparsers)
     ParametersCommand(subparsers)
     ProcessorsCommand(subparsers)
     ServicesCommand(subparsers)
     SpaceSystemsCommand(subparsers)
     StorageCommand(subparsers)
     StreamsCommand(subparsers)
@@ -99,14 +104,16 @@
     except KeyboardInterrupt:
         print()  # Clear prompt
     except NoServerError:
         print("No server. Run: 'yamcs login' to login to Yamcs")
     except NoInstanceError:
         print("No instance. Run: 'yamcs config set instance <instance>'")
     except Unauthorized:
+        if args.debug:
+            print(logging.traceback.format_exc())
         print("Unauthorized. Run: 'yamcs login' to login to Yamcs")
     except Exception as e:
         if args.debug:
             print(logging.traceback.format_exc())
         else:
             print(e)
```

### Comparing `yamcs-cli-1.4.5/src/yamcs/cli/algorithms.py` & `yamcs-cli-1.4.6/src/yamcs/cli/algorithms.py`

 * *Files identical despite different names*

### Comparing `yamcs-cli-1.4.5/src/yamcs/cli/bash_completion.sh` & `yamcs-cli-1.4.6/src/yamcs/cli/bash_completion.sh`

 * *Files identical despite different names*

### Comparing `yamcs-cli-1.4.5/src/yamcs/cli/commands.py` & `yamcs-cli-1.4.6/src/yamcs/cli/services.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,43 +1,63 @@
 from yamcs.cli import utils
-from yamcs.cli.completers import CommandCompleter
+from yamcs.cli.completers import ServiceCompleter
 from yamcs.client import YamcsClient
 
 
-class CommandsCommand(utils.Command):
+class ServicesCommand(utils.Command):
     def __init__(self, parent):
-        super(CommandsCommand, self).__init__(parent, "commands", "Read commands")
+        super(ServicesCommand, self).__init__(parent, "services", "Manage services")
 
         subparsers = self.parser.add_subparsers(title="Commands", metavar="COMMAND")
         subparsers.required = True
 
-        subparser = self.create_subparser(subparsers, "list", "List commands")
+        subparser = self.create_subparser(subparsers, "list", "List services")
         subparser.set_defaults(func=self.list_)
 
-        subparser = self.create_subparser(subparsers, "describe", "Describe a command")
+        subparser = self.create_subparser(subparsers, "start", "Start a service")
         subparser.add_argument(
-            "command", metavar="NAME", type=str, help="name of the command"
-        ).completer = CommandCompleter
-        subparser.set_defaults(func=self.describe)
+            "services",
+            metavar="SERVICE",
+            type=str,
+            nargs="+",
+            help="name of the service",
+        ).completer = ServiceCompleter
+        subparser.set_defaults(func=self.start)
+
+        subparser = self.create_subparser(subparsers, "stop", "Stop a service")
+        subparser.add_argument(
+            "services",
+            metavar="SERVICE",
+            type=str,
+            nargs="+",
+            help="name of the service",
+        ).completer = ServiceCompleter
+        subparser.set_defaults(func=self.stop)
 
     def list_(self, args):
         opts = utils.CommandOptions(args)
         client = YamcsClient(**opts.client_kwargs)
-        mdb = client.get_mdb(opts.require_instance())
 
-        rows = [["NAME", "DESCRIPTION", "ABSTRACT"]]
-        for command in mdb.list_commands():
+        rows = [["NAME", "CLASS", "STATUS"]]
+        for service in client.list_services(opts.require_instance()):
             rows.append(
                 [
-                    command.qualified_name,
-                    command.description,
-                    command.abstract,
+                    service.name,
+                    service.class_name,
+                    service.state,
                 ]
             )
         utils.print_table(rows)
 
-    def describe(self, args):
+    def start(self, args):
         opts = utils.CommandOptions(args)
         client = YamcsClient(**opts.client_kwargs)
-        mdb = client.get_mdb(opts.require_instance())
-        command = mdb.get_command(args.command)
-        print(command._proto)
+
+        for service in args.services:
+            client.start_service(opts.require_instance(), service=service)
+
+    def stop(self, args):
+        opts = utils.CommandOptions(args)
+        client = YamcsClient(**opts.client_kwargs)
+
+        for service in args.services:
+            client.stop_service(opts.require_instance(), service=service)
```

### Comparing `yamcs-cli-1.4.5/src/yamcs/cli/completers.py` & `yamcs-cli-1.4.6/src/yamcs/cli/completers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-from yamcs.cli import utils
 from yamcs.client import YamcsClient
 
+from yamcs.cli import utils
+
 
 def AlgorithmCompleter(prefix, parsed_args, **kwargs):
     opts = utils.CommandOptions(parsed_args)
     client = YamcsClient(**opts.client_kwargs)
     mdb = client.get_mdb(opts.require_instance())
     return [x.qualified_name for x in mdb.list_algorithms()]
 
@@ -81,14 +82,21 @@
 def ParameterCompleter(prefix, parsed_args, **kwargs):
     opts = utils.CommandOptions(parsed_args)
     client = YamcsClient(**opts.client_kwargs)
     mdb = client.get_mdb(opts.require_instance())
     return [x.qualified_name for x in mdb.list_parameters()]
 
 
+def ProcessorCompleter(prefix, parsed_args, **kwargs):
+    opts = utils.CommandOptions(parsed_args)
+    client = YamcsClient(**opts.client_kwargs)
+    processors = client.list_processors(opts.require_instance())
+    return [x.name for x in processors]
+
+
 def ServiceCompleter(prefix, parsed_args, **kwargs):
     opts = utils.CommandOptions(parsed_args)
     client = YamcsClient(**opts.client_kwargs)
     return [x.name for x in client.list_services(opts.require_instance())]
 
 
 def SpaceSystemCompleter(prefix, parsed_args, **kwargs):
```

### Comparing `yamcs-cli-1.4.5/src/yamcs/cli/config.py` & `yamcs-cli-1.4.6/src/yamcs/cli/config.py`

 * *Files identical despite different names*

### Comparing `yamcs-cli-1.4.5/src/yamcs/cli/containers.py` & `yamcs-cli-1.4.6/src/yamcs/cli/containers.py`

 * *Files identical despite different names*

### Comparing `yamcs-cli-1.4.5/src/yamcs/cli/dbshell.py` & `yamcs-cli-1.4.6/src/yamcs/cli/dbshell.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,20 +5,21 @@
 import os
 import readline
 import sys
 from collections import abc
 from pydoc import pager
 
 from google.protobuf import json_format
-from yamcs.cli import utils
-from yamcs.cli.protobuf import cmdhistory_pb2, timeline_pb2
 from yamcs.client import YamcsClient
 from yamcs.core.exceptions import YamcsError
 from yamcs.protobuf.events import events_pb2
 
+from yamcs.cli import utils
+from yamcs.cli.protobuf import cmdhistory_pb2, timeline_pb2
+
 SHOW_OPTIONS = ("databases", "engines", "streams", "tables", "stream")
 
 PB_ASSIGNMENT_TYPE = "PROTOBUF(org.yamcs.cmdhistory.protobuf.Cmdhistory$AssignmentInfo)"
 PB_BANDFILTER_TYPE = "PROTOBUF(org.yamcs.timeline.protobuf.BandFilter)"
 PB_EVENT_TYPE = "PROTOBUF(org.yamcs.yarch.protobuf.Db$Event)"
 
 
@@ -43,15 +44,15 @@
         self.parser.add_argument(
             "-c", "--command", metavar="COMMAND", type=str, help="SQL command string"
         )
         self.parser.add_argument(
             "-N",
             "--skip-column-names",
             action="store_true",
-            help="Don't print print column names",
+            help="Don't print column names",
         )
         self.parser.add_argument(
             "-B",
             "--batch",
             action="store_true",
             help="Don't use history file. Disable interactive behavior",
         )
```

### Comparing `yamcs-cli-1.4.5/src/yamcs/cli/instances.py` & `yamcs-cli-1.4.6/src/yamcs/cli/instances.py`

 * *Files identical despite different names*

### Comparing `yamcs-cli-1.4.5/src/yamcs/cli/links.py` & `yamcs-cli-1.4.6/src/yamcs/cli/links.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
+from yamcs.client import YamcsClient
+
 from yamcs.cli import utils
 from yamcs.cli.completers import LinkCompleter
-from yamcs.client import YamcsClient
 
 
 class LinksCommand(utils.Command):
     def __init__(self, parent):
         super(LinksCommand, self).__init__(parent, "links", "Manage data links")
 
         subparsers = self.parser.add_subparsers(title="Commands", metavar="COMMAND")
@@ -27,14 +28,25 @@
 
         subparser = self.create_subparser(subparsers, "disable", "Disable a link")
         subparser.add_argument(
             "links", metavar="LINK", type=str, nargs="+", help="name of the link"
         ).completer = LinkCompleter
         subparser.set_defaults(func=self.disable)
 
+        subparser = self.create_subparser(
+            subparsers, "run-action", "Run a custom link action"
+        )
+        subparser.add_argument(
+            "link", metavar="LINK", type=str, help="name of the link"
+        ).completer = LinkCompleter
+        subparser.add_argument(
+            "action", metavar="ACTION", type=str, help="name of the action"
+        )
+        subparser.set_defaults(func=self.run_action)
+
     def list_(self, args):
         opts = utils.CommandOptions(args)
         client = YamcsClient(**opts.client_kwargs)
 
         rows = [["NAME", "CLASS", "STATUS", "IN", "OUT"]]
         for link in client.list_links(opts.require_instance()):
             rows.append(
@@ -65,7 +77,13 @@
             link.disable_link()
 
     def describe(self, args):
         opts = utils.CommandOptions(args)
         client = YamcsClient(**opts.client_kwargs)
         link = client.get_link(opts.require_instance(), args.link)
         print(link.get_info())
+
+    def run_action(self, args):
+        opts = utils.CommandOptions(args)
+        client = YamcsClient(**opts.client_kwargs)
+        link = client.get_link(opts.require_instance(), args.link)
+        link.run_action(args.action)
```

### Comparing `yamcs-cli-1.4.5/src/yamcs/cli/login.py` & `yamcs-cli-1.4.6/src/yamcs/cli/login.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,15 @@
+import os
 from getpass import getpass
 
-from yamcs.cli import utils
 from yamcs.client import YamcsClient
 from yamcs.core import auth
 
+from yamcs.cli import utils
+
 
 class LoginCommand(utils.Command):
     def __init__(self, parent):
         super(LoginCommand, self).__init__(parent, "login", "Login to a Yamcs server")
 
         self.parser.set_defaults(func=self.do_login)
         self.parser.add_argument(
@@ -18,14 +20,19 @@
             help="server URL (example: http://localhost:8090)",
         )
         self.parser.add_argument(
             "--kerberos",
             action="store_true",
             help="Authenticate using Kerberos negotiation",
         )
+        self.parser.add_argument(
+            "-u",
+            "--username",
+            help="Username",
+        )
 
     def do_login(self, args):
         opts = utils.CommandOptions(args)
 
         url = args.url or self.read_url(opts)
 
         client_kwargs = {
@@ -45,36 +52,48 @@
                     "the optional package: yamcs-client-kerberos"
                 )
                 return False
 
             credentials = KerberosCredentials()
             client = YamcsClient(credentials=credentials, **client_kwargs)
             print("Login succeeded")
+        elif args.username:
+            credentials = self.read_credentials(username=args.username)
+            if credentials:
+                client = YamcsClient(credentials=credentials, **client_kwargs)
+                print("Login succeeded")
+            else:
+                return
         elif client.get_auth_info().require_authentication:
             credentials = self.read_credentials()
             if credentials:
                 client = YamcsClient(credentials=credentials, **client_kwargs)
                 print("Login succeeded")
+            else:
+                return
         else:
             user_info = client.get_user_info()
             print("Anonymous login succeeded (username: {})".format(user_info.username))
 
         self.save_client_config(client, opts.config)
 
     def read_url(self, opts):
         default_url = opts.url or "http://localhost:8090"
         return input("URL [{}]: ".format(default_url)) or default_url
 
-    def read_credentials(self):
-        username = input("Username: ")
+    def read_credentials(self, username=None):
+        if username is None:
+            username = input("Username: ")
         if not username:
             print("*** Username may not be empty")
             return False
 
-        password = getpass("Password: ")
+        password = os.environ.get("YAMCS_CLI_PASSWORD")
+        if password is None:
+            password = getpass("Password: ")
         if not password:
             print("*** Password may not be empty")
             return False
 
         return auth.Credentials(username=username, password=password)
 
     def save_client_config(self, client, config):
```

### Comparing `yamcs-cli-1.4.5/src/yamcs/cli/logout.py` & `yamcs-cli-1.4.6/src/yamcs/cli/logout.py`

 * *Files identical despite different names*

### Comparing `yamcs-cli-1.4.5/src/yamcs/cli/parameter_archive.py` & `yamcs-cli-1.4.6/src/yamcs/cli/parameter_archive.py`

 * *Files identical despite different names*

### Comparing `yamcs-cli-1.4.5/src/yamcs/cli/processors.py` & `yamcs-cli-1.4.6/src/yamcs/cli/processors.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,31 +1,60 @@
-from yamcs.cli import utils
 from yamcs.client import YamcsClient
 
+from yamcs.cli import utils
+from yamcs.cli.completers import ProcessorCompleter
+
 
 class ProcessorsCommand(utils.Command):
     def __init__(self, parent):
         super(ProcessorsCommand, self).__init__(parent, "processors", "Read processors")
 
         subparsers = self.parser.add_subparsers(title="Commands", metavar="COMMAND")
         subparsers.required = True
 
         subparser = self.create_subparser(subparsers, "list", "List processors")
         subparser.set_defaults(func=self.list_)
 
+        subparser = self.create_subparser(subparsers, "delete", "Delete processor")
+        subparser.add_argument(
+            "processors",
+            metavar="PROCESSOR",
+            type=str,
+            nargs="+",
+            help="name of the processor",
+        ).completer = ProcessorCompleter
+        subparser.set_defaults(func=self.delete)
+
     def list_(self, args):
         opts = utils.CommandOptions(args)
         client = YamcsClient(**opts.client_kwargs)
 
-        rows = [["NAME", "TYPE", "OWNER", "PERSISTENT", "MISSION TIME", "STATE"]]
+        rows = [
+            [
+                "NAME",
+                "TYPE",
+                "OWNER",
+                "PERSISTENT",
+                "PROTECTED",
+                "MISSION TIME",
+                "STATE",
+            ]
+        ]
         for processor in client.list_processors(opts.require_instance()):
             rows.append(
                 [
                     processor.name,
                     processor.type,
                     processor.owner,
                     processor.persistent,
+                    processor.protected,
                     processor.mission_time,
                     processor.state,
                 ]
             )
         utils.print_table(rows)
+
+    def delete(self, args):
+        opts = utils.CommandOptions(args)
+        client = YamcsClient(**opts.client_kwargs)
+        for processor in args.processors:
+            client.delete_processor(opts.require_instance(), processor)
```

### Comparing `yamcs-cli-1.4.5/src/yamcs/cli/protobuf/cmdhistory_pb2.py` & `yamcs-cli-1.4.6/src/yamcs/cli/protobuf/cmdhistory_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs-cli-1.4.5/src/yamcs/cli/protobuf/db_pb2.py` & `yamcs-cli-1.4.6/src/yamcs/cli/protobuf/db_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs-cli-1.4.5/src/yamcs/cli/protobuf/replication_pb2.py` & `yamcs-cli-1.4.6/src/yamcs/cli/protobuf/replication_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs-cli-1.4.5/src/yamcs/cli/protobuf/security_pb2.py` & `yamcs-cli-1.4.6/src/yamcs/cli/protobuf/security_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs-cli-1.4.5/src/yamcs/cli/protobuf/tablespace_pb2.py` & `yamcs-cli-1.4.6/src/yamcs/cli/protobuf/tablespace_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs-cli-1.4.5/src/yamcs/cli/protobuf/timeline_pb2.py` & `yamcs-cli-1.4.6/src/yamcs/cli/protobuf/timeline_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs-cli-1.4.5/src/yamcs/cli/space_systems.py` & `yamcs-cli-1.4.6/src/yamcs/cli/space_systems.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
+from yamcs.client import YamcsClient
+
 from yamcs.cli import utils
 from yamcs.cli.completers import SpaceSystemCompleter
-from yamcs.client import YamcsClient
 
 
 class SpaceSystemsCommand(utils.Command):
     def __init__(self, parent):
         super(SpaceSystemsCommand, self).__init__(
             parent, "space-systems", "Read space systems"
         )
@@ -19,14 +20,23 @@
             subparsers, "describe", "Describe a space system"
         )
         subparser.add_argument(
             "space_system", metavar="NAME", type=str, help="name of the space system"
         ).completer = SpaceSystemCompleter
         subparser.set_defaults(func=self.describe)
 
+        subparser = self.create_subparser(
+            subparsers, "export", "Export a space system in XTCE format"
+        )
+
+        subparser.add_argument(
+            "space_system", metavar="NAME", type=str, help="name of the space system"
+        ).completer = SpaceSystemCompleter
+        subparser.set_defaults(func=self.export)
+
     def list_(self, args):
         opts = utils.CommandOptions(args)
         client = YamcsClient(**opts.client_kwargs)
         mdb = client.get_mdb(opts.require_instance())
 
         rows = [["NAME", "DESCRIPTION"]]
         for space_system in mdb.list_space_systems():
@@ -40,7 +50,14 @@
 
     def describe(self, args):
         opts = utils.CommandOptions(args)
         client = YamcsClient(**opts.client_kwargs)
         mdb = client.get_mdb(opts.require_instance())
         space_system = mdb.get_space_system(args.space_system)
         print(space_system._proto)
+
+    def export(self, args):
+        opts = utils.CommandOptions(args)
+        client = YamcsClient(**opts.client_kwargs)
+        mdb = client.get_mdb(opts.require_instance())
+        xtce = mdb.export_space_system(args.space_system)
+        print(xtce)
```

### Comparing `yamcs-cli-1.4.5/src/yamcs/cli/storage.py` & `yamcs-cli-1.4.6/src/yamcs/cli/storage.py`

 * *Files identical despite different names*

### Comparing `yamcs-cli-1.4.5/src/yamcs/cli/streams.py` & `yamcs-cli-1.4.6/src/yamcs/cli/streams.py`

 * *Files identical despite different names*

### Comparing `yamcs-cli-1.4.5/src/yamcs/cli/tables.py` & `yamcs-cli-1.4.6/src/yamcs/cli/tables.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import gzip
 import os
 import time
 from sys import stdout
 
+from yamcs.client import YamcsClient
+
 from yamcs.cli import utils
 from yamcs.cli.completers import TableCompleter
-from yamcs.client import YamcsClient
 
 
 class TablesCommand(utils.Command):
     def __init__(self, parent):
         super(TablesCommand, self).__init__(
             parent, "tables", "Read and manipulate tables"
         )
@@ -26,14 +27,35 @@
         ).completer = TableCompleter
         subparser.set_defaults(func=self.describe)
 
         subparser = self.create_subparser(subparsers, "dump", "Dump tables")
         subparser.add_argument(
             "tables", metavar="TABLE", type=str, nargs="+", help="name of the tables"
         ).completer = TableCompleter
+
+        query_group = subparser.add_mutually_exclusive_group()
+        query_group.add_argument(
+            "-q",
+            "--query",
+            type=str,
+            help=(
+                "Provides a SQL WHERE search condition that limits the rows "
+                "included in the output"
+            ),
+        )
+        query_group.add_argument(
+            "--query-file",
+            metavar="FILE",
+            type=str,
+            help=(
+                "Specifies the path to a file containing a SQL WHERE search "
+                "condition that limits the rows included in the output"
+            ),
+        )
+
         subparser.set_defaults(func=self.dump)
         subparser.add_argument(
             "-d",
             "--dir",
             type=str,
             help=(
                 "Specifies the directory where to output dump files. "
@@ -111,27 +133,33 @@
         opts = utils.CommandOptions(args)
         client = YamcsClient(**opts.client_kwargs)
         archive = client.get_archive(opts.require_instance())
         for table in args.tables:
             path = table + ".dump.gz" if args.gzip else table + ".dump"
             if args.dir:
                 path = os.path.join(args.dir, path)
+
+            query = args.query
+            if args.query_file:
+                with open(args.query_file, "rt") as file:
+                    query = file.read().strip()
+
             if args.gzip:
                 with gzip.open(path, "wb", compresslevel=1) as f:
-                    self.write_dump(f, archive, table, path)
+                    self.write_dump(f, archive, table, query, path)
             else:
                 with open(path, "wb") as f:
-                    self.write_dump(f, archive, table, path)
+                    self.write_dump(f, archive, table, query, path)
 
-    def write_dump(self, f, archive, table, path):
+    def write_dump(self, f, archive, table, query, path):
         txsize = 0
         t0 = time.time()
         t = t0
         prev_t = None
-        for chunk in archive.dump_table(table):
+        for chunk in archive.dump_table(table, query=query):
             txsize += f.write(chunk)
             t = time.time()
             if not prev_t or (t - prev_t > 0.5):  # Limit console writes
                 self.report_dump_stats(path, txsize, t - t0)
                 prev_t = t
         if txsize > 0:
             self.report_dump_stats(path, txsize, t - t0)
@@ -187,15 +215,15 @@
         chunk_size = 32 * 1024
         fsize = os.path.getsize(path)
 
         def report_load_stats(elapsed):
             nonlocal path, fsize, txsize
             rate = (txsize / 1024 / 1024) / elapsed
             stdout.write(
-                "\r{}: {:.2f} MB (rx: {:.2f} MB at {:.2f} MB/s)".format(
+                "\r{}: {:.2f} MB (tx: {:.2f} MB at {:.2f} MB/s)".format(
                     path, fsize / 1024 / 1024, txsize / 1024 / 1024, rate
                 )
             )
             stdout.flush()
 
         def read_in_chunks():
             nonlocal f, txsize, t0, t, prev_t
```

### Comparing `yamcs-cli-1.4.5/src/yamcs/cli/utils.py` & `yamcs-cli-1.4.6/src/yamcs/cli/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,18 +3,19 @@
 import os
 from configparser import ConfigParser
 from datetime import datetime, timedelta, timezone
 from urllib.parse import urlparse
 
 import pkg_resources
 from dateutil import parser
-from yamcs.cli.exceptions import NoInstanceError, NoServerError
 from yamcs.core import auth
 from yamcs.core.helpers import parse_server_timestring, to_isostring
 
+from yamcs.cli.exceptions import NoInstanceError, NoServerError
+
 HOME = os.path.expanduser("~")
 CONFIG_DIR = os.path.join(os.path.join(HOME, ".config"), "yamcs-cli")
 CONFIG_FILE = os.path.join(CONFIG_DIR, "config")
 CREDENTIALS_FILE = os.path.join(CONFIG_DIR, "credentials")
 
 
 def get_user_agent():
@@ -162,16 +163,15 @@
         else:
             return parts[0], parts[1]
     else:
         return parts[0], None
 
 
 class Command(object):
-
-    config_options = ["core.url", "core.instance"]
+    config_options = ["core.url", "core.instance", "core.enable_utc"]
 
     def __init__(self, subparsers, command, help_, add_epilog=True):
         self.parser = self.create_subparser(
             subparsers, command, help_, add_epilog=add_epilog
         )
 
     def create_subparser(self, subparsers, command, help_, add_epilog=True):
@@ -216,28 +216,37 @@
 
 class CommandOptions(object):
     def __init__(self, args):
         self.config = read_config()
         self._credentials = read_credentials()
         self._args = args
 
+        if self.enable_utc:
+            os.environ["PYTHON_YAMCS_CLIENT_UTC"] = "1"
+
     @property
     def instance(self):
         return self._args.instance or (
             self.config.has_section("core")
             and self.config.get("core", "instance", fallback=None)
         )
 
     @property
     def url(self):
         if self.config.has_section("core"):
             return self.config.get("core", "url", fallback=None)
         return None
 
     @property
+    def enable_utc(self):
+        if self.config.has_section("core"):
+            return self.config.getboolean("core", "enable_utc", fallback=False)
+        return False
+
+    @property
     def user_agent(self):
         return get_user_agent()
 
     def require_instance(self):
         if not self.instance:
             raise NoInstanceError()
         return self.instance
```

### Comparing `yamcs-cli-1.4.5/src/yamcs_cli.egg-info/PKG-INFO` & `yamcs-cli-1.4.6/src/yamcs_cli.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,40 +1,42 @@
 Metadata-Version: 2.1
 Name: yamcs-cli
-Version: 1.4.5
+Version: 1.4.6
 Summary: Yamcs Command-Line Tools
 Home-page: https://github.com/yamcs/yamcs-cli
 Author: Space Applications Services
 Author-email: yamcs@spaceapplications.com
 License: LGPL
-Description: # Command-Line Interface
-        
-        ## Development Setup
-        
-        Install build dependencies (you may want to do this in a virtualenv):
-        
-            pip install -r requirements.txt
-        
-        
-        Install `yamcs-cli` from the source base:
-        
-            python setup.py develop
-        
-        Changes to any source file have immediate impact.
-        
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: kerberos
+License-File: LICENSE
+
+# Command-Line Interface
+
+## Development Setup
+
+Install build dependencies (you may want to do this in a virtualenv):
+
+    pip install -r requirements.txt
+
+
+Install `yamcs-cli` from the source base:
+
+    python setup.py develop
+
+Changes to any source file have immediate impact.
```

### Comparing `yamcs-cli-1.4.5/src/yamcs_cli.egg-info/SOURCES.txt` & `yamcs-cli-1.4.6/src/yamcs_cli.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.py
 src/yamcs/cli/__main__.py
+src/yamcs/cli/alarms.py
 src/yamcs/cli/algorithms.py
 src/yamcs/cli/bash_completion.sh
 src/yamcs/cli/commands.py
 src/yamcs/cli/completers.py
 src/yamcs/cli/config.py
 src/yamcs/cli/containers.py
 src/yamcs/cli/dbshell.py
 src/yamcs/cli/events.py
 src/yamcs/cli/exceptions.py
 src/yamcs/cli/instances.py
 src/yamcs/cli/links.py
 src/yamcs/cli/login.py
 src/yamcs/cli/logout.py
+src/yamcs/cli/packets.py
 src/yamcs/cli/parameter_archive.py
 src/yamcs/cli/parameters.py
 src/yamcs/cli/processors.py
 src/yamcs/cli/services.py
 src/yamcs/cli/space_systems.py
 src/yamcs/cli/storage.py
 src/yamcs/cli/streams.py
```

