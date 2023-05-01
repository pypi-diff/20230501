# Comparing `tmp/liblineage-1.3.1.tar.gz` & `tmp/liblineage-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liblineage-1.3.1.tar", max compression
+gzip compressed data, was "liblineage-1.3.2.tar", max compression
```

## Comparing `liblineage-1.3.1.tar` & `liblineage-1.3.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0      386 2023-04-17 16:03:26.868684 liblineage-1.3.1/README.md
--rw-r--r--   0        0        0      237 2023-04-17 16:11:42.746823 liblineage-1.3.1/liblineage/__init__.py
--rw-r--r--   0        0        0      198 2023-04-17 16:03:26.868684 liblineage-1.3.1/liblineage/constants/infra.py
--rw-r--r--   0        0        0      657 2023-04-17 16:03:26.868684 liblineage-1.3.1/liblineage/constants/versions.py
--rw-r--r--   0        0        0      746 2023-04-17 16:03:26.868684 liblineage-1.3.1/liblineage/device.py
--rw-r--r--   0        0        0     2212 2023-04-17 16:03:26.868684 liblineage-1.3.1/liblineage/hudson/build_target.py
--rw-r--r--   0        0        0      222 2023-04-17 16:03:26.868684 liblineage-1.3.1/liblineage/hudson/period.py
--rw-r--r--   0        0        0     2360 2023-04-17 16:03:26.868684 liblineage-1.3.1/liblineage/ota/full_update_info.py
--rw-r--r--   0        0        0      219 2023-04-17 16:03:26.868684 liblineage-1.3.1/liblineage/updater/__init__.py
--rw-r--r--   0        0        0      463 2023-04-17 16:03:26.868684 liblineage-1.3.1/liblineage/updater/http_utils.py
--rw-r--r--   0        0        0     2008 2023-04-17 16:03:26.868684 liblineage-1.3.1/liblineage/updater/v1/__init__.py
--rw-r--r--   0        0        0      479 2023-04-17 16:03:26.868684 liblineage-1.3.1/liblineage/updater/v1/_deserializer.py
--rw-r--r--   0        0        0     1249 2023-04-17 16:03:26.868684 liblineage-1.3.1/liblineage/updater/v1/build.py
--rw-r--r--   0        0        0     1726 2023-04-17 16:03:26.868684 liblineage-1.3.1/liblineage/updater/v2/__init__.py
--rw-r--r--   0        0        0      527 2023-04-17 16:03:26.868684 liblineage-1.3.1/liblineage/updater/v2/_deserializer.py
--rw-r--r--   0        0        0      943 2023-04-17 16:03:26.868684 liblineage-1.3.1/liblineage/updater/v2/build.py
--rw-r--r--   0        0        0      971 2023-04-17 16:03:26.868684 liblineage-1.3.1/liblineage/updater/v2/build_file.py
--rw-r--r--   0        0        0     1049 2023-04-17 16:03:26.868684 liblineage-1.3.1/liblineage/updater/v2/device.py
--rw-r--r--   0        0        0      681 2023-04-17 16:03:26.868684 liblineage-1.3.1/liblineage/updater/v2/oem.py
--rw-r--r--   0        0        0      543 2023-04-17 16:03:26.868684 liblineage-1.3.1/liblineage/updater/v2/oem_device.py
--rw-r--r--   0        0        0      879 2023-04-17 16:03:26.868684 liblineage-1.3.1/liblineage/wiki/data_types/architecture_data.py
--rw-r--r--   0        0        0      582 2023-04-17 16:03:26.868684 liblineage-1.3.1/liblineage/wiki/data_types/base_data.py
--rw-r--r--   0        0        0     1259 2023-04-17 16:03:26.868684 liblineage-1.3.1/liblineage/wiki/data_types/battery_data.py
--rw-r--r--   0        0        0      898 2023-04-17 16:03:26.868684 liblineage-1.3.1/liblineage/wiki/data_types/bluetooth_data.py
--rw-r--r--   0        0        0      890 2023-04-17 16:03:26.868684 liblineage-1.3.1/liblineage/wiki/data_types/camera_data.py
--rw-r--r--   0        0        0     1204 2023-04-17 16:03:26.868684 liblineage-1.3.1/liblineage/wiki/data_types/dimension_data.py
--rw-r--r--   0        0        0      819 2023-04-17 16:03:26.868684 liblineage-1.3.1/liblineage/wiki/data_types/peripherals_data.py
--rw-r--r--   0        0        0     1141 2023-04-17 16:03:26.868684 liblineage-1.3.1/liblineage/wiki/data_types/release_data.py
--rw-r--r--   0        0        0     1352 2023-04-17 16:03:26.868684 liblineage-1.3.1/liblineage/wiki/data_types/screen_data.py
--rw-r--r--   0        0        0      877 2023-04-17 16:03:26.868684 liblineage-1.3.1/liblineage/wiki/data_types/sdcard_data.py
--rw-r--r--   0        0        0    11403 2023-04-17 16:10:54.370325 liblineage-1.3.1/liblineage/wiki/device_data.py
--rw-r--r--   0        0        0      520 2023-04-17 16:11:39.474790 liblineage-1.3.1/pyproject.toml
--rw-r--r--   0        0        0     1281 1970-01-01 00:00:00.000000 liblineage-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0      386 2022-08-26 23:24:36.752356 liblineage-1.3.2/README.md
+-rw-r--r--   0        0        0      237 2023-05-01 17:23:47.459149 liblineage-1.3.2/liblineage/__init__.py
+-rw-r--r--   0        0        0      198 2022-08-30 13:21:57.046166 liblineage-1.3.2/liblineage/constants/infra.py
+-rw-r--r--   0        0        0      657 2023-03-06 00:37:23.199983 liblineage-1.3.2/liblineage/constants/versions.py
+-rw-r--r--   0        0        0      746 2023-03-06 15:41:20.302137 liblineage-1.3.2/liblineage/device.py
+-rw-r--r--   0        0        0     2277 2023-05-01 17:19:48.153672 liblineage-1.3.2/liblineage/hudson/build_target.py
+-rw-r--r--   0        0        0      222 2022-09-10 16:59:53.229174 liblineage-1.3.2/liblineage/hudson/period.py
+-rw-r--r--   0        0        0     2360 2023-03-06 15:35:33.081202 liblineage-1.3.2/liblineage/ota/full_update_info.py
+-rw-r--r--   0        0        0      219 2023-03-06 13:45:03.612525 liblineage-1.3.2/liblineage/updater/__init__.py
+-rw-r--r--   0        0        0      463 2023-03-06 13:57:45.253121 liblineage-1.3.2/liblineage/updater/http_utils.py
+-rw-r--r--   0        0        0     2008 2023-03-06 15:15:22.908220 liblineage-1.3.2/liblineage/updater/v1/__init__.py
+-rw-r--r--   0        0        0      479 2023-03-06 15:15:13.344857 liblineage-1.3.2/liblineage/updater/v1/_deserializer.py
+-rw-r--r--   0        0        0     1249 2023-03-06 15:13:58.101291 liblineage-1.3.2/liblineage/updater/v1/build.py
+-rw-r--r--   0        0        0     1726 2023-03-06 15:15:46.388292 liblineage-1.3.2/liblineage/updater/v2/__init__.py
+-rw-r--r--   0        0        0      527 2023-03-06 15:16:02.488342 liblineage-1.3.2/liblineage/updater/v2/_deserializer.py
+-rw-r--r--   0        0        0      943 2023-03-06 13:43:39.422459 liblineage-1.3.2/liblineage/updater/v2/build.py
+-rw-r--r--   0        0        0      971 2023-03-06 00:38:14.543370 liblineage-1.3.2/liblineage/updater/v2/build_file.py
+-rw-r--r--   0        0        0     1049 2023-04-11 15:28:06.745781 liblineage-1.3.2/liblineage/updater/v2/device.py
+-rw-r--r--   0        0        0      681 2023-03-06 13:30:12.755159 liblineage-1.3.2/liblineage/updater/v2/oem.py
+-rw-r--r--   0        0        0      543 2023-03-06 13:30:12.755159 liblineage-1.3.2/liblineage/updater/v2/oem_device.py
+-rw-r--r--   0        0        0      879 2023-05-01 15:29:50.890397 liblineage-1.3.2/liblineage/wiki/data_types/architecture_data.py
+-rw-r--r--   0        0        0      582 2022-08-27 01:08:57.416656 liblineage-1.3.2/liblineage/wiki/data_types/base_data.py
+-rw-r--r--   0        0        0     1279 2023-05-01 17:14:06.456807 liblineage-1.3.2/liblineage/wiki/data_types/battery_data.py
+-rw-r--r--   0        0        0      918 2023-05-01 17:14:18.776934 liblineage-1.3.2/liblineage/wiki/data_types/bluetooth_data.py
+-rw-r--r--   0        0        0      904 2023-05-01 17:13:44.383245 liblineage-1.3.2/liblineage/wiki/data_types/camera_data.py
+-rw-r--r--   0        0        0     1204 2023-05-01 15:29:50.890397 liblineage-1.3.2/liblineage/wiki/data_types/dimension_data.py
+-rw-r--r--   0        0        0      819 2023-05-01 15:29:50.890397 liblineage-1.3.2/liblineage/wiki/data_types/peripherals_data.py
+-rw-r--r--   0        0        0     1144 2023-05-01 17:15:15.924192 liblineage-1.3.2/liblineage/wiki/data_types/release_data.py
+-rw-r--r--   0        0        0     1352 2023-05-01 15:29:50.890397 liblineage-1.3.2/liblineage/wiki/data_types/screen_data.py
+-rw-r--r--   0        0        0      897 2023-05-01 17:15:56.411278 liblineage-1.3.2/liblineage/wiki/data_types/sdcard_data.py
+-rw-r--r--   0        0        0    11617 2023-05-01 17:17:27.062215 liblineage-1.3.2/liblineage/wiki/device_data.py
+-rw-r--r--   0        0        0      520 2023-05-01 17:23:43.362447 liblineage-1.3.2/pyproject.toml
+-rw-r--r--   0        0        0     1281 1970-01-01 00:00:00.000000 liblineage-1.3.2/PKG-INFO
```

### Comparing `liblineage-1.3.1/liblineage/constants/versions.py` & `liblineage-1.3.2/liblineage/constants/versions.py`

 * *Files identical despite different names*

### Comparing `liblineage-1.3.1/liblineage/device.py` & `liblineage-1.3.2/liblineage/device.py`

 * *Files identical despite different names*

### Comparing `liblineage-1.3.1/liblineage/hudson/build_target.py` & `liblineage-1.3.2/liblineage/hudson/build_target.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 LINEAGE_BUILD_TARGETS_FILE = f"https://raw.githubusercontent.com/{GITHUB_ORG}/hudson/master/lineage-build-targets"
 
 class BuildTarget:
 	def __init__(self,
 	             device: str,
 	             build_type: str,
 	             branch_name: str,
-	             period: str,
+	             period: Period,
 	            ):
 		self.device = device
 		self.build_type = build_type
 		self.branch_name = branch_name
 		self.period = period
 
 	def __str__(self) -> str:
@@ -70,7 +70,9 @@
 
 			if delta_day <= 0:
 				# Go to next month
 				month_to_days = [31, 28, 31, 30, 31, 30, 31, 31, 30, 31, 30, 31]
 				delta_day += month_to_days[today.month-1]
 
 			return today + timedelta(days=delta_day)
+
+		raise NotImplementedError(f"Unknown period {self.period}")
```

### Comparing `liblineage-1.3.1/liblineage/ota/full_update_info.py` & `liblineage-1.3.2/liblineage/ota/full_update_info.py`

 * *Files identical despite different names*

### Comparing `liblineage-1.3.1/liblineage/updater/v1/__init__.py` & `liblineage-1.3.2/liblineage/updater/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `liblineage-1.3.1/liblineage/updater/v1/build.py` & `liblineage-1.3.2/liblineage/updater/v1/build.py`

 * *Files identical despite different names*

### Comparing `liblineage-1.3.1/liblineage/updater/v2/__init__.py` & `liblineage-1.3.2/liblineage/updater/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `liblineage-1.3.1/liblineage/updater/v2/_deserializer.py` & `liblineage-1.3.2/liblineage/updater/v2/_deserializer.py`

 * *Files identical despite different names*

### Comparing `liblineage-1.3.1/liblineage/updater/v2/build.py` & `liblineage-1.3.2/liblineage/updater/v2/build.py`

 * *Files identical despite different names*

### Comparing `liblineage-1.3.1/liblineage/updater/v2/build_file.py` & `liblineage-1.3.2/liblineage/updater/v2/build_file.py`

 * *Files identical despite different names*

### Comparing `liblineage-1.3.1/liblineage/updater/v2/device.py` & `liblineage-1.3.2/liblineage/updater/v2/device.py`

 * *Files identical despite different names*

### Comparing `liblineage-1.3.1/liblineage/updater/v2/oem.py` & `liblineage-1.3.2/liblineage/updater/v2/oem.py`

 * *Files identical despite different names*

### Comparing `liblineage-1.3.1/liblineage/updater/v2/oem_device.py` & `liblineage-1.3.2/liblineage/updater/v2/oem_device.py`

 * *Files identical despite different names*

### Comparing `liblineage-1.3.1/liblineage/wiki/data_types/architecture_data.py` & `liblineage-1.3.2/liblineage/wiki/data_types/architecture_data.py`

 * *Files identical despite different names*

### Comparing `liblineage-1.3.1/liblineage/wiki/data_types/base_data.py` & `liblineage-1.3.2/liblineage/wiki/data_types/base_data.py`

 * *Files identical despite different names*

### Comparing `liblineage-1.3.1/liblineage/wiki/data_types/battery_data.py` & `liblineage-1.3.2/liblineage/wiki/data_types/battery_data.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 #
 # Copyright (C) 2022 The LineageOS Project
 #
 # SPDX-License-Identifier: LGPL-3.0-or-later
 #
 
-from typing import Dict, List, Union
+from typing import Dict, List, Optional, Union
 
 from liblineage.wiki.data_types.base_data import BaseData
 
 class BatteryData(BaseData):
 	"""LineageOS battery information.
 
 	Attributes:
 	- capacity: The battery capacity (mAh)
 	- removable: Whether the battery is removable
 	- tech: The battery technology
 	"""
 	def __init__(self,
 	             capacity: int,
 	             removable: bool,
-	             tech: str = None,
+	             tech: Optional[str] = None,
 	            ):
 		"""Initialize the battery information."""
 		super().__init__()
 
 		self.capacity = capacity
 		self.removable = removable
 		self.tech = tech
```

### Comparing `liblineage-1.3.1/liblineage/wiki/data_types/bluetooth_data.py` & `liblineage-1.3.2/liblineage/wiki/data_types/bluetooth_data.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 #
 # Copyright (C) 2022 The LineageOS Project
 #
 # SPDX-License-Identifier: LGPL-3.0-or-later
 #
 
-from typing import Dict, List, Union
+from typing import Dict, List, Optional, Union
 
 from liblineage.wiki.data_types.base_data import BaseData
 
 class BluetoothData(BaseData):
 	"""LineageOS Bluetooth information.
 
 	Attributes:
 	- spec: Bluetooth specification
 	- profiles: Bluetooth profile
 	"""
 	def __init__(self,
 	             spec: str,
-	             profiles: List[str] = None
+	             profiles: Optional[List[str]] = None
 	            ):
 		"""Initialize the Bluetooth information."""
 		super().__init__()
 
 		self.spec = spec
 		self.profiles = profiles or []
```

### Comparing `liblineage-1.3.1/liblineage/wiki/data_types/camera_data.py` & `liblineage-1.3.2/liblineage/wiki/data_types/camera_data.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #
 # Copyright (C) 2022 The LineageOS Project
 #
 # SPDX-License-Identifier: LGPL-3.0-or-later
 #
 
-from typing import Dict, List, Union
+from typing import Dict, List, Sequence, Union
 
 from liblineage.wiki.data_types.base_data import BaseData
 
 class CameraData(BaseData):
 	"""The format for the camera property.
 
 	Attributes:
@@ -22,15 +22,15 @@
 		"""Initialize the camera information."""
 		super().__init__()
 
 		self.info = info
 		self.flash = flash
 
 	@classmethod
-	def from_data(cls, data: Union[None, List[Dict]]) -> Union[None, List["CameraData"]]:
+	def from_data(cls, data: Union[None, List[Dict]]) -> Union[None, Sequence["CameraData"]]:
 		"""Create a camera information object from YAML data."""
 		if data is None:
 			camera = None
 		elif isinstance(data, list):
 			camera = [cls.from_dict(camera_data) for camera_data in data]
 		else:
 			raise Exception("Invalid camera data")
```

### Comparing `liblineage-1.3.1/liblineage/wiki/data_types/dimension_data.py` & `liblineage-1.3.2/liblineage/wiki/data_types/dimension_data.py`

 * *Files identical despite different names*

### Comparing `liblineage-1.3.1/liblineage/wiki/data_types/peripherals_data.py` & `liblineage-1.3.2/liblineage/wiki/data_types/peripherals_data.py`

 * *Files identical despite different names*

### Comparing `liblineage-1.3.1/liblineage/wiki/data_types/release_data.py` & `liblineage-1.3.2/liblineage/wiki/data_types/release_data.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,29 +5,30 @@
 #
 
 from datetime import datetime, date
 from typing import Dict, List, Union
 
 class ReleaseData:
 	"""LineageOS release information."""
+	@staticmethod
 	def convert_release_date(data: Union[int, str]):
 		data = str(data)
 		# YYYY-MM-DD
 		try:
 			return date.fromisoformat(data)
 		except ValueError:
 			# YYYY-MM
 			try:
 				return datetime.strptime(data, "%Y-%m").date()
 			except ValueError:
 				# YYYY
 				return datetime.strptime(data, "%Y").date()
 
 	@classmethod
-	def from_data(cls, data: Union[date, int, str, List]) -> Union[date, date, date, Dict[str, date]]:
+	def from_data(cls, data: Union[date, int, str, List]) -> Union[date, Dict[str, date]]:
 		"""Create a release information object from YAML data."""
 		if isinstance(data, date):
 			release = data
 		elif isinstance(data, int):
 			release = cls.convert_release_date(data)
 		elif isinstance(data, str):
 			release = cls.convert_release_date(data)
```

### Comparing `liblineage-1.3.1/liblineage/wiki/data_types/screen_data.py` & `liblineage-1.3.2/liblineage/wiki/data_types/screen_data.py`

 * *Files identical despite different names*

### Comparing `liblineage-1.3.1/liblineage/wiki/data_types/sdcard_data.py` & `liblineage-1.3.2/liblineage/wiki/data_types/sdcard_data.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 #
 # Copyright (C) 2022 The LineageOS Project
 #
 # SPDX-License-Identifier: LGPL-3.0-or-later
 #
 
-from typing import Dict, Union
+from typing import Dict, Optional, Union
 
 from liblineage.wiki.data_types.base_data import BaseData
 
 class SdcardData(BaseData):
 	"""The format required for the sdcard property.
 
 	Attributes:
 	- sizeMax: Maximum size for a sdcard
 	- slot: where the sdcard is inserted
 	"""
 	def __init__(self,
 	             sizeMax: str,
-	             slot: str = None
+	             slot: Optional[str] = None
 	            ):
 		"""Initialize the sdcard information."""
 		super().__init__()
 
 		self.sizeMax = sizeMax
 		self.slot = slot
```

### Comparing `liblineage-1.3.1/liblineage/wiki/device_data.py` & `liblineage-1.3.2/liblineage/wiki/device_data.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (C) 2022 The LineageOS Project
 #
 # SPDX-License-Identifier: LGPL-3.0-or-later
 #
 
 from datetime import date
 import requests
-from typing import Dict, List, Union
+from typing import Any, Dict, List, Sequence, Union
 import yaml
 
 from liblineage.constants.infra import GITHUB_ORG, GITHUB_ORG_URL
 from liblineage.wiki.data_types.architecture_data import ArchitectureData
 from liblineage.wiki.data_types.battery_data import BatteryData
 from liblineage.wiki.data_types.bluetooth_data import BluetoothData
 from liblineage.wiki.data_types.camera_data import CameraData
@@ -95,15 +95,15 @@
 	             vendor: str,
 	             vendor_short: str,
 	             versions: List[float],
 
 				 before_install: Union[str, None] = None,
 				 before_lineage_install: Union[str, None] = None,
 				 before_recovery_install: Union[str, None] = None,
-				 cameras: Union[List[CameraData], None] = None,
+				 cameras: Union[Sequence[CameraData], None] = None,
 				 carrier: Union[str, None] = None,
 				 custom_recovery_codename: Union[str, None] = None,
 				 custom_recovery_link: Union[str, None] = None,
 				 custom_unlock_cmd: Union[str, None] = None,
 				 download_boot: Union[str, None] = None,
 				 format_on_upgrade: Union[bool, None] = None,
 				 has_recovery_partition: Union[bool, None] = None,
@@ -218,56 +218,75 @@
 		response = requests.get(url=url)
 		response.raise_for_status()
 		return cls.from_dict(yaml.safe_load(response.text))
 
 	def __str__(self) -> str:
 		"""Return a string representation of the device data."""
 		infos = {
-			"Name": self.name,
-			"Codename": self.codename,
-			"Architecture": self.architecture,
-			"Battery": ", ".join([f'{device}: {battery_data}' for device, battery_data in self.battery.items()]) if isinstance(self.battery, dict) else self.battery,
-			"Bluetooth": self.bluetooth,
-			"CPU": self.cpu,
-			"CPU cores": self.cpu_cores,
-			"CPU frequency": self.cpu_freq,
-			"Dimensions": ", ".join([f'{device}: {dimensions_data}' for device, dimensions_data in self.dimensions.items()]) if isinstance(self.dimensions, dict) else self.dimensions,
-			"GPU": self.gpu,
+			"Name": self._print_data(self.name),
+			"Codename": self._print_data(self.codename),
+			"Architecture": self._print_data(self.architecture),
+			"Battery": self._print_data(self.battery),
+			"Bluetooth": self._print_data(self.bluetooth),
+			"CPU": self._print_data(self.cpu),
+			"CPU cores": self._print_data(self.cpu_cores),
+			"CPU frequency": self._print_data(self.cpu_freq),
+			"Dimensions": self._print_data(self.dimensions),
+			"GPU": self._print_data(self.gpu),
 			"Kernel repository": f"{GITHUB_ORG_URL}/{self.kernel}",
 			"Maintainers": ", ".join(self.maintainers) if self.maintainers else "None (unmaintained)",
-			"Peripherals": ", ".join(self.peripherals) if isinstance(self.peripherals, list) else ", ".join([f'{device}: {", ".join(peripherals)}' for device, peripherals in self.peripherals.items()]) if isinstance(self.peripherals, dict) else self.peripherals,
-			"Release": ", ".join([f'{device}: {date}' for device, date in self.release.items()]) if isinstance(self.release, dict) else self.release,
-			"Screen": ", ".join([f'{device}: {screen_data}' for device, screen_data in self.screen.items()]) if isinstance(self.screen, dict) else self.screen,
-			"SoC": ", ".join([f'{device}: {soc}' for device, soc in self.soc.items()]) if isinstance(self.soc, dict) else ", ".join(self.soc) if isinstance(self.soc, list) else self.soc,
+			"Peripherals": self._print_data(self.peripherals),
+			"Release": self._print_data(self.release),
+			"Screen": self._print_data(self.screen),
+			"SoC": self._print_data(self.soc),
 			"Device tree repository": f'{GITHUB_ORG_URL}/{self.tree}',
-			"Type": self.type,
-			"Vendor": self.vendor,
-			"Vendor (short)": self.vendor_short,
-			"Versions": ", ".join([f'{version}' for version in self.versions]),
+			"Type": self._print_data(self.type),
+			"Vendor": self._print_data(self.vendor),
+			"Vendor (short)": self._print_data(self.vendor_short),
+			"Versions": self._print_data(self.versions),
 		}
 
 		opt_infos = {
 			key: value for key, value in {
-				"Cameras": ", ".join([f'{camera}' for camera in self.cameras]) if isinstance(self.cameras, list) else self.cameras,
-				"Carrier": self.carrier,
-				"Custom recovery codename": self.custom_recovery_codename,
-				"Custom recovery link": self.custom_recovery_link,
-				"Custom unlock command": self.custom_unlock_cmd,
-				"Download boot": self.download_boot,
-				"Format on upgrade": self.format_on_upgrade,
-				"Has recovery partition": self.has_recovery_partition,
-				"Is A/B device": self.is_ab_device,
-				"Is unlockable": self.is_unlockable,
+				"Cameras": self._print_data(self.cameras),
+				"Carrier": self._print_data(self.carrier),
+				"Custom recovery codename": self._print_data(self.custom_recovery_codename),
+				"Custom recovery link": self._print_data(self.custom_recovery_link),
+				"Custom unlock command": self._print_data(self.custom_unlock_cmd),
+				"Download boot": self._print_data(self.download_boot),
+				"Format on upgrade": self._print_data(self.format_on_upgrade),
+				"Has recovery partition": self._print_data(self.has_recovery_partition),
+				"Is A/B device": self._print_data(self.is_ab_device),
+				"Is unlockable": self._print_data(self.is_unlockable),
 				"Models": ", ".join(self.models) if isinstance(self.models, list) else self.models,
-				"Network": ", ".join(self.network) if isinstance(self.network, list) else self.network,
-				"Recovery boot": self.recovery_boot,
-				"Required bootloader": self.required_bootloader,
-				"SD card": self.sdcard,
-				"Uses TWRP": self.uses_twrp,
+				"Network": self._print_data(self.network),
+				"Recovery boot": self._print_data(self.recovery_boot),
+				"Required bootloader": self._print_data(self.required_bootloader),
+				"SD card": self._print_data(self.sdcard),
+				"Uses TWRP": self._print_data(self.uses_twrp),
 			}.items()
 			if value is not None
 		}
 
 		return "\n".join([f"{key}: {value}" for key, value in {
 			**infos,
 			**opt_infos,
 		}.items()])
+
+	@staticmethod
+	def _print_data(data: Union[Any, List[Any], List[Dict[str, Any]], None]):
+		"""Return a string representation of the data."""
+		if isinstance(data, list):
+			if len(data) > 0 and isinstance(data[0], dict):
+				return "".join([
+					f"\n- {device}: {str(value)}"
+					for d in data
+					for device, value in d.items()
+				])
+			elif len(data) > 0 and isinstance(data[0], (complex, float, int, str)):
+				return ", ".join([str(value) for value in data])
+			else:
+				return "".join([f"\n - {value}" for value in data])
+		elif isinstance(data, dict):
+			return "".join([f"\n - {device}: {str(value)}" for device, value in data.items()])
+		else:
+			return str(data)
```

### Comparing `liblineage-1.3.1/pyproject.toml` & `liblineage-1.3.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "liblineage"
-version = "1.3.1"
+version = "1.3.2"
 description = "LineageOS utils library"
 authors = ["Sebastiano Barezzi <barezzisebastiano@gmail.com>"]
 license = "LGPL-3.0-or-later"
 readme = "README.md"
 repository = "https://github.com/sebaubuntu-python/liblineage"
 
 [tool.poetry.dependencies]
```

### Comparing `liblineage-1.3.1/PKG-INFO` & `liblineage-1.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liblineage
-Version: 1.3.1
+Version: 1.3.2
 Summary: LineageOS utils library
 Home-page: https://github.com/sebaubuntu-python/liblineage
 License: LGPL-3.0-or-later
 Author: Sebastiano Barezzi
 Author-email: barezzisebastiano@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
```

