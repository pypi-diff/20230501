# Comparing `tmp/hubitatcontrol-2.1.0.tar.gz` & `tmp/hubitatcontrol-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hubitatcontrol-2.1.0.tar", max compression
+gzip compressed data, was "hubitatcontrol-2.2.0.tar", max compression
```

## Comparing `hubitatcontrol-2.1.0.tar` & `hubitatcontrol-2.2.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1064 2023-03-12 19:21:22.061753 hubitatcontrol-2.1.0/LICENSE
--rw-r--r--   0        0        0     6247 2023-04-23 03:06:31.100361 hubitatcontrol-2.1.0/README.md
--rw-r--r--   0        0        0     1936 2023-04-29 01:57:50.164004 hubitatcontrol-2.1.0/hubitatcontrol/__init__.py
--rw-r--r--   0        0        0     3765 2023-04-23 03:06:31.104361 hubitatcontrol-2.1.0/hubitatcontrol/__main__.py
--rw-r--r--   0        0        0      172 2023-04-29 01:54:13.037854 hubitatcontrol-2.1.0/hubitatcontrol/environment.py
--rw-r--r--   0        0        0     1060 2023-04-23 03:06:31.104361 hubitatcontrol-2.1.0/hubitatcontrol/generic.py
--rw-r--r--   0        0        0     2902 2023-04-23 03:06:31.104361 hubitatcontrol-2.1.0/hubitatcontrol/hub.py
--rw-r--r--   0        0        0     2774 2023-04-23 03:06:31.104361 hubitatcontrol-2.1.0/hubitatcontrol/lights.py
--rw-r--r--   0        0        0      336 2023-04-29 01:51:56.296942 hubitatcontrol-2.1.0/hubitatcontrol/sensors.py
--rw-r--r--   0        0        0     2606 2023-04-29 02:26:10.971754 hubitatcontrol-2.1.0/pyproject.toml
--rw-r--r--   0        0        0     7129 1970-01-01 00:00:00.000000 hubitatcontrol-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-03-12 19:21:22.061753 hubitatcontrol-2.2.0/LICENSE
+-rw-r--r--   0        0        0     6311 2023-05-01 03:13:59.733229 hubitatcontrol-2.2.0/README.md
+-rw-r--r--   0        0        0     2381 2023-05-01 03:13:59.733229 hubitatcontrol-2.2.0/hubitatcontrol/__init__.py
+-rw-r--r--   0        0        0     3824 2023-05-01 03:13:59.733229 hubitatcontrol-2.2.0/hubitatcontrol/__main__.py
+-rw-r--r--   0        0        0      172 2023-05-01 03:13:59.733229 hubitatcontrol-2.2.0/hubitatcontrol/environment.py
+-rw-r--r--   0        0        0     1060 2023-04-23 03:06:31.104361 hubitatcontrol-2.2.0/hubitatcontrol/generic.py
+-rw-r--r--   0        0        0     2902 2023-04-23 03:06:31.104361 hubitatcontrol-2.2.0/hubitatcontrol/hub.py
+-rw-r--r--   0        0        0     2774 2023-04-23 03:06:31.104361 hubitatcontrol-2.2.0/hubitatcontrol/lights.py
+-rw-r--r--   0        0        0      336 2023-04-29 01:51:56.296942 hubitatcontrol-2.2.0/hubitatcontrol/sensors.py
+-rw-r--r--   0        0        0     2606 2023-05-01 03:17:15.357544 hubitatcontrol-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0     7193 1970-01-01 00:00:00.000000 hubitatcontrol-2.2.0/PKG-INFO
```

### Comparing `hubitatcontrol-2.1.0/LICENSE` & `hubitatcontrol-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hubitatcontrol-2.1.0/README.md` & `hubitatcontrol-2.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,17 @@
 
 ## Intro
 
 This guide assumes you own a **Hubitat Elevation** home automation controller.
 
 If you are interested in purchasing one, you can purchase a unit from the manufactures website at [hubitat.com](https://hubitat.com/products) or from [Amazon.com](https://www.amazon.com/Hubitat-Elevation-Home-Automation-Hub/dp/B07D19VVTX/)
 
+## Changes
+See [CHANGELOG.md](CHANGELOG.md) for current changes
+
 ## Setup
 
 To get the required API keys, you will need to log in to your Hubitat admin interface.
 
 See [Maker API Documentation](https://docs2.hubitat.com/en/apps/maker-api) for how to add the `MakerAPI` application and to generate new API keys
 
 If you are using the cloud API endpoint for access, you will ALSO need to include the Cloud API key when setting up a new Hub object.
@@ -104,15 +107,15 @@
 ## Docs
 
 [Located in /docs folder](docs)
 
 You will need a .dot file browser for the class diagrams
 
 ## Issues / Features
-See: 
+See:
 
 https://github.com/Jelloeater/hubitatcontrol/issues
 
 ## Structure
 
 **Class Model**
```

### Comparing `hubitatcontrol-2.1.0/hubitatcontrol/__init__.py` & `hubitatcontrol-2.2.0/hubitatcontrol/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,43 +2,56 @@
 
 import hubitatcontrol.generic
 import hubitatcontrol.lights
 import hubitatcontrol.sensors
 from hubitatcontrol.hub import Hub
 
 
+def get_device_type(device_in: hubitatcontrol.hub.Device, hub_in: hubitatcontrol.hub):
+    if device_in is None:
+        raise Exception("Device Not Found")
+    if "ColorControl" in device_in["capabilities"] and "ColorMode" in device_in["capabilities"]:
+        return hubitatcontrol.lights.RGBWBulb(device_from_hub=device_in, hub=hub_in)
+    if "ColorTemperature" in device_in["capabilities"]:
+        return hubitatcontrol.lights.ColorTempBulb(device_from_hub=device_in, hub=hub_in)
+    if "ChangeLevel" in device_in["capabilities"]:
+        return hubitatcontrol.lights.Bulb(device_from_hub=device_in, hub=hub_in)
+    if "SwitchLevel" in device_in["capabilities"]:
+        return hubitatcontrol.lights.Dimmer(device_from_hub=device_in, hub=hub_in)
+    if "PowerMeter" in device_in["capabilities"] and "Outlet" in device_in["capabilities"]:
+        return hubitatcontrol.generic.ZigbeeOutlet(device_from_hub=device_in, hub=hub_in)
+    if "Switch" in device_in["capabilities"]:
+        return hubitatcontrol.generic.Switch(device_from_hub=device_in, hub=hub_in)
+    if "TemperatureMeasurement" in device_in["capabilities"]:
+        return hubitatcontrol.sensors.TemperatureSensor(device_from_hub=device_in, hub=hub_in)
+
+
 def get_hub(host, token, app_id, cloud_token=None) -> Hub:
     return Hub(host=host, token=token, app_id=app_id, cloud_token=cloud_token)
 
 
 def lookup_device(hub_in, device_lookup):
-    # TODO Refactor to use ID, and and add interface for name search
     """
     Takes device NAME, not ID for lookup
     """
-    d = hub_in.get_device(device_lookup)
-    if d is None:
-        raise Exception("Device Not Found")
-    if "ColorControl" in d["capabilities"] and "ColorMode" in d["capabilities"]:
-        return hubitatcontrol.lights.RGBWBulb(device_from_hub=d, hub=hub_in)
-    if "ColorTemperature" in d["capabilities"]:
-        return hubitatcontrol.lights.ColorTempBulb(device_from_hub=d, hub=hub_in)
-    if "ChangeLevel" in d["capabilities"]:
-        return hubitatcontrol.lights.Bulb(device_from_hub=d, hub=hub_in)
-    if "SwitchLevel" in d["capabilities"]:
-        return hubitatcontrol.lights.Dimmer(device_from_hub=d, hub=hub_in)
-    if "PowerMeter" in d["capabilities"] and "Outlet" in d["capabilities"]:
-        return hubitatcontrol.generic.ZigbeeOutlet(device_from_hub=d, hub=hub_in)
-    if "Switch" in d["capabilities"]:
-        return hubitatcontrol.generic.Switch(device_from_hub=d, hub=hub_in)
-    if "TemperatureMeasurement" in d["capabilities"]:
-        return hubitatcontrol.sensors.TemperatureSensor(device_from_hub=d, hub=hub_in)
-    return d  # Fall through return # pragma: no cover
+
+    return get_device_type(
+        device_in=hub_in.get_device(device_lookup), hub_in=hub_in
+    )  # Fall through return # pragma: no cover
+
+
+def lookup_device_id(hub_in, device_id):
+    """
+    Takes device NAME, not ID for lookup
+    """
+    return get_device_type(
+        device_in=hub_in.get_device_id(device_id), hub_in=hub_in
+    )  # Fall through return # pragma: no cover
 
 
 def get_all_temperature_sensors(hub_in: hubitatcontrol.hub) -> list[hubitatcontrol.sensors.TemperatureSensor]:
     """Returns list of all hub devices with associated helper functions"""
     device_list = []
     for i in hub_in.devices:
         if "TemperatureMeasurement" in i["capabilities"]:
-            device_list.append(lookup_device(hub_in, i['name']))
+            device_list.append(lookup_device_id(hub_in, i['id']))
     return device_list
```

### Comparing `hubitatcontrol-2.1.0/hubitatcontrol/__main__.py` & `hubitatcontrol-2.2.0/hubitatcontrol/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
 def hub_from_keyring():
     check_keyring()
     host_env = keyring.get_password("hubitatcontrol", "HUBITAT_HOST")
     token_env = keyring.get_password("hubitatcontrol", "HUBITAT_API_TOKEN")
     app_id_env = keyring.get_password("hubitatcontrol", "HUBITAT_API_APP_ID")
     cloud_token_env = keyring.get_password("hubitatcontrol", "HUBITAT_CLOUD_TOKEN")
-    if cloud_token_env is None:
+    if cloud_token_env == 'None':  # nosec # Fixes string to obj casting on env file parse
         cloud_token_env = None
     return get_hub(host=host_env, token=token_env, app_id=app_id_env, cloud_token=cloud_token_env)
 
 
 @app.command()
 def ls():
     """
```

### Comparing `hubitatcontrol-2.1.0/hubitatcontrol/generic.py` & `hubitatcontrol-2.2.0/hubitatcontrol/generic.py`

 * *Files identical despite different names*

### Comparing `hubitatcontrol-2.1.0/hubitatcontrol/hub.py` & `hubitatcontrol-2.2.0/hubitatcontrol/hub.py`

 * *Files identical despite different names*

### Comparing `hubitatcontrol-2.1.0/hubitatcontrol/lights.py` & `hubitatcontrol-2.2.0/hubitatcontrol/lights.py`

 * *Files identical despite different names*

### Comparing `hubitatcontrol-2.1.0/pyproject.toml` & `hubitatcontrol-2.2.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hubitatcontrol"
-version = "v2.1.0"
+version = "v2.2.0"
 description = "Hubitat Maker API Interface"
 authors = ["Jesse Schoepfer <jelloeater@gmail.com>"]
 license = "MIT License"
 readme = "README.md"
 homepage = "https://github.com/Jelloeater/hubitatcontrol"
 keywords = ["hubitat", "makerapi","requests"]
 classifiers = ["Development Status :: 5 - Production/Stable",
```

### Comparing `hubitatcontrol-2.1.0/PKG-INFO` & `hubitatcontrol-2.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hubitatcontrol
-Version: 2.1.0
+Version: 2.2.0
 Summary: Hubitat Maker API Interface
 Home-page: https://github.com/Jelloeater/hubitatcontrol
 License: MIT
 Keywords: hubitat,makerapi,requests
 Author: Jesse Schoepfer
 Author-email: jelloeater@gmail.com
 Requires-Python: >=3.10,<4.0
@@ -36,14 +36,17 @@
 
 ## Intro
 
 This guide assumes you own a **Hubitat Elevation** home automation controller.
 
 If you are interested in purchasing one, you can purchase a unit from the manufactures website at [hubitat.com](https://hubitat.com/products) or from [Amazon.com](https://www.amazon.com/Hubitat-Elevation-Home-Automation-Hub/dp/B07D19VVTX/)
 
+## Changes
+See [CHANGELOG.md](CHANGELOG.md) for current changes
+
 ## Setup
 
 To get the required API keys, you will need to log in to your Hubitat admin interface.
 
 See [Maker API Documentation](https://docs2.hubitat.com/en/apps/maker-api) for how to add the `MakerAPI` application and to generate new API keys
 
 If you are using the cloud API endpoint for access, you will ALSO need to include the Cloud API key when setting up a new Hub object.
@@ -129,15 +132,15 @@
 ## Docs
 
 [Located in /docs folder](docs)
 
 You will need a .dot file browser for the class diagrams
 
 ## Issues / Features
-See: 
+See:
 
 https://github.com/Jelloeater/hubitatcontrol/issues
 
 ## Structure
 
 **Class Model**
```

