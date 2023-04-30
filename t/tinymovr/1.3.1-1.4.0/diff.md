# Comparing `tmp/tinymovr-1.3.1.tar.gz` & `tmp/tinymovr-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinymovr-1.3.1.tar", last modified: Thu Apr 20 17:25:49 2023, max compression
+gzip compressed data, was "tinymovr-1.4.0.tar", last modified: Sun Apr 30 22:59:46 2023, max compression
```

## Comparing `tinymovr-1.3.1.tar` & `tinymovr-1.4.0.tar`

### file list

```diff
@@ -1,38 +1,43 @@
-drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-04-20 17:25:49.371284 tinymovr-1.3.1/
--rw-r--r--   0 yanconst   (501) staff       (20)      185 2023-04-20 17:24:50.000000 tinymovr-1.3.1/MANIFEST.in
--rw-r--r--   0 yanconst   (501) staff       (20)     2144 2023-04-20 17:25:49.371103 tinymovr-1.3.1/PKG-INFO
--rw-r--r--   0 yanconst   (501) staff       (20)     1689 2023-04-08 07:47:15.000000 tinymovr-1.3.1/README.md
--rw-r--r--   0 yanconst   (501) staff       (20)       38 2023-04-20 17:25:49.371333 tinymovr-1.3.1/setup.cfg
--rw-r--r--   0 yanconst   (501) staff       (20)     2334 2023-04-17 16:47:58.000000 tinymovr-1.3.1/setup.py
-drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-04-20 17:25:49.367184 tinymovr-1.3.1/tinymovr/
--rw-r--r--   0 yanconst   (501) staff       (20)       55 2023-04-08 07:47:15.000000 tinymovr-1.3.1/tinymovr/__init__.py
--rw-r--r--   0 yanconst   (501) staff       (20)     3529 2023-04-08 07:47:15.000000 tinymovr-1.3.1/tinymovr/channel.py
--rw-r--r--   0 yanconst   (501) staff       (20)     2845 2023-04-20 17:24:50.000000 tinymovr-1.3.1/tinymovr/cli.py
-drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-04-20 17:25:49.368698 tinymovr-1.3.1/tinymovr/codec/
--rw-r--r--   0 yanconst   (501) staff       (20)       65 2022-02-09 17:27:03.000000 tinymovr-1.3.1/tinymovr/codec/__init__.py
--rw-r--r--   0 yanconst   (501) staff       (20)     2944 2023-04-08 07:47:15.000000 tinymovr-1.3.1/tinymovr/codec/codec.py
-drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-04-20 17:25:49.369262 tinymovr-1.3.1/tinymovr/config/
--rw-r--r--   0 yanconst   (501) staff       (20)      160 2023-04-08 07:47:15.000000 tinymovr-1.3.1/tinymovr/config/__init__.py
--rw-r--r--   0 yanconst   (501) staff       (20)     3358 2023-04-08 07:47:15.000000 tinymovr-1.3.1/tinymovr/config/config.py
--rw-r--r--   0 yanconst   (501) staff       (20)    15484 2023-04-08 07:47:15.000000 tinymovr-1.3.1/tinymovr/config/device.yaml
--rw-r--r--   0 yanconst   (501) staff       (20)     1075 2023-04-08 07:47:15.000000 tinymovr-1.3.1/tinymovr/constants.py
--rw-r--r--   0 yanconst   (501) staff       (20)     3292 2023-04-08 07:47:15.000000 tinymovr-1.3.1/tinymovr/discovery.py
-drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-04-20 17:25:49.370190 tinymovr-1.3.1/tinymovr/gui/
--rw-r--r--   0 yanconst   (501) staff       (20)      431 2023-04-20 17:24:50.000000 tinymovr-1.3.1/tinymovr/gui/__init__.py
--rw-r--r--   0 yanconst   (501) staff       (20)     1582 2023-04-20 17:24:50.000000 tinymovr-1.3.1/tinymovr/gui/gui.py
--rw-r--r--   0 yanconst   (501) staff       (20)     9660 2023-04-20 17:24:50.000000 tinymovr-1.3.1/tinymovr/gui/helpers.py
--rw-r--r--   0 yanconst   (501) staff       (20)    12203 2023-04-20 17:24:50.000000 tinymovr-1.3.1/tinymovr/gui/window.py
--rw-r--r--   0 yanconst   (501) staff       (20)     4472 2023-04-17 16:47:58.000000 tinymovr-1.3.1/tinymovr/gui/worker.py
-drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-04-20 17:25:49.365294 tinymovr-1.3.1/tinymovr/resources/
-drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-04-20 17:25:49.370838 tinymovr-1.3.1/tinymovr/resources/icons/
--rw-r--r--   0 yanconst   (501) staff       (20)     3184 2023-04-20 17:24:50.000000 tinymovr-1.3.1/tinymovr/resources/icons/call.png
--rw-r--r--   0 yanconst   (501) staff       (20)    12497 2023-04-20 17:24:50.000000 tinymovr-1.3.1/tinymovr/resources/icons/empty.png
--rw-r--r--   0 yanconst   (501) staff       (20)    30143 2023-04-20 17:24:50.000000 tinymovr-1.3.1/tinymovr/resources/icons/empty@2x.png
--rw-r--r--   0 yanconst   (501) staff       (20)     3088 2023-04-08 07:47:15.000000 tinymovr-1.3.1/tinymovr/tee.py
-drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-04-20 17:25:49.368297 tinymovr-1.3.1/tinymovr.egg-info/
--rw-r--r--   0 yanconst   (501) staff       (20)     2144 2023-04-20 17:25:49.000000 tinymovr-1.3.1/tinymovr.egg-info/PKG-INFO
--rw-r--r--   0 yanconst   (501) staff       (20)      696 2023-04-20 17:25:49.000000 tinymovr-1.3.1/tinymovr.egg-info/SOURCES.txt
--rw-r--r--   0 yanconst   (501) staff       (20)        1 2023-04-20 17:25:49.000000 tinymovr-1.3.1/tinymovr.egg-info/dependency_links.txt
--rw-r--r--   0 yanconst   (501) staff       (20)       82 2023-04-20 17:25:49.000000 tinymovr-1.3.1/tinymovr.egg-info/entry_points.txt
--rw-r--r--   0 yanconst   (501) staff       (20)      166 2023-04-20 17:25:49.000000 tinymovr-1.3.1/tinymovr.egg-info/requires.txt
--rw-r--r--   0 yanconst   (501) staff       (20)        9 2023-04-20 17:25:49.000000 tinymovr-1.3.1/tinymovr.egg-info/top_level.txt
+drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-04-30 22:59:46.446589 tinymovr-1.4.0/
+-rw-r--r--   0 yanconst   (501) staff       (20)      426 2023-04-29 08:24:21.000000 tinymovr-1.4.0/MANIFEST.in
+-rw-r--r--   0 yanconst   (501) staff       (20)     2144 2023-04-30 22:59:46.446398 tinymovr-1.4.0/PKG-INFO
+-rw-r--r--   0 yanconst   (501) staff       (20)     1689 2023-04-08 07:47:15.000000 tinymovr-1.4.0/README.md
+-rw-r--r--   0 yanconst   (501) staff       (20)       38 2023-04-30 22:59:46.446637 tinymovr-1.4.0/setup.cfg
+-rw-r--r--   0 yanconst   (501) staff       (20)     2334 2023-04-17 16:47:58.000000 tinymovr-1.4.0/setup.py
+drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-04-30 22:59:46.439984 tinymovr-1.4.0/tinymovr/
+-rw-r--r--   0 yanconst   (501) staff       (20)       55 2023-04-08 07:47:15.000000 tinymovr-1.4.0/tinymovr/__init__.py
+-rw-r--r--   0 yanconst   (501) staff       (20)     3489 2023-04-27 23:25:49.000000 tinymovr-1.4.0/tinymovr/channel.py
+-rw-r--r--   0 yanconst   (501) staff       (20)     2845 2023-04-20 17:24:50.000000 tinymovr-1.4.0/tinymovr/cli.py
+drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-04-30 22:59:46.441827 tinymovr-1.4.0/tinymovr/codec/
+-rw-r--r--   0 yanconst   (501) staff       (20)       65 2022-02-09 17:27:03.000000 tinymovr-1.4.0/tinymovr/codec/__init__.py
+-rw-r--r--   0 yanconst   (501) staff       (20)     2944 2023-04-08 07:47:15.000000 tinymovr-1.4.0/tinymovr/codec/codec.py
+drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-04-30 22:59:46.442477 tinymovr-1.4.0/tinymovr/config/
+-rw-r--r--   0 yanconst   (501) staff       (20)      160 2023-04-08 07:47:15.000000 tinymovr-1.4.0/tinymovr/config/__init__.py
+-rw-r--r--   0 yanconst   (501) staff       (20)     4111 2023-04-30 22:31:52.000000 tinymovr-1.4.0/tinymovr/config/config.py
+-rw-r--r--   0 yanconst   (501) staff       (20)    16329 2023-04-30 22:31:52.000000 tinymovr-1.4.0/tinymovr/config/device.yaml
+-rw-r--r--   0 yanconst   (501) staff       (20)     1075 2023-04-08 07:47:15.000000 tinymovr-1.4.0/tinymovr/constants.py
+-rw-r--r--   0 yanconst   (501) staff       (20)     3292 2023-04-08 07:47:15.000000 tinymovr-1.4.0/tinymovr/discovery.py
+drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-04-30 22:59:46.443733 tinymovr-1.4.0/tinymovr/gui/
+-rw-r--r--   0 yanconst   (501) staff       (20)      474 2023-04-29 08:24:21.000000 tinymovr-1.4.0/tinymovr/gui/__init__.py
+-rw-r--r--   0 yanconst   (501) staff       (20)     1701 2023-04-29 08:24:21.000000 tinymovr-1.4.0/tinymovr/gui/gui.py
+-rw-r--r--   0 yanconst   (501) staff       (20)    14256 2023-04-29 08:24:21.000000 tinymovr-1.4.0/tinymovr/gui/helpers.py
+-rw-r--r--   0 yanconst   (501) staff       (20)    12941 2023-04-29 08:24:21.000000 tinymovr-1.4.0/tinymovr/gui/window.py
+-rw-r--r--   0 yanconst   (501) staff       (20)     4472 2023-04-17 16:47:58.000000 tinymovr-1.4.0/tinymovr/gui/worker.py
+drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-04-30 22:59:46.437887 tinymovr-1.4.0/tinymovr/resources/
+drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-04-30 22:59:46.445968 tinymovr-1.4.0/tinymovr/resources/icons/
+-rw-r--r--   0 yanconst   (501) staff       (20)     3184 2023-04-20 17:24:50.000000 tinymovr-1.4.0/tinymovr/resources/icons/call.png
+-rw-r--r--   0 yanconst   (501) staff       (20)     3184 2023-04-29 08:24:21.000000 tinymovr-1.4.0/tinymovr/resources/icons/call@2x.png
+-rw-r--r--   0 yanconst   (501) staff       (20)    22790 2023-04-29 08:24:21.000000 tinymovr-1.4.0/tinymovr/resources/icons/call_dark.png
+-rw-r--r--   0 yanconst   (501) staff       (20)    22672 2023-04-29 08:24:21.000000 tinymovr-1.4.0/tinymovr/resources/icons/call_dark@2x.png
+-rw-r--r--   0 yanconst   (501) staff       (20)    26604 2023-04-29 08:24:21.000000 tinymovr-1.4.0/tinymovr/resources/icons/empty.png
+-rw-r--r--   0 yanconst   (501) staff       (20)    44831 2023-04-29 08:24:21.000000 tinymovr-1.4.0/tinymovr/resources/icons/empty@2x.png
+-rw-r--r--   0 yanconst   (501) staff       (20)    30381 2023-04-29 08:24:21.000000 tinymovr-1.4.0/tinymovr/resources/icons/empty_dark.png
+-rw-r--r--   0 yanconst   (501) staff       (20)    51206 2023-04-29 08:24:21.000000 tinymovr-1.4.0/tinymovr/resources/icons/empty_dark@2x.png
+-rw-r--r--   0 yanconst   (501) staff       (20)     3343 2023-04-29 08:24:21.000000 tinymovr-1.4.0/tinymovr/tee.py
+drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-04-30 22:59:46.441476 tinymovr-1.4.0/tinymovr.egg-info/
+-rw-r--r--   0 yanconst   (501) staff       (20)     2144 2023-04-30 22:59:46.000000 tinymovr-1.4.0/tinymovr.egg-info/PKG-INFO
+-rw-r--r--   0 yanconst   (501) staff       (20)      897 2023-04-30 22:59:46.000000 tinymovr-1.4.0/tinymovr.egg-info/SOURCES.txt
+-rw-r--r--   0 yanconst   (501) staff       (20)        1 2023-04-30 22:59:46.000000 tinymovr-1.4.0/tinymovr.egg-info/dependency_links.txt
+-rw-r--r--   0 yanconst   (501) staff       (20)       82 2023-04-30 22:59:46.000000 tinymovr-1.4.0/tinymovr.egg-info/entry_points.txt
+-rw-r--r--   0 yanconst   (501) staff       (20)      166 2023-04-30 22:59:46.000000 tinymovr-1.4.0/tinymovr.egg-info/requires.txt
+-rw-r--r--   0 yanconst   (501) staff       (20)        9 2023-04-30 22:59:46.000000 tinymovr-1.4.0/tinymovr.egg-info/top_level.txt
```

### Comparing `tinymovr-1.3.1/PKG-INFO` & `tinymovr-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinymovr
-Version: 1.3.1
+Version: 1.4.0
 Summary: Tinymovr Studio
 Home-page: https://github.com/yconst/Tinymovr
 Author: Yannis Chatzikonstantinou
 Author-email: info@tinymovr.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `tinymovr-1.3.1/README.md` & `tinymovr-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `tinymovr-1.3.1/setup.py` & `tinymovr-1.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `tinymovr-1.3.1/tinymovr/channel.py` & `tinymovr-1.4.0/tinymovr/channel.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,16 +55,15 @@
 
     def send(self, data, ep_id):
         rtr = False if data and len(data) else True
         get_tee().send(self.create_frame(ep_id, rtr, data))
 
     def recv(self, ep_id, timeout=1.0):
         with self.lock:
-            if not self.evt.wait(timeout=timeout):
-                print("missed")
+            self.evt.wait(timeout=timeout)
             self.evt.clear()
             frame_id = arbitration_from_ids(ep_id, 0, self.node_id)
             index = 0
             while index < len(self.queue):
                 if self.queue[index].arbitration_id == frame_id:
                     return self.queue.pop(index).data
                 index += 1
```

### Comparing `tinymovr-1.3.1/tinymovr/cli.py` & `tinymovr-1.4.0/tinymovr/cli.py`

 * *Files identical despite different names*

### Comparing `tinymovr-1.3.1/tinymovr/codec/codec.py` & `tinymovr-1.4.0/tinymovr/codec/codec.py`

 * *Files identical despite different names*

### Comparing `tinymovr-1.3.1/tinymovr/config/config.py` & `tinymovr-1.4.0/tinymovr/config/config.py`

 * *Files 17% similar despite different names*

```diff
@@ -28,18 +28,22 @@
 
 def_path_str = str(files("tinymovr").joinpath("config/device.yaml"))
 with open(def_path_str) as dev_def_raw:
     dev_def = yaml.safe_load(dev_def_raw)
 
 
 class ProtocolVersionError(Exception):
-    def __init__(self, *args, **kwargs):
+    def __init__(self, dev_id, version_str, *args, **kwargs):
+        self.dev_id = dev_id
+        self.version_str = cleanup_incomplete_version(version_str)
         msg = (
-            "Incompatible protocol versions (hash mismatch)."
-            "Please try upgrading firmware & studio to the same version."
+            "Incompatible protocol versions (hash mismatch) for device {}. "
+            "Firmware is compatible with Studio version {}.\n\n"
+            "Either upgrade studio and firmware, or install a compatible Studio version like so:\n\n"
+            "pip3 uninstall tinymovr\npip3 install tinymovr=={}".format(self.dev_id, self.version_str, self.version_str)
         )
         super().__init__(msg, *args, **kwargs)
 
 
 def get_bus_config(suggested_types=None):
     """
     Get the bus configuration (interface, channel) for
@@ -78,22 +82,38 @@
     to decode the actual hash value and id
     """
     node_id = heartbeat_msg.arbitration_id & 0x3F
     chan = CANChannel(node_id)
     node = deserialize(dev_def)
     hash, *_ = chan.serializer.deserialize(heartbeat_msg.data[:4], DataType.UINT32)
     if node.hash_uint32 != hash:  # hash_uint32 is local, hash is remote
-        raise ProtocolVersionError()
+        version_str = "".join(heartbeat_msg.data[4:])
+        if not version_str.strip():
+            version_str = "1.3.1"
+        raise ProtocolVersionError(node_id, version_str)
     node._channel = chan
     return node
 
 
 def configure_logging():
     """
     Configure logging for various modules
     """
     logging.getLogger("can.io.logger").setLevel(logging.WARNING)
     logging.getLogger("parso").setLevel(logging.WARNING)
     logging.getLogger("asyncio").setLevel(logging.WARNING)
     logger = logging.getLogger("tinymovr")
     logger.setLevel(logging.DEBUG)
     return logger
+
+
+def cleanup_incomplete_version(version_str, char='.'):
+    """
+    Clean up any version string that is
+    incomplete or malformed
+    """
+    parts = version_str.split(char)
+    
+    while '' in parts:
+        parts.remove('')
+    
+    return char.join(parts)
```

### Comparing `tinymovr-1.3.1/tinymovr/config/device.yaml` & `tinymovr-1.4.0/tinymovr/config/device.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -383,29 +383,50 @@
     remote_attributes:
       - name: max_accel
         dtype: float
         unit: ticks/s
         meta: {export: True}
         getter_name: planner_get_max_accel
         setter_name: planner_set_max_accel
-        summary: The trajectory planner max acceleration.
+        summary: The max allowed acceleration of the generated trajectory.
       - name: max_decel
         dtype: float
         unit: ticks/second/second
         meta: {export: True}
         getter_name: planner_get_max_decel
         setter_name: planner_set_max_decel
-        summary: The trajectory planner max deceleration.
+        summary: The max allowed deceleration of the generated trajectory.
       - name: max_vel
         dtype: float
         unit: ticks/second
         meta: {export: True}
         getter_name: planner_get_max_vel
         setter_name: planner_set_max_vel
-        summary: The trajectory planner max cruise velocity.
+        summary: The max allowed cruise velocity of the generated trajectory.
+      - name: t_accel
+        dtype: float
+        unit: second
+        meta: {export: True}
+        getter_name: planner_get_deltat_accel
+        setter_name: planner_set_deltat_accel
+        summary: In time mode, the acceleration time of the generated trajectory.
+      - name: t_decel
+        dtype: float
+        unit: second
+        meta: {export: True}
+        getter_name: planner_get_deltat_decel
+        setter_name: planner_set_deltat_decel
+        summary: In time mode, the deceleration time of the generated trajectory.
+      - name: t_total
+        dtype: float
+        unit: second
+        meta: {export: True}
+        getter_name: planner_get_deltat_total
+        setter_name: planner_set_deltat_total
+        summary: In time mode, the total time of the generated trajectory.
       - name: move_to
         summary: Move to target position respecting velocity and acceleration limits.
         caller_name: planner_move_to_vlimit
         dtype: void
         arguments:
           - name: pos_setpoint
             dtype: float
```

### Comparing `tinymovr-1.3.1/tinymovr/constants.py` & `tinymovr-1.4.0/tinymovr/constants.py`

 * *Files identical despite different names*

### Comparing `tinymovr-1.3.1/tinymovr/discovery.py` & `tinymovr-1.4.0/tinymovr/discovery.py`

 * *Files identical despite different names*

### Comparing `tinymovr-1.3.1/tinymovr/gui/gui.py` & `tinymovr-1.4.0/tinymovr/gui/gui.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     --bitrate=<bitrate>  CAN bitrate [default: 1000000].
 """
 
 import sys
 import pkg_resources
 from docopt import docopt
 from PySide6.QtWidgets import QApplication
-from tinymovr.gui import MainWindow, app_stylesheet
+from tinymovr.gui import MainWindow, app_stylesheet, app_stylesheet_dark, is_dark_mode
 from tinymovr.constants import app_name
 
 
 """
 Tinymovr Studio GUI
 Copyright Ioannis Chatzikonstantinou 2020-2023
 
@@ -37,11 +37,14 @@
 """
 
 
 def spawn():
     version = pkg_resources.require("tinymovr")[0].version
     arguments = docopt(__doc__, version=app_name + " " + str(version))
     app = QApplication(sys.argv)
-    app.setStyleSheet(app_stylesheet)
+    if is_dark_mode():
+        app.setStyleSheet(app_stylesheet_dark)
+    else:
+        app.setStyleSheet(app_stylesheet)
     w = MainWindow(app, arguments)
     w.show()
     sys.exit(app.exec_())
```

### Comparing `tinymovr-1.3.1/tinymovr/gui/helpers.py` & `tinymovr-1.4.0/tinymovr/gui/helpers.py`

 * *Files 26% similar despite different names*

```diff
@@ -15,15 +15,17 @@
 this program. If not, see <http://www.gnu.org/licenses/>.
 """
 
 import time
 import os
 import enum
 import pint
+from PySide6.QtCore import Qt
 from PySide6 import QtGui
+from PySide6.QtGui import QPixmap, QIcon, QGuiApplication, QPalette
 from PySide6.QtWidgets import QMessageBox, QFileDialog, QTreeWidget
 from avlos.definitions import RemoteAttribute
 import tinymovr
 
 
 app_stylesheet = """
 
@@ -37,14 +39,166 @@
     QPushButton:pressed {
         background-color: #cdcdcf;
         border-style: inset;
     }
     QPushButton:hover:!pressed
     {
     background-color: #eaeaec;
+    } 
+
+/* --------------------------------------- QScrollBar -----------------------------------*/
+
+    QScrollBar:horizontal
+    {
+        height: 15px;
+        margin: 3px 15px 3px 15px;
+        border: 1px transparent white;
+        border-radius: 4px;
+        background-color: white;
+    }
+
+    QScrollBar::handle:horizontal
+    {
+        background-color: #dfdfe1;      /* #605F5F; */
+        min-width: 5px;
+        border-radius: 4px;
+    }
+
+    QScrollBar::add-line:horizontal
+    {
+        margin: 0px 3px 0px 3px;
+        border-image: url(:/qss_icons/rc/right_arrow_disabled.png);
+        width: 10px;
+        height: 10px;
+        subcontrol-position: right;
+        subcontrol-origin: margin;
+    }
+
+    QScrollBar::sub-line:horizontal
+    {
+        margin: 0px 3px 0px 3px;
+        border-image: url(:/qss_icons/rc/left_arrow_disabled.png);
+        height: 10px;
+        width: 10px;
+        subcontrol-position: left;
+        subcontrol-origin: margin;
+    }
+
+    QScrollBar::add-line:horizontal:hover,QScrollBar::add-line:horizontal:on
+    {
+        border-image: url(:/qss_icons/rc/right_arrow.png);
+        height: 10px;
+        width: 10px;
+        subcontrol-position: right;
+        subcontrol-origin: margin;
+    }
+
+
+    QScrollBar::sub-line:horizontal:hover, QScrollBar::sub-line:horizontal:on
+    {
+        border-image: url(:/qss_icons/rc/left_arrow.png);
+        height: 10px;
+        width: 10px;
+        subcontrol-position: left;
+        subcontrol-origin: margin;
+    }
+
+    QScrollBar::up-arrow:horizontal, QScrollBar::down-arrow:horizontal
+    {
+        background: none;
+    }
+
+
+    QScrollBar::add-page:horizontal, QScrollBar::sub-page:horizontal
+    {
+        background: none;
+    }
+
+    QScrollBar:vertical
+    {
+        background-color: white;
+        width: 15px;
+        margin: 15px 3px 15px 3px;
+        border: 1px transparent white;
+        border-radius: 4px;
+    }
+
+    QScrollBar::handle:vertical
+    {
+        background-color: #dfdfe1;
+        min-height: 5px;
+        border-radius: 4px;
+    }
+
+    QScrollBar::sub-line:vertical
+    {
+        margin: 3px 0px 3px 0px;
+        border-image: url(:/qss_icons/rc/up_arrow_disabled.png);
+        height: 10px;
+        width: 10px;
+        subcontrol-position: top;
+        subcontrol-origin: margin;
+    }
+
+    QScrollBar::add-line:vertical
+    {
+        margin: 3px 0px 3px 0px;
+        border-image: url(:/qss_icons/rc/down_arrow_disabled.png);
+        height: 10px;
+        width: 10px;
+        subcontrol-position: bottom;
+        subcontrol-origin: margin;
+    }
+
+    QScrollBar::sub-line:vertical:hover,QScrollBar::sub-line:vertical:on
+    {
+        border-image: url(:/qss_icons/rc/up_arrow.png);
+        height: 10px;
+        width: 10px;
+        subcontrol-position: top;
+        subcontrol-origin: margin;
+    }
+
+    QScrollBar::add-line:vertical:hover, QScrollBar::add-line:vertical:on
+    {
+        border-image: url(:/qss_icons/rc/down_arrow.png);
+        height: 10px;
+        width: 10px;
+        subcontrol-position: bottom;
+        subcontrol-origin: margin;
+    }
+
+    QScrollBar::up-arrow:vertical, QScrollBar::down-arrow:vertical
+    {
+        background: none;
+    }
+
+    QScrollBar::add-page:vertical, QScrollBar::sub-page:vertical
+    {
+        background: none;
+    }
+"""
+
+
+app_stylesheet_dark = """
+
+/* --------------------------------------- QPushButton -----------------------------------*/
+
+    QPushButton {
+        background-color: #363638;
+        border-radius: 4px; 
+        margin: 0 0 1px 0;
+    }
+    QPushButton:pressed {
+        background-color: #767678;
+        border-style: inset;
+    }
+    QPushButton:hover:!pressed
+    {
+    background-color: #464648;
     }
 
 /* --------------------------------------- QScrollBar -----------------------------------*/
 
     QScrollBar:horizontal
     {
         height: 15px;
@@ -182,17 +336,18 @@
         super().__init__(parent)
         self.placeholder_image = load_pixmap("empty.png")
 
     def paintEvent(self, event):
         if self.topLevelItemCount() == 0:
             painter = QtGui.QPainter(self.viewport())
             painter.setOpacity(0.5)  # Adjust the opacity of the placeholder image
+            pixel_ratio = QtGui.QGuiApplication.primaryScreen().devicePixelRatio()
             painter.drawPixmap(
-                (self.viewport().width() - self.placeholder_image.width()) / 2,
-                (self.viewport().height() - self.placeholder_image.height()) / 2,
+                (self.viewport().width() - self.placeholder_image.width()/pixel_ratio) / 2,
+                (self.viewport().height() - self.placeholder_image.height()/pixel_ratio) / 2,
                 self.placeholder_image,
             )
         else:
             super().paintEvent(event)
 
 
 def format_value(value, include_unit=True):
@@ -205,22 +360,44 @@
     if not include_unit and isinstance(value, pint.Quantity):
         return str(value.magnitude)
     if isinstance(value, float):
         return "{0:.6g}".format(value)
     return str(value)
 
 
-def load_pixmap(fname_pixmap):
+def load_pixmap(filename, dark_mode_suffix='_dark', high_dpi_suffix='@2x'):
     """
-    Load an image from a file and return it as a QPixmap
+    Load an image from a file and return it as a QPixmap.
+    Load appropriate variants based on pixel ratio and
+    dark or light mode.
     """
+    # Get the pixel ratio
+    pixel_ratio = QtGui.QGuiApplication.primaryScreen().devicePixelRatio()
+
+    # Prepare the filename based on the conditions
+    parts = filename.split('.')
+    if is_dark_mode():
+        parts[0] += dark_mode_suffix
+    if pixel_ratio > 1:
+        parts[0] += high_dpi_suffix
+    adjusted_filename = '.'.join(parts)
+
     file_path = os.path.join(
-        os.path.dirname(tinymovr.__file__), "resources", "icons", fname_pixmap
+        os.path.dirname(tinymovr.__file__), "resources", "icons", adjusted_filename
     )
-    return QtGui.QPixmap(file_path)
+
+    # Load the pixmap and set the device pixel ratio
+    pixmap = QtGui.QPixmap(file_path)
+    pixmap.setDevicePixelRatio(pixel_ratio)
+
+    return pixmap
+
+
+def is_dark_mode():
+    return QGuiApplication.palette().color(QPalette.Window).lightness() < 128
 
 
 def load_icon(fname_icon):
     """
     Load an image from a file and return it as a QIcon
     """
     pixmap = load_pixmap(fname_icon)
```

### Comparing `tinymovr-1.3.1/tinymovr/gui/window.py` & `tinymovr-1.4.0/tinymovr/gui/window.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS
 FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
 You should have received a copy of the GNU General Public License along with
 this program. If not, see <http://www.gnu.org/licenses/>.
 """
 
 import time
+import pkg_resources
 from functools import partial
 from contextlib import suppress
 import json
 from PySide6 import QtCore
 from PySide6.QtCore import Signal
 from PySide6.QtWidgets import (
     QMainWindow,
@@ -29,14 +30,15 @@
     QFrame,
     QHBoxLayout,
     QVBoxLayout,
     QHeaderView,
     QLabel,
     QTreeWidgetItem,
     QPushButton,
+    QMessageBox
 )
 from PySide6.QtGui import QAction
 import pyqtgraph as pg
 from tinymovr.constants import app_name
 from tinymovr.channel import ResponseError as ChannelResponseError
 from tinymovr.config import get_bus_config, configure_logging
 from avlos import get_registry
@@ -72,23 +74,28 @@
 
         self.setWindowTitle(app_name)
 
         # Create a menu bar, menus and actions
         self.menu_bar = QMenuBar()
 
         self.file_menu = QMenu("File")
+        self.help_menu = QMenu("Help")
 
         self.export_action = QAction("Export Config...", self)
         self.import_action = QAction("Import Config", self)
+        self.about_action = QAction("About", self)
         self.export_action.triggered.connect(self.on_export)
         self.import_action.triggered.connect(self.on_import)
+        self.about_action.triggered.connect(self.show_about_box)
         self.file_menu.addAction(self.export_action)
         self.file_menu.addAction(self.import_action)
+        self.help_menu.addAction(self.about_action)
 
         self.menu_bar.addMenu(self.file_menu)
+        self.menu_bar.addMenu(self.help_menu)
         self.setMenuBar(self.menu_bar)
 
         # Setup the tree widget
         self.tree_widget = OurQTreeWidget()
         self.tree_widget.itemChanged.connect(self.item_changed)
         self.tree_widget.itemDoubleClicked.connect(self.double_click)
         self.tree_widget.setHeaderLabels(["Attribute", "Value"])
@@ -270,17 +277,22 @@
                 if len(x) >= 200:
                     x.pop(0)
                     y.pop(0)
                 x.append(time.time() - self.start_time)
                 y.append(magnitude_of(val))
                 graph_info["data_line"].setData(x, y)
                 graph_info["widget"].update()
+        meas_dt = self.worker._rate_limited_update.meas_dt
+        if meas_dt == 0:
+            meas_dt_str = "-"
+        else:
+            meas_dt_str = "{:.1f}Hz".format(meas_dt)
         self.status_label.setText(
-            "{:.1f}Hz\t CH:{:.0f}%\t RT:{:.1f}ms".format(
-                1 / self.worker._rate_limited_update.meas_dt,
+            "{}\t CH:{:.0f}%\t RT:{:.1f}ms".format(
+                meas_dt_str,
                 self.worker._rate_limited_update.load * 100,
                 self.worker.timed_getter.dt * 1000,
             )
         )
 
     @QtCore.Slot()
     def f_call_clicked(self, f):
@@ -325,7 +337,13 @@
     def delete_graph_by_attr_name(self, attr_name):
         self.graphs_by_id[attr_name]["widget"].deleteLater()
         del self.graphs_by_id[attr_name]
 
     def delete_graphs(self):
         for attr_name in list(self.graphs_by_id.keys()):
             self.delete_graph_by_attr_name(attr_name)
+
+    def show_about_box(self):
+        version_str = (pkg_resources.require("tinymovr")[0].version)
+        app_str = "{} {}".format(app_name, version_str)
+        QMessageBox.about(self, "About Tinymovr", "{}\nhttps://tinymovr.com\n\nCat Sleeping Icon by Denis Sazhin from Noun Project".format(app_str))
+
```

### Comparing `tinymovr-1.3.1/tinymovr/gui/worker.py` & `tinymovr-1.4.0/tinymovr/gui/worker.py`

 * *Files identical despite different names*

### Comparing `tinymovr-1.3.1/tinymovr/resources/icons/call.png` & `tinymovr-1.4.0/tinymovr/resources/icons/call.png`

 * *Files identical despite different names*

### Comparing `tinymovr-1.3.1/tinymovr/tee.py` & `tinymovr-1.4.0/tinymovr/tee.py`

 * *Files 5% similar despite different names*

```diff
@@ -47,14 +47,15 @@
 
     Also implements a simple forwarding mechanism for sending messages, to
     simplify interfacing with CAN bus objects.
     """
 
     def __init__(self, bus, timeout):
         self.bus = bus
+        self.flush_rx_buffer()
         self.timeout = timeout
         self.clients = []
         self.state = TeeState.INIT
         self.update_thread = Thread(target=self.update, daemon=True)
         self.update_thread.start()
 
     def add(self, filter_cb, recv_cb):
@@ -87,22 +88,31 @@
 
     def stop(self):
         self.state = TeeState.STOPPING
         while TeeState.STOPPING == self.state:
             time.sleep(0.01)
         assert TeeState.STOPPED == self.state
 
+    def flush_rx_buffer(self, trials=100):
+        """
+        Flush the RX buffer of a bus
+        """
+        for i in range(trials):
+            if not self.bus.recv(timeout=0.001):
+                return
+
 
 def init_tee(bus, timeout=0.1):
     """
     Initializes a tee using a python-can bus instance
     """
     global tee
     assert None == tee
     tee = Tee(bus, timeout)
+    return tee
 
 
 def destroy_tee():
     """
     Destroys the existing tee, stopping its thread.
     """
     global tee
```

### Comparing `tinymovr-1.3.1/tinymovr.egg-info/PKG-INFO` & `tinymovr-1.4.0/tinymovr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinymovr
-Version: 1.3.1
+Version: 1.4.0
 Summary: Tinymovr Studio
 Home-page: https://github.com/yconst/Tinymovr
 Author: Yannis Chatzikonstantinou
 Author-email: info@tinymovr.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `tinymovr-1.3.1/tinymovr.egg-info/SOURCES.txt` & `tinymovr-1.4.0/tinymovr.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -20,9 +20,14 @@
 tinymovr/config/device.yaml
 tinymovr/gui/__init__.py
 tinymovr/gui/gui.py
 tinymovr/gui/helpers.py
 tinymovr/gui/window.py
 tinymovr/gui/worker.py
 tinymovr/resources/icons/call.png
+tinymovr/resources/icons/call@2x.png
+tinymovr/resources/icons/call_dark.png
+tinymovr/resources/icons/call_dark@2x.png
 tinymovr/resources/icons/empty.png
-tinymovr/resources/icons/empty@2x.png
+tinymovr/resources/icons/empty@2x.png
+tinymovr/resources/icons/empty_dark.png
+tinymovr/resources/icons/empty_dark@2x.png
```

