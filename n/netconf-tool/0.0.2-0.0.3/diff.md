# Comparing `tmp/netconf_tool-0.0.2.tar.gz` & `tmp/netconf_tool-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netconf_tool-0.0.2.tar", last modified: Sat Apr 29 18:06:22 2023, max compression
+gzip compressed data, was "netconf_tool-0.0.3.tar", last modified: Mon May  1 08:55:44 2023, max compression
```

## Comparing `netconf_tool-0.0.2.tar` & `netconf_tool-0.0.3.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:06:22.197682 netconf_tool-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    12920 2023-04-29 18:06:22.197682 netconf_tool-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12693 2023-04-29 18:06:05.000000 netconf_tool-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:06:22.193682 netconf_tool-0.0.2/netconf_tool/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 18:06:05.000000 netconf_tool-0.0.2/netconf_tool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-29 18:06:05.000000 netconf_tool-0.0.2/netconf_tool/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-04-29 18:06:05.000000 netconf_tool-0.0.2/netconf_tool/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-04-29 18:06:05.000000 netconf_tool-0.0.2/netconf_tool/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:06:22.197682 netconf_tool-0.0.2/netconf_tool/operations/
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-04-29 18:06:05.000000 netconf_tool-0.0.2/netconf_tool/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-04-29 18:06:05.000000 netconf_tool-0.0.2/netconf_tool/operations/capabilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-04-29 18:06:05.000000 netconf_tool-0.0.2/netconf_tool/operations/get_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:06:22.197682 netconf_tool-0.0.2/netconf_tool/subscription/
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-29 18:06:05.000000 netconf_tool-0.0.2/netconf_tool/subscription/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-04-29 18:06:05.000000 netconf_tool-0.0.2/netconf_tool/subscription/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-04-29 18:06:05.000000 netconf_tool-0.0.2/netconf_tool/subscription/rabbitmq.py
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-04-29 18:06:05.000000 netconf_tool-0.0.2/netconf_tool/subscription/redis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:06:22.197682 netconf_tool-0.0.2/netconf_tool/yangcli/
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-29 18:06:05.000000 netconf_tool-0.0.2/netconf_tool/yangcli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-04-29 18:06:05.000000 netconf_tool-0.0.2/netconf_tool/yangcli/get_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:06:22.197682 netconf_tool-0.0.2/netconf_tool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12920 2023-04-29 18:06:22.000000 netconf_tool-0.0.2/netconf_tool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-29 18:06:22.000000 netconf_tool-0.0.2/netconf_tool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 18:06:22.000000 netconf_tool-0.0.2/netconf_tool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-29 18:06:22.000000 netconf_tool-0.0.2/netconf_tool.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-29 18:06:22.000000 netconf_tool-0.0.2/netconf_tool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-29 18:06:22.000000 netconf_tool-0.0.2/netconf_tool.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 18:06:22.197682 netconf_tool-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-04-29 18:06:05.000000 netconf_tool-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:55:44.411070 netconf_tool-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    16171 2023-05-01 08:55:44.411070 netconf_tool-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15944 2023-05-01 08:55:23.000000 netconf_tool-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:55:44.407070 netconf_tool-0.0.3/netconf_tool/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 08:55:23.000000 netconf_tool-0.0.3/netconf_tool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-01 08:55:23.000000 netconf_tool-0.0.3/netconf_tool/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-05-01 08:55:23.000000 netconf_tool-0.0.3/netconf_tool/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-05-01 08:55:23.000000 netconf_tool-0.0.3/netconf_tool/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:55:44.407070 netconf_tool-0.0.3/netconf_tool/operations/
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-01 08:55:23.000000 netconf_tool-0.0.3/netconf_tool/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-05-01 08:55:23.000000 netconf_tool-0.0.3/netconf_tool/operations/capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-05-01 08:55:23.000000 netconf_tool-0.0.3/netconf_tool/operations/get_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5233 2023-05-01 08:55:23.000000 netconf_tool-0.0.3/netconf_tool/operations/get_yang.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:55:44.407070 netconf_tool-0.0.3/netconf_tool/subscription/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-01 08:55:23.000000 netconf_tool-0.0.3/netconf_tool/subscription/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-05-01 08:55:23.000000 netconf_tool-0.0.3/netconf_tool/subscription/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-05-01 08:55:23.000000 netconf_tool-0.0.3/netconf_tool/subscription/rabbitmq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-05-01 08:55:23.000000 netconf_tool-0.0.3/netconf_tool/subscription/redis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:55:44.407070 netconf_tool-0.0.3/netconf_tool/yangcli/
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-01 08:55:23.000000 netconf_tool-0.0.3/netconf_tool/yangcli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-05-01 08:55:23.000000 netconf_tool-0.0.3/netconf_tool/yangcli/get_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:55:44.407070 netconf_tool-0.0.3/netconf_tool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16171 2023-05-01 08:55:44.000000 netconf_tool-0.0.3/netconf_tool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-01 08:55:44.000000 netconf_tool-0.0.3/netconf_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 08:55:44.000000 netconf_tool-0.0.3/netconf_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-01 08:55:44.000000 netconf_tool-0.0.3/netconf_tool.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-01 08:55:44.000000 netconf_tool-0.0.3/netconf_tool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-01 08:55:44.000000 netconf_tool-0.0.3/netconf_tool.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 08:55:44.411070 netconf_tool-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-05-01 08:55:23.000000 netconf_tool-0.0.3/setup.py
```

### Comparing `netconf_tool-0.0.2/PKG-INFO` & `netconf_tool-0.0.3/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,7 @@
-Metadata-Version: 2.1
-Name: netconf_tool
-Version: 0.0.2
-Summary: Click CLI application to help with NETCONF development experience
-Home-page: https://github.com/BSpendlove/netconf-tool
-Description-Content-Type: text/markdown
-
 # netconf-tool
 
 This is a tool aimed for developer experience / making things faster when I am trying to test NETCONF related tasks without having to rewrite a random python script. I've found myself constantly writing little python scripts for NETCONF to test functionality or even grab data such as server capabilities, setup event based notifications/subscription to test something and have probably got 100 scripts that do the same thing in different folders through the various projects I've worked on.
 
 Therefore I've created this tool to improve my developer experience working with NETCONF. At the ease of a quick command, I want to be able to get config, try out some edit-config functionality, grab capabilities of a new vendor I am working with, test NETCONF notifications etc... and now I can and want to share my progress as I work my way through adding functionality to this tool.
 
 Here are the reasons for the required modules:
@@ -173,7 +166,40 @@
            </isis>     
          </protocol>    
        </protocols>   
      </network-instance>  
    </network-instances> 
  </data>
 ```
+
+### netconf-tool operations get-yang-models
+
+Gathers all YANG models present on the NETCONF server and saves them by default to `./yang_models`
+
+```
+$ netconf-tool operations get-yang-models --host 192.0.2.1
+2023-05-01 08:34:24.603 | INFO     | netconf_tool.operations.get_yang:cli_operations_get_yang_models:36 - Attempting to establish NETCONF session to 192.0.2.1:830
+2023-05-01 08:34:24.965 | SUCCESS  | netconf_tool.operations.get_yang:cli_operations_get_yang_models:46 - Established NETCONF connection to 192.0.2.1:830 (Session ID: 164)
+2023-05-01 08:34:49.831 | SUCCESS  | netconf_tool.operations.get_yang:cli_operations_get_yang_models:62 - Exported module nc-notifications (yang_models/nc-notifications.yang)
+2023-05-01 08:34:49.938 | SUCCESS  | netconf_tool.operations.get_yang:cli_operations_get_yang_models:62 - Exported module notifications (yang_models/notifications.yang)
+2023-05-01 08:34:50.046 | SUCCESS  | netconf_tool.operations.get_yang:cli_operations_get_yang_models:62 - Exported module openconfig-aaa (yang_models/openconfig-aaa.yang)
+2023-05-01 08:34:50.154 | SUCCESS  | netconf_tool.operations.get_yang:cli_operations_get_yang_models:62 - Exported module openconfig-aaa-types (yang_models/openconfig-aaa-types.yang)
+2023-05-01 08:34:50.262 | SUCCESS  | netconf_tool.operations.get_yang:cli_operations_get_yang_models:62 - Exported module openconfig-acl (yang_models/openconfig-acl.yang)
+2023-05-01 08:34:50.369 | SUCCESS  | netconf_tool.operations.get_yang:cli_operations_get_yang_models:62 - Exported module openconfig-aft (yang_models/openconfig-aft.yang)
+2023-05-01 08:34:50.476 | SUCCESS  | netconf_tool.operations.get_yang:cli_operations_get_yang_models:62 - Exported module openconfig-aft-types (yang_models/openconfig-aft-types.yang)
+2023-05-01 08:34:50.583 | SUCCESS  | netconf_tool.operations.get_yang:cli_operations_get_yang_models:62 - Exported module openconfig-alarm-types (yang_models/openconfig-alarm-types.yang)
+2023-05-01 08:34:50.690 | SUCCESS  | netconf_tool.operations.get_yang:cli_operations_get_yang_models:62 - Exported module openconfig-alarms (yang_models/openconfig-alarms.yang)
+............. and so on .............
+2023-05-01 08:37:21.411 | SUCCESS  | netconf_tool.operations.get_yang:cli_operations_get_yang_models:76 - Exported a total of 280 YANG models
+```
+
+### netconf-tool operations get-yang-model
+
+Gathers a specific YANG model if it exist on the NETCONF server and saves it by default to `./yang_models`
+
+```
+$ netconf-tool operations get-yang-model --host 192.0.2.1 --name openconfig-segment-routing
+2023-05-01 08:31:21.036 | INFO     | netconf_tool.operations.get_yang:cli_operations_get_yang_model:96 - Creating output directory and any child folders
+2023-05-01 08:31:21.036 | INFO     | netconf_tool.operations.get_yang:cli_operations_get_yang_model:100 - Attempting to establish NETCONF session to 192.0.2.1:830
+2023-05-01 08:31:21.398 | SUCCESS  | netconf_tool.operations.get_yang:cli_operations_get_yang_model:110 - Established NETCONF connection to 192.0.2.1:830 (Session ID: 162)
+2023-05-01 08:31:21.508 | SUCCESS  | netconf_tool.operations.get_yang:cli_operations_get_yang_model:134 - Exported module openconfig-segment-routing (yang_models/openconfig-segment-routing.yang)
+```
```

### Comparing `netconf_tool-0.0.2/README.md` & `netconf_tool-0.0.3/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+Metadata-Version: 2.1
+Name: netconf_tool
+Version: 0.0.3
+Summary: Click CLI application to help with NETCONF development experience
+Home-page: https://github.com/BSpendlove/netconf-tool
+Description-Content-Type: text/markdown
+
 # netconf-tool
 
 This is a tool aimed for developer experience / making things faster when I am trying to test NETCONF related tasks without having to rewrite a random python script. I've found myself constantly writing little python scripts for NETCONF to test functionality or even grab data such as server capabilities, setup event based notifications/subscription to test something and have probably got 100 scripts that do the same thing in different folders through the various projects I've worked on.
 
 Therefore I've created this tool to improve my developer experience working with NETCONF. At the ease of a quick command, I want to be able to get config, try out some edit-config functionality, grab capabilities of a new vendor I am working with, test NETCONF notifications etc... and now I can and want to share my progress as I work my way through adding functionality to this tool.
 
 Here are the reasons for the required modules:
@@ -165,8 +172,41 @@
              </global>      
            </isis>     
          </protocol>    
        </protocols>   
      </network-instance>  
    </network-instances> 
  </data>
-```
+```
+
+### netconf-tool operations get-yang-models
+
+Gathers all YANG models present on the NETCONF server and saves them by default to `./yang_models`
+
+```
+$ netconf-tool operations get-yang-models --host 192.0.2.1
+2023-05-01 08:34:24.603 | INFO     | netconf_tool.operations.get_yang:cli_operations_get_yang_models:36 - Attempting to establish NETCONF session to 192.0.2.1:830
+2023-05-01 08:34:24.965 | SUCCESS  | netconf_tool.operations.get_yang:cli_operations_get_yang_models:46 - Established NETCONF connection to 192.0.2.1:830 (Session ID: 164)
+2023-05-01 08:34:49.831 | SUCCESS  | netconf_tool.operations.get_yang:cli_operations_get_yang_models:62 - Exported module nc-notifications (yang_models/nc-notifications.yang)
+2023-05-01 08:34:49.938 | SUCCESS  | netconf_tool.operations.get_yang:cli_operations_get_yang_models:62 - Exported module notifications (yang_models/notifications.yang)
+2023-05-01 08:34:50.046 | SUCCESS  | netconf_tool.operations.get_yang:cli_operations_get_yang_models:62 - Exported module openconfig-aaa (yang_models/openconfig-aaa.yang)
+2023-05-01 08:34:50.154 | SUCCESS  | netconf_tool.operations.get_yang:cli_operations_get_yang_models:62 - Exported module openconfig-aaa-types (yang_models/openconfig-aaa-types.yang)
+2023-05-01 08:34:50.262 | SUCCESS  | netconf_tool.operations.get_yang:cli_operations_get_yang_models:62 - Exported module openconfig-acl (yang_models/openconfig-acl.yang)
+2023-05-01 08:34:50.369 | SUCCESS  | netconf_tool.operations.get_yang:cli_operations_get_yang_models:62 - Exported module openconfig-aft (yang_models/openconfig-aft.yang)
+2023-05-01 08:34:50.476 | SUCCESS  | netconf_tool.operations.get_yang:cli_operations_get_yang_models:62 - Exported module openconfig-aft-types (yang_models/openconfig-aft-types.yang)
+2023-05-01 08:34:50.583 | SUCCESS  | netconf_tool.operations.get_yang:cli_operations_get_yang_models:62 - Exported module openconfig-alarm-types (yang_models/openconfig-alarm-types.yang)
+2023-05-01 08:34:50.690 | SUCCESS  | netconf_tool.operations.get_yang:cli_operations_get_yang_models:62 - Exported module openconfig-alarms (yang_models/openconfig-alarms.yang)
+............. and so on .............
+2023-05-01 08:37:21.411 | SUCCESS  | netconf_tool.operations.get_yang:cli_operations_get_yang_models:76 - Exported a total of 280 YANG models
+```
+
+### netconf-tool operations get-yang-model
+
+Gathers a specific YANG model if it exist on the NETCONF server and saves it by default to `./yang_models`
+
+```
+$ netconf-tool operations get-yang-model --host 192.0.2.1 --name openconfig-segment-routing
+2023-05-01 08:31:21.036 | INFO     | netconf_tool.operations.get_yang:cli_operations_get_yang_model:96 - Creating output directory and any child folders
+2023-05-01 08:31:21.036 | INFO     | netconf_tool.operations.get_yang:cli_operations_get_yang_model:100 - Attempting to establish NETCONF session to 192.0.2.1:830
+2023-05-01 08:31:21.398 | SUCCESS  | netconf_tool.operations.get_yang:cli_operations_get_yang_model:110 - Established NETCONF connection to 192.0.2.1:830 (Session ID: 162)
+2023-05-01 08:31:21.508 | SUCCESS  | netconf_tool.operations.get_yang:cli_operations_get_yang_model:134 - Exported module openconfig-segment-routing (yang_models/openconfig-segment-routing.yang)
+```
```

### Comparing `netconf_tool-0.0.2/netconf_tool/decorators.py` & `netconf_tool-0.0.3/netconf_tool/decorators.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,14 +36,17 @@
         "--port",
         help="Port of NETCONF Server to connect to",
         type=int,
         default=830,
         required=True,
     )
     @click.option(
+        "--timeout", help="SSH socket connection timeout", type=int, default=10
+    )
+    @click.option(
         "--username",
         help="Username to authenticate to NETCONF Server",
         envvar="NETCONF_TOOL_USERNAME",
     )
     @click.option(
         "--password",
         help="Password to authenticate to NETCONF Server",
```

### Comparing `netconf_tool-0.0.2/netconf_tool/helpers.py` & `netconf_tool-0.0.3/netconf_tool/helpers.py`

 * *Files identical despite different names*

### Comparing `netconf_tool-0.0.2/netconf_tool/operations/capabilities.py` & `netconf_tool-0.0.3/netconf_tool/operations/capabilities.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,26 +15,28 @@
     "--export-json",
     help="Export server capabilities into RFC3986 compliant URIs into a JSON file",
     type=str,
 )
 def netconf_tool_cli_operations_list_server_capabilities(
     host: str,
     port: int,
+    timout: int,
     username: str,
     password: str,
     device_handler: str,
     hostkey_verify: bool,
     export_json: str,
 ):
     """Print or Export all NETCONF Server capabilities"""
     logger.info(f"Attempting to establish NETCONF session to {host}:{port}")
     try:
         with manager.connect(
             host=host,
             port=port,
+            timeout=timeout,
             username=username,
             password=password,
             device_params={"name": device_handler},
             hostkey_verify=hostkey_verify,
         ) as m:
             logger.success(
                 f"Established NETCONF connection to {host}:{port} (Session ID: {m.session_id})"
```

### Comparing `netconf_tool-0.0.2/netconf_tool/operations/get_config.py` & `netconf_tool-0.0.3/netconf_tool/yangcli/get_config.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,101 +1,94 @@
 import click
-import xmltodict
 import json
-from xml.dom import minidom
-from xml.etree import ElementTree
-from xml.etree.ElementTree import ParseError
+import xmltodict
 from ncclient import manager
 from ncclient.transport.errors import SSHError, AuthenticationError
 from loguru import logger
-
-from netconf_tool.operations import netconf_tool_cli_operations
+from xml.dom import minidom
+from netconf_tool.yangcli import netconf_tool_cli_yangcli
 from netconf_tool.decorators import common_format_options, common_netconf_options
+from netconf_tool.helpers import build_xml_from_cli_commands
 
 
-@netconf_tool_cli_operations.command("get-config")
+@netconf_tool_cli_yangcli.command("get-config")
 @common_netconf_options
 @common_format_options
+@click.argument("command")
 @click.option(
     "--datastore",
     help="Specify which datastore to retrieve configuration from",
     type=click.Choice(["running", "candidate"]),
     default="running",
 )
-@click.option(
-    "--filter", help="Include an XML filter to filter get-config operation", type=str
-)
-def cli_operations_get_config(
+def netconf_tool_cli_yangcli_get_config(
     host: str,
     port: int,
+    timeout: int,
     username: str,
     password: str,
     device_handler: str,
     hostkey_verify: bool,
+    command: str,
     datastore: str,
-    filter: str,
     format_json: bool,
     export_xml: str,
     export_json: str,
 ):
-    """Subscribes to notifications/events in real-time and prints them to the screen for debugging/troubleshooting"""
-    if filter:
-        logger.debug("Performing some basic XML validation")
-        try:
-            ElementTree.fromstring(filter)
-        except ParseError as err:
-            logger.error(f"Parsing error detected with --filter: {err}")
-            exit()
+    """Print or Export all NETCONF Server capabilities - note this command does not perform any validation and is just a test"""
+    filter = build_xml_from_cli_commands(command)
+    if not filter:
+        logger.error("Unable to build XML filter")
+        exit()
 
+    logger.debug(f"Filter that will be used for get-config: {filter}")
     logger.info(f"Attempting to establish NETCONF session to {host}:{port}")
+
     try:
         with manager.connect(
             host=host,
             port=port,
+            timeout=timeout,
             username=username,
             password=password,
             device_params={"name": device_handler},
             hostkey_verify=hostkey_verify,
         ) as m:
             logger.success(
                 f"Established NETCONF connection to {host}:{port} (Session ID: {m.session_id})"
             )
-            if filter:
-                configuration = m.get_config(
-                    source=datastore, filter=("subtree", filter)
+            configuration = m.get_config(source=datastore, filter=("subtree", filter))
+            xml_data = minidom.parseString(configuration.data_xml).toprettyxml(
+                indent=" ", newl=""
+            )
+
+            if export_xml:
+                with open(export_xml, "w") as out_file:
+                    out_file.write(xml_data)
+                logger.success(
+                    f"Exported get-config operation to {export_xml} in XML format"
                 )
-            else:
-                configuration = m.get_config(source=datastore)
-    except SSHError as err:
-        logger.error(err)
-        exit()
-    except AuthenticationError as err:
-        logger.error("Unable to authenticate to NETCONF server")
-        exit()
-    except Exception as err:
-        logger.error(f"Generic Exception caught: {err}")
-        exit()
+                exit()
 
-    xml_data = minidom.parseString(configuration.data_xml).toprettyxml(
-        indent=" ", newl=""
-    )
-
-    if export_xml:
-        with open(export_xml, "w") as out_file:
-            out_file.write(xml_data)
-        logger.success(f"Exported get-config operation to {export_xml} in XML format")
-        exit()
+            if export_json:
+                json_data = xmltodict.parse(xml_data)
 
-    if export_json:
-        json_data = xmltodict.parse(xml_data)
+                with open(export_json, "w") as out_file:
+                    json.dump(json_data, out_file, indent=4)
 
-        with open(export_json, "w") as out_file:
-            json.dump(json_data, out_file, indent=4)
+                logger.success(
+                    f"Exported get-config operation to {export_json} in JSON format"
+                )
+                exit()
 
-        logger.success(f"Exported get-config operation to {export_json} in JSON format")
-        exit()
+            if format_json:
+                json_data = xmltodict.parse(xml_data)
+                exit(json.dumps(json_data, indent=4))
 
-    if format_json:
-        json_data = xmltodict.parse(xml_data)
-        exit(json.dumps(json_data, indent=4))
+            exit(xml_data)
 
-    exit(xml_data)
+    except SSHError as err:
+        logger.error(err)
+    except AuthenticationError as err:
+        logger.error("Unable to authenticate to NETCONF server")
+    except Exception as err:
+        logger.error(f"Generic Exception caught: {err}")
```

### Comparing `netconf_tool-0.0.2/netconf_tool/subscription/local.py` & `netconf_tool-0.0.3/netconf_tool/subscription/local.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,25 +6,27 @@
 
 
 @netconf_tool_cli_subscription.command("local")
 @common_netconf_options
 def cli_subscription_local(
     host: str,
     port: int,
+    timeout: int,
     username: str,
     password: str,
     device_handler: str,
     hostkey_verify: bool,
 ):
     """Create a local event listener using <create-subscription> which will simply print out the events to the CLI"""
     logger.info(f"Attempting to establish NETCONF session to {host}:{port}")
     try:
         with manager.connect(
             host=host,
             port=port,
+            timeout=timeout,
             username=username,
             password=password,
             device_params={"name": device_handler},
             hostkey_verify=hostkey_verify,
         ) as m:
             logger.success(
                 f"Established NETCONF connection to {host}:{port} (Session ID: {m.session_id})"
```

### Comparing `netconf_tool-0.0.2/netconf_tool/subscription/rabbitmq.py` & `netconf_tool-0.0.3/netconf_tool/subscription/rabbitmq.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,14 +41,15 @@
     "--rabbitmq-password",
     help="Password to authenticate if authentication is used",
     type=str,
 )
 def cli_subscription_rabbitmq(
     host: str,
     port: int,
+    timeout: int,
     username: str,
     password: str,
     device_handler: str,
     hostkey_verify: bool,
     rabbitmq_host: str,
     rabbitmq_port: int,
     rabbitmq_queue: str,
@@ -80,14 +81,15 @@
     )
 
     logger.info(f"Attempting to establish NETCONF session to {host}:{port}")
     try:
         with manager.connect(
             host=host,
             port=port,
+            timeout=timeout,
             username=username,
             password=password,
             device_params={"name": device_handler},
             hostkey_verify=hostkey_verify,
         ) as m:
             logger.success(
                 f"Established NETCONF connection to {host}:{port} (Session ID: {m.session_id})"
```

### Comparing `netconf_tool-0.0.2/netconf_tool/subscription/redis.py` & `netconf_tool-0.0.3/netconf_tool/subscription/redis.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     help="Channel to publish message to",
     type=str,
     default="netconf_tool:all_events",
 )
 def cli_subscription_redis_pubsub(
     host: str,
     port: int,
+    timeout: int,
     username: str,
     password: str,
     device_handler: str,
     hostkey_verify: bool,
     redis_host: str,
     redis_port: int,
     redis_channel: str,
@@ -43,14 +44,15 @@
 
     logger.info(f"Attempting to establish NETCONF session to {host}:{port}")
 
     try:
         with manager.connect(
             host=host,
             port=port,
+            timeout=timeout,
             username=username,
             password=password,
             device_params={"name": device_handler},
             hostkey_verify=hostkey_verify,
         ) as m:
             logger.success(
                 f"Established NETCONF connection to {host}:{port} (Session ID: {m.session_id})"
```

### Comparing `netconf_tool-0.0.2/netconf_tool.egg-info/PKG-INFO` & `netconf_tool-0.0.3/netconf_tool.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netconf-tool
-Version: 0.0.2
+Version: 0.0.3
 Summary: Click CLI application to help with NETCONF development experience
 Home-page: https://github.com/BSpendlove/netconf-tool
 Description-Content-Type: text/markdown
 
 # netconf-tool
 
 This is a tool aimed for developer experience / making things faster when I am trying to test NETCONF related tasks without having to rewrite a random python script. I've found myself constantly writing little python scripts for NETCONF to test functionality or even grab data such as server capabilities, setup event based notifications/subscription to test something and have probably got 100 scripts that do the same thing in different folders through the various projects I've worked on.
@@ -173,7 +173,40 @@
            </isis>     
          </protocol>    
        </protocols>   
      </network-instance>  
    </network-instances> 
  </data>
 ```
+
+### netconf-tool operations get-yang-models
+
+Gathers all YANG models present on the NETCONF server and saves them by default to `./yang_models`
+
+```
+$ netconf-tool operations get-yang-models --host 192.0.2.1
+2023-05-01 08:34:24.603 | INFO     | netconf_tool.operations.get_yang:cli_operations_get_yang_models:36 - Attempting to establish NETCONF session to 192.0.2.1:830
+2023-05-01 08:34:24.965 | SUCCESS  | netconf_tool.operations.get_yang:cli_operations_get_yang_models:46 - Established NETCONF connection to 192.0.2.1:830 (Session ID: 164)
+2023-05-01 08:34:49.831 | SUCCESS  | netconf_tool.operations.get_yang:cli_operations_get_yang_models:62 - Exported module nc-notifications (yang_models/nc-notifications.yang)
+2023-05-01 08:34:49.938 | SUCCESS  | netconf_tool.operations.get_yang:cli_operations_get_yang_models:62 - Exported module notifications (yang_models/notifications.yang)
+2023-05-01 08:34:50.046 | SUCCESS  | netconf_tool.operations.get_yang:cli_operations_get_yang_models:62 - Exported module openconfig-aaa (yang_models/openconfig-aaa.yang)
+2023-05-01 08:34:50.154 | SUCCESS  | netconf_tool.operations.get_yang:cli_operations_get_yang_models:62 - Exported module openconfig-aaa-types (yang_models/openconfig-aaa-types.yang)
+2023-05-01 08:34:50.262 | SUCCESS  | netconf_tool.operations.get_yang:cli_operations_get_yang_models:62 - Exported module openconfig-acl (yang_models/openconfig-acl.yang)
+2023-05-01 08:34:50.369 | SUCCESS  | netconf_tool.operations.get_yang:cli_operations_get_yang_models:62 - Exported module openconfig-aft (yang_models/openconfig-aft.yang)
+2023-05-01 08:34:50.476 | SUCCESS  | netconf_tool.operations.get_yang:cli_operations_get_yang_models:62 - Exported module openconfig-aft-types (yang_models/openconfig-aft-types.yang)
+2023-05-01 08:34:50.583 | SUCCESS  | netconf_tool.operations.get_yang:cli_operations_get_yang_models:62 - Exported module openconfig-alarm-types (yang_models/openconfig-alarm-types.yang)
+2023-05-01 08:34:50.690 | SUCCESS  | netconf_tool.operations.get_yang:cli_operations_get_yang_models:62 - Exported module openconfig-alarms (yang_models/openconfig-alarms.yang)
+............. and so on .............
+2023-05-01 08:37:21.411 | SUCCESS  | netconf_tool.operations.get_yang:cli_operations_get_yang_models:76 - Exported a total of 280 YANG models
+```
+
+### netconf-tool operations get-yang-model
+
+Gathers a specific YANG model if it exist on the NETCONF server and saves it by default to `./yang_models`
+
+```
+$ netconf-tool operations get-yang-model --host 192.0.2.1 --name openconfig-segment-routing
+2023-05-01 08:31:21.036 | INFO     | netconf_tool.operations.get_yang:cli_operations_get_yang_model:96 - Creating output directory and any child folders
+2023-05-01 08:31:21.036 | INFO     | netconf_tool.operations.get_yang:cli_operations_get_yang_model:100 - Attempting to establish NETCONF session to 192.0.2.1:830
+2023-05-01 08:31:21.398 | SUCCESS  | netconf_tool.operations.get_yang:cli_operations_get_yang_model:110 - Established NETCONF connection to 192.0.2.1:830 (Session ID: 162)
+2023-05-01 08:31:21.508 | SUCCESS  | netconf_tool.operations.get_yang:cli_operations_get_yang_model:134 - Exported module openconfig-segment-routing (yang_models/openconfig-segment-routing.yang)
+```
```

### Comparing `netconf_tool-0.0.2/netconf_tool.egg-info/SOURCES.txt` & `netconf_tool-0.0.3/netconf_tool.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -9,13 +9,14 @@
 netconf_tool.egg-info/dependency_links.txt
 netconf_tool.egg-info/entry_points.txt
 netconf_tool.egg-info/requires.txt
 netconf_tool.egg-info/top_level.txt
 netconf_tool/operations/__init__.py
 netconf_tool/operations/capabilities.py
 netconf_tool/operations/get_config.py
+netconf_tool/operations/get_yang.py
 netconf_tool/subscription/__init__.py
 netconf_tool/subscription/local.py
 netconf_tool/subscription/rabbitmq.py
 netconf_tool/subscription/redis.py
 netconf_tool/yangcli/__init__.py
 netconf_tool/yangcli/get_config.py
```

### Comparing `netconf_tool-0.0.2/setup.py` & `netconf_tool-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name="netconf_tool",
-    version="0.0.2",
+    version="0.0.3",
     packages=find_packages(exclude=("dev")),
     include_package_data=True,
     description="Click CLI application to help with NETCONF development experience",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/BSpendlove/netconf-tool",
     install_requires=[
```

