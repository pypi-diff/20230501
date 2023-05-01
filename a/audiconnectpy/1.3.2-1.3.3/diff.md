# Comparing `tmp/audiconnectpy-1.3.2.tar.gz` & `tmp/audiconnectpy-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audiconnectpy-1.3.2.tar", last modified: Wed Apr 26 06:33:49 2023, max compression
+gzip compressed data, was "audiconnectpy-1.3.3.tar", last modified: Mon May  1 16:08:33 2023, max compression
```

## Comparing `audiconnectpy-1.3.2.tar` & `audiconnectpy-1.3.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:33:49.872015 audiconnectpy-1.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-26 06:33:37.000000 audiconnectpy-1.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-26 06:33:37.000000 audiconnectpy-1.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-04-26 06:33:49.872015 audiconnectpy-1.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-04-26 06:33:37.000000 audiconnectpy-1.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:33:49.872015 audiconnectpy-1.3.2/audiconnectpy/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-26 06:33:37.000000 audiconnectpy-1.3.2/audiconnectpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-04-26 06:33:37.000000 audiconnectpy-1.3.2/audiconnectpy/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    22874 2023-04-26 06:33:37.000000 audiconnectpy-1.3.2/audiconnectpy/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-04-26 06:33:37.000000 audiconnectpy-1.3.2/audiconnectpy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    29813 2023-04-26 06:33:37.000000 audiconnectpy-1.3.2/audiconnectpy/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    30468 2023-04-26 06:33:37.000000 audiconnectpy-1.3.2/audiconnectpy/services.py
--rw-r--r--   0 runner    (1001) docker     (123)    19549 2023-04-26 06:33:37.000000 audiconnectpy-1.3.2/audiconnectpy/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:33:49.872015 audiconnectpy-1.3.2/audiconnectpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-04-26 06:33:49.000000 audiconnectpy-1.3.2/audiconnectpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-26 06:33:49.000000 audiconnectpy-1.3.2/audiconnectpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 06:33:49.000000 audiconnectpy-1.3.2/audiconnectpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 06:33:49.000000 audiconnectpy-1.3.2/audiconnectpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-26 06:33:49.000000 audiconnectpy-1.3.2/audiconnectpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-04-26 06:33:37.000000 audiconnectpy-1.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 06:33:49.872015 audiconnectpy-1.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-04-26 06:33:48.000000 audiconnectpy-1.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:33:49.872015 audiconnectpy-1.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-26 06:33:37.000000 audiconnectpy-1.3.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:08:33.937215 audiconnectpy-1.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-01 16:08:09.000000 audiconnectpy-1.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-01 16:08:09.000000 audiconnectpy-1.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-05-01 16:08:33.937215 audiconnectpy-1.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-05-01 16:08:09.000000 audiconnectpy-1.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:08:33.937215 audiconnectpy-1.3.3/audiconnectpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-01 16:08:09.000000 audiconnectpy-1.3.3/audiconnectpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-05-01 16:08:09.000000 audiconnectpy-1.3.3/audiconnectpy/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22628 2023-05-01 16:08:09.000000 audiconnectpy-1.3.3/audiconnectpy/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-01 16:08:09.000000 audiconnectpy-1.3.3/audiconnectpy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27875 2023-05-01 16:08:09.000000 audiconnectpy-1.3.3/audiconnectpy/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30451 2023-05-01 16:08:09.000000 audiconnectpy-1.3.3/audiconnectpy/services.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-05-01 16:08:09.000000 audiconnectpy-1.3.3/audiconnectpy/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:08:33.937215 audiconnectpy-1.3.3/audiconnectpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-05-01 16:08:33.000000 audiconnectpy-1.3.3/audiconnectpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-01 16:08:33.000000 audiconnectpy-1.3.3/audiconnectpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 16:08:33.000000 audiconnectpy-1.3.3/audiconnectpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 16:08:33.000000 audiconnectpy-1.3.3/audiconnectpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-01 16:08:33.000000 audiconnectpy-1.3.3/audiconnectpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-01 16:08:09.000000 audiconnectpy-1.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 16:08:33.937215 audiconnectpy-1.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-05-01 16:08:27.000000 audiconnectpy-1.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:08:33.937215 audiconnectpy-1.3.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-01 16:08:09.000000 audiconnectpy-1.3.3/tests/__init__.py
```

### Comparing `audiconnectpy-1.3.2/LICENSE` & `audiconnectpy-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.3.2/PKG-INFO` & `audiconnectpy-1.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiconnectpy
-Version: 1.3.2
+Version: 1.3.3
 Summary: Provides asynchronous authentication and access to Audi Connect
 Home-page: https://github.com/cyr-ius/audiconnectpy/tree/master/audiconnectpy
 Author: cyr-ius
 Author-email: cyr-ius@ipocus.net
 License: GPL-3
 Keywords: connect,async
 Classifier: Programming Language :: Python
```

### Comparing `audiconnectpy-1.3.2/README.md` & `audiconnectpy-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.3.2/audiconnectpy/api.py` & `audiconnectpy-1.3.3/audiconnectpy/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 
 import logging
 
 from aiohttp import ClientSession
 
 from .auth import Auth
 from .exceptions import AudiException
-from .models import Vehicle
+from .models import Globals, Vehicle
 from .services import AudiService
-from .util import Globals
+from .util import ExtendedDict
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class AudiConnect:
     """Representation of an Audi Connect Account."""
 
@@ -51,16 +51,18 @@
         """Update data."""
         if not await self.async_login():
             return False
         # Update the state of all vehicles.
         try:
             if len(self._audi_vehicles) == 0:
                 vehicles_response = await self.services.async_get_vehicle_information()
-                for response in vehicles_response.get("userVehicles", {}):
-                    self._audi_vehicles.append(Vehicle(response, self.services))
+                for response in vehicles_response.getr("data.userVehicles", {}):
+                    self._audi_vehicles.append(
+                        Vehicle(ExtendedDict(response), self.services)
+                    )
             for vehicle in self._audi_vehicles:
                 await self._async_add_or_update_vehicle(vehicle, vinlist)
             return True
         except IOError as exception:
             # Force a re-login in case of failure/exception
             self.is_connected = False
             _LOGGER.exception(exception)
```

### Comparing `audiconnectpy-1.3.2/audiconnectpy/auth.py` & `audiconnectpy-1.3.3/audiconnectpy/auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 from .exceptions import (
     AudiException,
     HttpRequestError,
     ServiceNotFoundError,
     TimeoutExceededError,
 )
-from .util import get_attr, jload, json_loads
+from .util import json_loads
 
 TIMEOUT = 120
 DELAY = 10
 HDR_XAPP_VERSION = "4.13.0"
 HDR_USER_AGENT = "myAudi-Android/4.13.0 (Build 800238275.2210271555) Android/11"
 MARKET_URL = "https://content.app.my.audi.com/service/mobileapp/configurations"
 CLIENT_ID = "09b6cbec-cd19-4589-82fd-363dfa8c24da@apps_vw-dilab_com"
@@ -364,15 +364,15 @@
                 _LOGGER.error("Refresh token failed: %s", str(error))
 
     async def _async_retrieve_url_service(self) -> None:
         """Get urls for request."""
         # Get markets to get language
         markets_json = await self.request("GET", f"{MARKET_URL}/markets", None)
 
-        country_spec = get_attr(markets_json, "countries.countrySpecifications")
+        country_spec = markets_json.getr("countries.countrySpecifications")
         if self._country.upper() not in country_spec:
             raise AudiException("Country not found")
 
         self.language = country_spec.get(self._country.upper(), {}).get(
             "defaultLanguage"
         )
 
@@ -513,24 +513,22 @@
         }
         asz_req_data = {
             "token": access_token,
             "grant_type": "id_token",
             "stage": "live",
             "config": "myaudi",
         }
-        azs_token_rsptxt = await self.request(
+        azs_token_json = await self.request(
             "POST",
             self._audi_baseurl + "/token",
             json.dumps(asz_req_data),
             headers=headers,
             allow_redirects=False,
         )
-        azs_token_json = jload(azs_token_rsptxt)
         _LOGGER.debug("AZS Token: %s", azs_token_json)
-
         return azs_token_json
 
     async def _async_get_idk_token(self, **kwargs: Any) -> Any:
         """Get IDK Token."""
         refresh_token = kwargs.get("refresh_token")
         code = kwargs.get("code")
         code_verifier = kwargs.get("code_verifier")
@@ -557,22 +555,21 @@
                 "response_type": "token id_token",
                 "code_verifier": code_verifier,
             }
 
         # IDK token request
         encoded_idk_data = urlencode(idk_data, encoding="utf-8").replace("+", "%20")
 
-        idk_token_rsptxt = await self.post(
+        idk_token_json = await self.post(
             self._token_endpoint_url,
             encoded_idk_data,
             headers=headers,
             allow_redirects=False,
             use_json=False,
         )
-        idk_token_json = jload(idk_token_rsptxt)
         _LOGGER.debug("IDK Token: %s", idk_token_json)
 
         return idk_token_json
 
     async def _async_register_idk(self) -> Any:
         """Register IDK."""
         # mbboauth client register
@@ -586,21 +583,20 @@
             "client_name": "SM-A405FN",
             "platform": "google",
             "client_brand": "Audi",
             "appName": "myAudi",
             "appVersion": HDR_XAPP_VERSION,
             "appId": "de.myaudi.mobile.assistant",
         }
-        mbboauth_client_reg_rsptxt = await self.post(
+        mbboauth_client_reg_json = await self.post(
             self._mbb_baseurl + "/mobile/register/v1",
             mbboauth_reg_data,
             headers=headers,
             allow_redirects=False,
         )
-        mbboauth_client_reg_json = jload(mbboauth_client_reg_rsptxt)
         return mbboauth_client_reg_json.get("client_id")
 
     async def _async_get_mbb_token(self, **kwargs: Any) -> Any:
         """Authentification to IDK."""
         refresh_token = kwargs.get("refresh_token")
         id_token = kwargs.get("id_token")
         headers = {
@@ -624,18 +620,16 @@
                 "grant_type": "id_token",
                 "token": id_token,
                 "scope": "sc2:fal",
             }
         encoded_mbboauth_data = urlencode(mbboauth_data, encoding="utf-8").replace(
             "+", "%20"
         )
-        mbboauth_rsptxt = await self.post(
+        mbboauth_json = await self.post(
             self._mbb_baseurl + "/mobile/oauth2/v1/token",
             encoded_mbboauth_data,
             headers=headers,
             allow_redirects=False,
             use_json=False,
         )
-        mbboauth_json = jload(mbboauth_rsptxt)
         _LOGGER.debug("MBB Token: %s", mbboauth_json)
-
         return mbboauth_json
```

### Comparing `audiconnectpy-1.3.2/audiconnectpy/models.py` & `audiconnectpy-1.3.3/audiconnectpy/services.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,804 +1,731 @@
-"""Definition class."""
+"""Call url service."""
 from __future__ import annotations
 
+import asyncio
 import logging
-from dataclasses import dataclass
-from typing import TYPE_CHECKING, Any, Literal
-
-from .exceptions import HttpRequestError, ServiceNotFoundError, TimeoutExceededError
-from .util import get_attr, retry, set_attr
-
-if TYPE_CHECKING:
-    from .services import AudiService
-
+from datetime import datetime, timedelta
+from hashlib import sha512
+from typing import Any, Literal
+
+from .auth import Auth
+from .exceptions import AudiException, HttpRequestError, TimeoutExceededError
+from .models import (
+    ChargerDataResponse,
+    ClimaterDataResponse,
+    DestinationDataResponse,
+    HistoryDataResponse,
+    PositionDataResponse,
+    PreheaterDataResponse,
+    TripDataResponse,
+    UsersDataResponse,
+    VehicleDataResponse,
+)
+from .util import ExtendedDict, to_byte_array
+
+MAX_RESPONSE_ATTEMPTS = 10
+REQUEST_STATUS_SLEEP = 10
+
+SUCCEEDED = "succeeded"
+FAILED = "failed"
+REQUEST_SUCCESSFUL = "request_successful"
+REQUEST_FAILED = "request_failed"
 
 _LOGGER = logging.getLogger(__name__)
 
 
-class VehicleDataResponse:
-    """Status class."""
+class AudiService:
+    """Audi service."""
 
-    IDS = {
-        "0x0": "UNKNOWN",
-        "0x0101010001": "UTC_TIME",
-        "0x0101010002": "UTC_TIME_AND_KILOMETER_STATUS",
-        "0x0202": "ACTIVE_INSTRUMENT_CLUSTER_WARNING",
-        "0x0203010001": "MAINTENANCE_INTERVAL_DISTANCE_TO_OIL_CHANGE",
-        "0x0203010002": "MAINTENANCE_INTERVAL_TIME_TO_OIL_CHANGE",
-        "0x0203010003": "MAINTENANCE_INTERVAL_DISTANCE_TO_INSPECTION",
-        "0x0203010004": "MAINTENANCE_INTERVAL_TIME_TO_INSPECTION",
-        "0x0203010005": "WARNING_OIL_CHANGE",
-        "0x0203010006": "MAINTENANCE_INTERVAL_ALARM_INSPECTION",
-        "0x0203010007": "MAINTENANCE_INTERVAL_MONTHLY_MILEAGE",
-        "0x0204040001": "OIL_LEVEL_AMOUNT_IN_LITERS",
-        "0x0204040002": "OIL_LEVEL_MINIMUM_WARNING",
-        "0x0204040003": "OIL_LEVEL_DIPSTICKS_PERCENTAGE",
-        "0x0204040004": "OIL_DISPLAY",
-        "0x0204040005": "OIL_LEVEL_VALID",
-        "0x0204040006": "OIL_LEVEL_PERCENTAGE",
-        "0x02040C0001": "ADBLUE_RANGE",
-        "0x02040C0002": "SRC_NO_DRIVEABILITY",
-        "0x0301010001": "LIGHT_STATUS",
-        "0x0301020001": "TEMPERATURE_OUTSIDE",
-        "0x0301030001": "BRAKING_STATUS",
-        "0x0301030002": "STATE_OF_CHARGE",
-        "0x0301030003": "BEM_OK",
-        "0x0301030005": "TOTAL_RANGE",
-        "0x0301030006": "PRIMARY_RANGE",
-        "0x0301030007": "PRIMARY_DRIVE",
-        "0x0301030008": "SECONDARY_RANGE",
-        "0x0301030009": "SECONDARY_DRIVE",
-        "0x030103000A": "TANK_LEVEL_IN_PERCENTAGE",
-        "0x030103000D": "TANK_LEVEL_ERROR",
-        "0x0301040001": "LOCK_STATE_LEFT_FRONT_DOOR",
-        "0x0301040002": "OPEN_STATE_LEFT_FRONT_DOOR",
-        "0x0301040003": "SAFETY_STATE_LEFT_FRONT_DOOR",
-        "0x0301040004": "LOCK_STATE_LEFT_REAR_DOOR",
-        "0x0301040005": "OPEN_STATE_LEFT_REAR_DOOR",
-        "0x0301040006": "SAFETY_STATE_LEFT_REAR_DOOR",
-        "0x0301040007": "LOCK_STATE_RIGHT_FRONT_DOOR",
-        "0x0301040008": "OPEN_STATE_RIGHT_FRONT_DOOR",
-        "0x0301040009": "SAFETY_STATE_RIGHT_FRONT_DOOR",
-        "0x030104000A": "LOCK_STATE_RIGHT_REAR_DOOR",
-        "0x030104000B": "OPEN_STATE_RIGHT_REAR_DOOR",
-        "0x030104000C": "SAFETY_STATE_RIGHT_REAR_DOOR",
-        "0x030104000D": "LOCK_STATE_TRUNK_LID",
-        "0x030104000E": "OPEN_STATE_TRUNK_LID",
-        "0x030104000F": "SAFETY_STATE_TRUNK_LID",
-        "0x0301040010": "LOCK_STATE_HOOD",
-        "0x0301040011": "OPEN_STATE_HOOD",
-        "0x0301040012": "SAFETY_STATE_HOOD",
-        "0x0301050001": "STATE_LEFT_FRONT_WINDOW",
-        "0x0301050002": "POSITION_LEFT_FRONT_WINDOW",
-        "0x0301050003": "STATE_LEFT_REAR_WINDOW",
-        "0x0301050004": "POSITION_LEFT_REAR_WINDOW",
-        "0x0301050005": "STATE_RIGHT_FRONT_WINDOW",
-        "0x0301050006": "POSITION_RIGHT_FRONT_WINDOW",
-        "0x0301050007": "STATE_RIGHT_REAR_WINDOW",
-        "0x0301050008": "POSITION_RIGHT_REAR_WINDOW",
-        "0x0301050009": "STATE_DECK",
-        "0x030105000A": "POSITION_DECK",
-        "0x030105000B": "STATE_SUN_ROOF_MOTOR_COVER",
-        "0x030105000C": "POSITION_SUN_ROOF_MOTOR_COVER",
-        "0x030105000D": "STATE_SUN_ROOF_REAR_MOTOR_COVER_3",
-        "0x030105000E": "POSITION_SUN_ROOF_REAR_MOTOR_COVER_3",
-        "0x030105000F": "STATE_SERVICE_FLAP",
-        "0x0301050011": "STATE_SPOILER",
-        "0x0301050012": "POSITION_SPOILER",
-        "0x0301060001": "TYRE_PRESSURE_LEFT_FRONT_CURRENT_VALUE",
-        "0x0301060002": "TYRE_PRESSURE_LEFT_FRONT_DESIRED_VALUE",
-        "0x0301060003": "TYRE_PRESSURE_LEFT_REAR_CURRENT_VALUE",
-        "0x0301060004": "TYRE_PRESSURE_LEFT_REAR_DESIRED_VALUE",
-        "0x0301060005": "TYRE_PRESSURE_RIGHT_FRONT_CURRENT_VALUE",
-        "0x0301060006": "TYRE_PRESSURE_RIGHT_FRONT_DESIRED_VALUE",
-        "0x0301060007": "TYRE_PRESSURE_RIGHT_REAR_CURRENT_VALUE",
-        "0x0301060008": "TYRE_PRESSURE_RIGHT_REAR_DESIRED_VALUE",
-        "0x0301060009": "TYRE_PRESSURE_SPARE_TYRE_CURRENT_VALUE",
-        "0x030106000A": "TYRE_PRESSURE_SPARE_TYRE_DESIRED_VALUE",
-        "0x030106000B": "TYRE_PRESSURE_LEFT_FRONT_TYRE_DIFFERENCE",
-        "0x030106000C": "TYRE_PRESSURE_LEFT_REAR_TYRE_DIFFERENCE",
-        "0x030106000D": "TYRE_PRESSURE_RIGHT_FRONT_TYRE_DIFFERENCE",
-        "0x030106000E": "TYRE_PRESSURE_RIGHT_REAR_TYRE_DIFFERENCE",
-        "0x030106000F": "TYRE_PRESSURE_SPARE_TYRE_DIFFERENCE",
-    }
+    brand = "Audi"
+    _home_region: dict[str, str] = {}
+    _home_region_setter: dict[str, str] = {}
+    _heater_source: dict[str, Literal["electric", "auxiliary", "automatic"]] = {}
+    _control_duration: dict[str, int] = {}
 
-    def __init__(self, data: dict[str, str], has_pin: bool = False) -> None:
+    def __init__(self, auth: Auth, country: str, spin: int) -> None:
         """Initialize."""
-        self.data: dict[str, Any] = data
-        self.has_pin = has_pin
-        self.measure_time = None
-        self.send_time = None
-        self.send_time_utc = None
-        self.measure_mileage = None
-        self.send_mileage = None
-        self._vehicle_data = self._get_attributes()
-
-    @property
-    def is_supported(self) -> bool:
-        """Supported status."""
-        return self.attributes is not None
-
-    @property
-    def attributes(self) -> Any:
-        """Attributes properties."""
-        return self._vehicle_data
-
-    def _get_attributes(self) -> dict[str, dict[str, Any]]:
-        _attributes: dict[str, Any] = {}
-
-        default = get_attr(
-            self.data, "CurrentVehicleDataByRequestResponse.vehicleData.data"
-        )
-        vehicle_data = get_attr(
-            self.data, "StoredVehicleDataResponse.vehicleData.data", default
-        )
-        if vehicle_data is None:
-            return _attributes
-
-        for raw_data in vehicle_data:
-            for raw_field in raw_data.get("field", {}):
-                ids = raw_field.get("id")
-                value = raw_field.get("value")
-                unit = raw_field.get("unit")
-                if ids == "0x0101010001":
-                    self.measure_time = raw_field.get("tsCarCaptured")
-                    self.send_time = raw_field.get("tsCarSent")
-                    self.send_time_utc = raw_field.get("tsCarSentUtc")
-                    self.measure_mileage = raw_field.get("milCarCaptured")
-                    self.send_mileage = raw_field.get("milCarSent")
-                    _attributes.update(set_attr("LAST_UPDATE_TIME", self.send_time_utc))
-
-                if identity := self.IDS.get(ids):
-                    _attributes.update(set_attr(identity, value, unit))
-                else:
-                    _LOGGER.error("%s not found", ids)
-
-        # Append meta sensors
-        _attributes.update(self._metadatas(_attributes))
-
-        return _attributes
-
-    @staticmethod
-    def _metadatas(attributes: dict[str, dict[str, Any]]) -> dict[Any, dict[str, Any]]:
-        _metadatas = {}
-        _attributes = attributes
-        trunk_open = get_attr(_attributes, "trunk_open") is not None
-        trunk_unlocked = get_attr(_attributes, "trunk_unlocked") is not None
-
-        # Windows open status
-        left_check = get_attr(_attributes, "open_left_front_windows.value")
-        left_rear_check = get_attr(_attributes, "open_left_rear_windows.value")
-        right_check = get_attr(_attributes, "open_right_front_windows.value")
-        right_rear_check = get_attr(_attributes, "open_right_rear_windows.value")
-        any_window_open = (
-            left_check and left_rear_check and right_check and right_rear_check
-        )
-        if (
-            left_check is not None
-            and left_rear_check is not None
-            and right_check is not None
-            and right_rear_check is not None
-        ):
-            _metadatas.update(set_attr("ANY_WINDOW_OPEN", any_window_open))
-
-        # Doors open status
-        left_check = get_attr(_attributes, "unlock_left_front_door.value")
-        left_rear_check = get_attr(_attributes, "unlock_left_rear_door.value")
-        right_check = get_attr(_attributes, "unlock_right_front_door.value")
-        right_rear_check = get_attr(_attributes, "unlock_right_rear_door.value")
-        any_door_unlocked = (
-            left_check and left_rear_check and right_check and right_rear_check
-        )
-        if bool_any_door_unlocked := (
-            left_check is not None
-            and left_rear_check is not None
-            and right_check is not None
-            and right_rear_check is not None
-        ):
-            _metadatas.update(set_attr("ANY_DOOR_UNLOCKED", any_door_unlocked))
-
-        # Doors open status
-        left_check = get_attr(_attributes, "open_left_front_door.value")
-        left_rear_check = get_attr(_attributes, "open_left_rear_door.value")
-        right_check = get_attr(_attributes, "open_right_front_door.value")
-        right_rear_check = get_attr(_attributes, "open_right_rear_door.value")
-        any_door_open = (
-            left_check and left_rear_check and right_check and right_rear_check
-        )
-        if bool_any_door_open := (
-            left_check is not None
-            and left_rear_check is not None
-            and right_check is not None
-            and right_rear_check is not None
-        ):
-            _metadatas.update(set_attr("ANY_DOOR_OPEN", any_door_open))
-
-        # Door trunk status
-        if (
-            bool_any_door_open
-            and bool_any_door_unlocked
-            and trunk_open
-            and trunk_unlocked
-        ):
-            if any_door_open and trunk_open:
-                _metadatas.update(set_attr("DOORS_TRUNK_STATUS", "Open"))
-            elif any_door_unlocked and trunk_unlocked:
-                _metadatas.update(set_attr("DOORS_TRUNK_STATUS", "Closed"))
-            else:
-                _metadatas.update(set_attr("DOORS_TRUNK_STATUS", "Locked"))
-
-        # Tyre pressure status
-        left_check = get_attr(_attributes, "tyre_pressure_left_front.value")
-        left_rear_check = get_attr(_attributes, "tyre_pressure_left_rear.value")
-        right_check = get_attr(_attributes, "tyre_pressure_right_front.value")
-        right_rear_check = get_attr(_attributes, "tyre_pressure_right_rear.value")
-        spare_check = get_attr(_attributes, "tyre_pressure_spare.value")
-        any_tyre_pressure = (
-            left_check
-            and left_rear_check
-            and right_check
-            and right_rear_check
-            and spare_check
-        )
-        if (
-            left_check is not None
-            and left_rear_check is not None
-            and right_check is not None
-            and right_rear_check is not None
-            and spare_check is not None
-        ):
-            _metadatas.update(set_attr("ANY_TYRE_PRESSURE", any_tyre_pressure))
-
-        return _metadatas
-
-
-@dataclass
-class PreheaterDataResponse:
-    """Preheater class."""
-
-    data: dict[str, Any]
-
-    @property
-    def is_supported(self) -> bool:
-        """Supported status."""
-        return self.attributes is not None
-
-    @property
-    def attributes(self) -> dict[Any, dict[str, Any]]:
-        """Attributes properties."""
-        _attributes = {}
-        report = get_attr(self.data, "statusResponse.climatisationStateReport")
-        if report:
-            _attributes.update(set_attr("PREHEATER_STATE", report))
-            _attributes.update(
-                set_attr("PREHEATER_ACTIVE", report.get("climatisationState"))
-            )
-            _attributes.update(
-                set_attr("PREHEATER_DURATION", report.get("climatisationDuration"))
-            )
-            _attributes.update(
-                set_attr("PREHEATER_REMAINING", report.get("remainingClimateTime"))
-            )
-
-        return _attributes
-
-
-@dataclass
-class ChargerDataResponse:
-    """Charger class."""
-
-    data: dict[str, Any]
-
-    @property
-    def is_supported(self) -> bool:
-        """Supported status."""
-        return (
-            get_attr(self.data, "charger.settings") is not None
-            or get_attr(self.data, "charger.status") is not None
-        )
-
-    @property
-    def attributes(self) -> dict[Any, dict[str, Any]]:
-        """Attributes properties."""
-        _attributes = {}
-        _settings = get_attr(self.data, "charger.settings")
-        _status = get_attr(self.data, "charger.status")
-        _charging_status = get_attr(self.data, "charger.status.chargingStatusData")
-        _cruising_status = get_attr(self.data, "charger.status.cruisingRangeStatusData")
-
-        _attributes.update(
-            set_attr(
-                "MAX_CHARGE_CURRENT", get_attr(_settings, "maxChargeCurrent.content")
-            )
-        )
-        _attributes.update(
-            set_attr(
-                "CHARGING_STATE", get_attr(_charging_status, "chargingState.content")
-            )
-        )
-        _attributes.update(
-            set_attr(
-                "ACTUAL_CHARGE_RATE",
-                get_attr(_charging_status, "actualChargeRate.content"),
-            )
-        )
-        _attributes.update(
-            set_attr(
-                "ACTUAL_CHARGE_RATE_UNIT",
-                get_attr(_charging_status, "chargeRateUnit.content"),
-            )
-        )
-        _attributes.update(
-            set_attr(
-                "CHARGING_POWER", get_attr(_charging_status, "chargingPower.content")
-            )
-        )
-        _attributes.update(
-            set_attr(
-                "CHARGING_MODE", get_attr(_charging_status, "chargingMode.content")
-            )
-        )
-        _attributes.update(
-            set_attr("ENERGY_FLOW", get_attr(_charging_status, "energyFlow.content"))
-        )
-        _attributes.update(
-            set_attr(
-                "PRIMARY_ENGINE_TYPE",
-                get_attr(_cruising_status, "engineTypeFirstEngine.content"),
-            )
-        )
-        _attributes.update(
-            set_attr(
-                "SECONDARY_ENGINE_TYPE",
-                get_attr(_cruising_status, "engineTypeSecondEngine.content"),
-            )
-        )
-        _attributes.update(
-            set_attr("HYBRID_RANGE", get_attr(_cruising_status, "hybridRange.content"))
-        )
-        _attributes.update(
-            set_attr(
-                "PRIMARY_ENGINE_RANGE",
-                get_attr(_cruising_status, "primaryEngineRange.content"),
-            )
-        )
-        _attributes.update(
-            set_attr(
-                "SECONDARY_ENGINE_RANGE",
-                get_attr(_cruising_status, "secondaryEngineRange.content"),
-            )
-        )
-        _attributes.update(
-            set_attr(
-                "STATE_OF_CHARGE",
-                get_attr(_status, "batteryStatusData.stateOfCharge.content"),
-            )
-        )
-        _attributes.update(
-            set_attr(
-                "PLUG_STATE", get_attr(_status, "plugStatusData.plugState.content")
-            )
-        )
-        _attributes.update(
-            set_attr("PLUG_LOCK", get_attr(_status, "plugStatusData.lockState.content"))
+        self._auth = auth
+        self.country: str = "DE" if country is None else country
+        self._spin = spin
+
+    async def async_get_vehicles(self) -> Any:
+        """Get all vehicles."""
+        url = await self._async_get_home_region("")
+        data = await self._auth.get(
+            f"{url}/usermanagement/users/v1/{self.brand}/{self.country}/vehicles"
+        )
+        return data
+
+    async def async_get_vehicle_details(self, vin: str) -> Any:
+        """Get vehicle data."""
+        url = await self._async_get_home_region(vin.upper())
+        accept = {
+            "Accept": "application/vnd.vwg.mbb.vehicleDataDetail_v2_1_0+json, application/vnd.vwg.mbb.genericError_v1_0_2+json"
+        }
+        headers = await self._auth.async_get_headers(token_type="mbb", headers=accept)
+        data = await self._auth.get(
+            f"{url}/vehicleMgmt/vehicledata/v2/{self.brand}/{self.country}/vehicles/{vin.upper()}/",
+            headers=headers,
+        )
+        return data
+
+    async def async_get_vehicle(self, vin: str) -> VehicleDataResponse:
+        """Get store data."""
+        url = await self._async_get_home_region(vin.upper())
+        data = await self._auth.get(
+            f"{url}/bs/vsr/v1/{self.brand}/{self.country}/vehicles/{vin.upper()}/status"
+        )
+        return VehicleDataResponse(data, self._spin is not None)
+
+    async def async_refresh_vehicle_data(self, vin: str) -> None:
+        """Refresh vehicle data."""
+        url = await self._async_get_home_region(vin.upper())
+        data = await self._auth.post(
+            f"{url}/bs/vsr/v1/{self.brand}/{self.country}/vehicles/{vin.upper()}/requests"
+        )
+        request_id: str = data.getr("CurrentVehicleDataResponse.requestId")
+        await self.async_check_request_succeeded(
+            f"{url}/bs/vsr/v1/{self.brand}/{self.country}/vehicles/{vin.upper()}/requests/{request_id}/jobstatus",
+            "refresh vehicle data",
+            REQUEST_SUCCESSFUL,
+            REQUEST_FAILED,
+            "requestStatusResponse.status",
+        )
+
+    async def async_get_stored_position(self, vin: str) -> PositionDataResponse:
+        """Get position data."""
+        url = await self._async_get_home_region(vin.upper())
+        data = await self._auth.get(
+            f"{url}/bs/cf/v1/{self.brand}/{self.country}/vehicles/{vin.upper()}/position"
+        )
+        return PositionDataResponse(data)
+
+    async def async_get_destinations(self, vin: str) -> DestinationDataResponse:
+        """Get destination data."""
+        url = await self._async_get_home_region(vin.upper())
+        data = await self._auth.get(
+            f"{url}/destinationfeedservice/mydestinations/v1/{self.brand}/{self.country}/vehicles/{vin.upper()}/destinations"
+        )
+        return DestinationDataResponse(data)
+
+    async def async_get_history(self, vin: str) -> HistoryDataResponse:
+        """Get history data."""
+        url = await self._async_get_home_region(vin.upper())
+        data = await self._auth.get(
+            f"{url}/bs/dwap/v1/{self.brand}/{self.country}/vehicles/{vin.upper()}/history"
+        )
+        return HistoryDataResponse(data)
+
+    async def async_get_vehicule_users(self, vin: str) -> UsersDataResponse:
+        """Get ufers of vehicle."""
+        url = await self._async_get_home_region(vin.upper())
+        data = await self._auth.get(f"{url}/bs/uic/v1/{vin.upper()}/users")
+        return UsersDataResponse(data)
+
+    async def async_get_charger(self, vin: str) -> ChargerDataResponse:
+        """Get charger data."""
+        url = await self._async_get_home_region(vin.upper())
+        data = await self._auth.get(
+            f"{url}/bs/batterycharge/v1/{self.brand}/{self.country}/vehicles/{vin.upper()}/charger"
+        )
+        return ChargerDataResponse(data)
+
+    async def async_get_tripdata(
+        self, vin: str, kind: Literal["short", "long", "cyclic"]
+    ) -> tuple[TripDataResponse, TripDataResponse]:
+        """Get trip data."""
+        if kind not in ["short", "long", "cyclic"]:
+            raise AudiException(f"Syntax error, {kind} must be 'short'|'long|'cyclic'")
+        kind.replace("short", "shortTerm").replace("long", "longTerm")
+        url = await self._async_get_home_region(vin.upper())
+        params = {
+            "type": "list",
+            "from": "1970-01-01T00:00:00Z",
+            # "from":(datetime.utcnow() - timedelta(days=365)).strftime("%Y-%m-%dT%H:%M:%SZ"),
+            "to": (datetime.utcnow() + timedelta(minutes=90)).strftime(
+                "%Y-%m-%dT%H:%M:%SZ"
+            ),
+        }
+        data = await self._auth.get(
+            f"{url}/bs/tripstatistics/v1/{self.brand}/{self.country}/vehicles/{vin.upper()}/tripdata/{kind}",
+            params=params,
+        )
+        td_sorted = sorted(
+            data.getr("tripDataList.tripData"),
+            key=lambda k: k["overallMileage"],  # type: ignore[no-any-return]
+            reverse=True,
+        )
+        td_current = td_sorted[0]
+        td_reset_trip = {}
+
+        for trip in td_sorted:
+            if (td_current["startMileage"] - trip["startMileage"]) > 2:
+                td_reset_trip = trip
+                break
+            td_current["tripID"] = trip["tripID"]
+            td_current["startMileage"] = trip["startMileage"]
+
+        return TripDataResponse(ExtendedDict(td_current)), TripDataResponse(
+            ExtendedDict(td_reset_trip)
+        )
+
+    async def async_get_operations_list(self, vin: str) -> Any:
+        """Get operation data."""
+        url = await self._async_get_home_region_setter(vin.upper())
+        data = await self._auth.get(
+            f"{url}/rolesrights/operationlist/v3/vehicles/{vin.upper()}"
+        )
+        return data
+
+    async def async_get_climater(self, vin: str) -> ClimaterDataResponse:
+        """Get climater data."""
+        url = await self._async_get_home_region(vin.upper())
+        data = await self._auth.get(
+            f"{url}/bs/climatisation/v1/{self.brand}/{self.country}/vehicles/{vin.upper()}/climater"
+        )
+        return ClimaterDataResponse(data)
+
+    async def async_get_preheater(self, vin: str) -> PreheaterDataResponse:
+        """Get Heater/Ventilation data."""
+        url = await self._async_get_home_region(vin.upper())
+        data = await self._auth.get(
+            f"{url}/bs/rs/v1/{self.brand}/{self.country}/vehicles/{vin.upper()}/status"
+        )
+        return PreheaterDataResponse(data)
+
+    async def async_get_climater_timer(self, vin: str) -> Any:
+        """Get timer."""
+        url = await self._async_get_home_region(vin.upper())
+        data = await self._auth.get(
+            f"{url}/bs/departuretimer/v1/{self.brand}/{self.country}/vehicles/{vin.upper()}/timer"
+        )
+        return data
+
+    async def async_get_capabilities(self, vin: str) -> VehicleDataResponse:
+        """Get capabilities."""
+        url = "https://emea.bff.cariad.digital"
+        headers = await self._auth.async_get_headers(token_type="idk")
+        data = await self._auth.get(
+            f"{url}/vehicle/v1/vehicles/{vin.upper()}/capabilities", headers=headers
+        )
+        return VehicleDataResponse(data, self._spin is not None)
+
+    async def async_get_vehicle_information(self) -> Any:
+        """Get vehicle information."""
+        headers = await self._auth.async_get_headers(
+            token_type="audi",
+            headers={
+                "Accept-Language": f"{self._auth.language}-{self.country.upper()}",
+                "Content-Type": "application/json",
+                "X-User-Country": self.country.upper(),
+            },
         )
-        _attributes.update(
-            set_attr(
-                "REMAINING_CHARGING_TIME",
-                get_attr(_status, "batteryStatusData.remainingChargingTime.content"),
-            )
+        data = {
+            "query": "query vehicleList {\n userVehicles {\n vin\n mappingVin\n vehicle { core { modelYear\n }\n media { shortName\n longName }\n }\n csid\n commissionNumber\n type\n devicePlatform\n mbbConnect\n userRole {\n role\n }\n vehicle {\n classification {\n driveTrain\n }\n }\n nickname\n }\n}"
+        }
+        resp = await self._auth.post(
+            "https://app-api.live-my.audi.com/vgql/v1/graphql",
+            data=data,
+            headers=headers,
+            allow_redirects=False,
+        )
+        if "data" not in resp:
+            raise AudiException("Invalid json in vehicle information")
+        return resp
+
+    async def async_get_honkflash(self, vin: str) -> Any:
+        """Get Honk & Flash status."""
+        url = await self._async_get_home_region(vin.upper())
+        data = await self._auth.get(
+            f"{url}/bs/rhf/v1/{self.brand}/{self.country}/configuration"
+        )
+        return data
+
+    async def async_get_personal_data(self) -> Any:
+        """Get Honk & Flash status."""
+        url = f"{self._auth.profil_url}/customers/{self._auth.user_id}"
+        headers = await self._auth.async_get_headers(token_type="idk")
+        data = await self._auth.get(f"{url}/personalData", headers=headers)
+        return data
+
+    async def async_get_real_car_data(self) -> Any:
+        """Get Honk & Flash status."""
+        url = f"{self._auth.profil_url}/customers/{self._auth.user_id}"
+        headers = await self._auth.async_get_headers(token_type="idk")
+        data = await self._auth.get(f"{url}/realCarData", headers=headers)
+        return data
+
+    async def async_get_mbb_status(self) -> Any:
+        """Get Honk & Flash status."""
+        url = f"{self._auth.profil_url}/customers/{self._auth.user_id}"
+        headers = await self._auth.async_get_headers(token_type="idk")
+        data = await self._auth.get(f"{url}/mbbStatusData", headers=headers)
+        return data
+
+    async def async_get_identity_data(self) -> Any:
+        """Get Honk & Flash status."""
+        url = f"{self._auth.profil_url}/customers/{self._auth.user_id}"
+        headers = await self._auth.async_get_headers(token_type="idk")
+        data = await self._auth.get(f"{url}/identityData", headers=headers)
+        return data
+
+    # async def async_get_users(self, vin: str) -> Any:
+    #     """Get users."""
+    #     url = "https://userinformationservice.apps.emea.vwapps.io/iaa"
+    #     headers = await self._auth.async_get_headers(token_type="idk")
+    #     data = await self._auth.get(f"{url}/uic/v1/vin/{vin.upper()}/users", headers=headers)
+    #     return data
+
+    async def async_get_fences(self, vin: str) -> Any:
+        """Get fences."""
+        url = await self._async_get_home_region(vin.upper())
+        data = await self._auth.get(
+            f"{url}/bs/geofencing/v1/{self.brand}/{self.country}/vehicles/{vin.upper()}/geofencingAlerts"
+        )
+        return data
+
+    async def async_get_fences_config(self, vin: str) -> Any:
+        """Get fences configuration."""
+        url = await self._async_get_home_region(vin.upper())
+        data = await self._auth.get(
+            f"{url}/bs/geofencing/v1/{self.brand}/{self.country}/vehicles/{vin.upper()}/geofencingConfiguration"
+        )
+        return data
+
+    async def async_get_speed_alert(self, vin: str) -> Any:
+        """Get speed alert."""
+        url = await self._async_get_home_region(vin.upper())
+        data = await self._auth.get(
+            f"{url}/bs/speedalert/v1/{self.brand}/{self.country}/vehicles/{vin.upper()}/speedAlerts"
+        )
+        return data
+
+    async def async_get_speed_config(self, vin: str) -> Any:
+        """Get speed alert configuration."""
+        url = await self._async_get_home_region(vin.upper())
+        data = await self._auth.get(
+            f"{url}/bs/speedalert/v1/{self.brand}/{self.country}/vehicles/{vin.upper()}/speedAlertConfiguration"
+        )
+        return data
+
+    async def async_lock(self, vin: str, lock: bool) -> None:
+        """Set lock."""
+        # OpenHab "lock","unlock"
+        url = await self._async_get_home_region(vin.upper())
+        data = '<?xml version="1.0" encoding= "UTF-8" ?>'
+        data += f'<rluAction xmlns="http://audi.de/connect/rlu"><action>{"lock" if lock else "unlock"}</action></rluAction>'
+        headers = await self._auth.async_get_headers(
+            token_type="idk",
+            headers={
+                "Content-Type": "application/vnd.vwg.mbb.RemoteLockUnlock_v1_0_0+xml"
+            },
+            security_token=await self._async_get_security_token(
+                vin, "rlu_v1/operations/" + ("LOCK" if lock else "UNLOCK")
+            ),
+        )
+
+        rsp = await self._auth.post(
+            f"{url}/bs/rlu/v1/{self.brand}/{self.country}/vehicles/{vin.upper()}/actions",
+            headers=headers,
+            data=data,
+            use_json=False,
+        )
+
+        request_id = rsp.getr("rluActionResponse.requestId")
+        await self.async_check_request_succeeded(
+            f"{url}/bs/rlu/v1/{self.brand}/{self.country}/vehicles/{vin.upper()}/requests/{request_id}/status",
+            "lock vehicle" if lock else "unlock vehicle",
+            REQUEST_SUCCESSFUL,
+            REQUEST_FAILED,
+            "requestStatusResponse.status",
+        )
+
+    async def async_climater(self, vin: str, start: bool) -> None:
+        """Set Climatisation."""
+        # OpenHab "startClimatisation","stopClimatisation"
+        url = await self._async_get_home_region(vin.upper())
+        heater_source = self._heater_source.get(vin, "electric")
+        action = (
+            "P_START_CLIMA_EL" if heater_source == "electric" else "P_START_CLIMA_AU"
+        )
+        security_token = await self._async_get_security_token(
+            vin, "rclima_v1/operations/" + (action if start else "P_QSTOPACT")
+        )
+        data = '<?xml version="1.0" encoding= "UTF-8" ?>'
+        data += f'<action><type>{"startClimatisation" if start else "stopClimatisation"}</type>'
+        data += f"<settings><heaterSource>{heater_source}</heaterSource></settings></action>"
+        headers = await self._auth.async_get_action_headers(
+            "application/vnd.vwg.mbb.ClimaterAction_v1_0_0+xml", security_token
+        )
+
+        # headers = await self._auth.async_get_action_headers(
+        #     "application/vnd.vwg.mbb.ClimaterAction_v1_0_2+json", security_token
+        # )
+        # data = (
+        #     {
+        #         "action": {
+        #             "type": "startClimatisation",
+        #             "settings": {
+        #                 "climatisationWithoutHVpower": "without_hv_power",
+        #                 "heaterSource": heater_source,
+        #             },
+        #         }
+        #     }
+        #     if start
+        #     else {"action": {"type": "stopClimatisation"}}
+        # )
+
+        rsp = await self._auth.post(
+            f"{url}/bs/climatisation/v1/{self.brand}/{self.country}/vehicles/{vin.upper()}/climater/actions",
+            headers=headers,
+            data=data,
+            use_json=False,
+        )
+        actionid = rsp.getr("action.actionId")
+        await self.async_check_request_succeeded(
+            f"{url}/bs/climatisation/v1/{self.brand}/{self.country}/vehicles/{vin.upper()}/climater/actions/{actionid}",
+            "start climatisation" if start else "stop climatisation",
+            SUCCEEDED,
+            FAILED,
+            "action.actionState",
+        )
+
+    async def async_climater_temp(self, vin: str, temperature: float = 19.5) -> None:
+        """Set Climatisation temperature."""
+        temperature = int(round(temperature, 1) * 10 + 2731)
+        url = await self._async_get_home_region(vin.upper())
+        heater_source = self._heater_source.get(vin, "electric")
+        data = '<?xml version="1.0" encoding= "UTF-8" ?>'
+        data += f"<action><type>setSettings</type><settings><targetTemperature>{temperature}</targetTemperature>"
+        data += "<climatisationWithoutHVpower>false</climatisationWithoutHVpower>"
+        data += f"<heaterSource>{heater_source}</heaterSource></settings></action>"
+        headers = await self._auth.async_get_action_headers(
+            "application/vnd.vwg.mbb.ClimaterAction_v1_0_0+xml", None
+        )
+        # data = json.dumps(
+        #     {
+        #         "action": {
+        #             "type": "setSettings",
+        #             "settings": {
+        #                 "targetTemperature": temperature,
+        #                 "climatisationWithoutHVpower": True,
+        #                 "heaterSource": heater_source,
+        #                 "climaterElementSettings": {
+        #                     "isClimatisationAtUnlock": False,
+        #                     "isMirrorHeatingEnabled": True,
+        #                 },
+        #             },
+        #         }
+        #     }
+        # )
+        # headers = await self._auth.async_get_action_headers("application/json", None)
+        rsp = await self._auth.post(
+            f"{url}/bs/climatisation/v1/{self.brand}/{self.country}/vehicles/{vin.upper()}/climater/actions",
+            headers=headers,
+            data=data,
+            use_json=False,
+        )
+        actionid = rsp.getr("action.actionId")
+        await self.async_check_request_succeeded(
+            f"{url}/bs/climatisation/v1/{self.brand}/{self.country}/vehicles/{vin.upper()}/climater/actions/{actionid}",
+            "set target temperature",
+            SUCCEEDED,
+            FAILED,
+            "action.actionState",
+        )
+
+    async def async_pre_heating(self, vin: str, start: bool) -> None:
+        """Set pre heater."""
+        # OpenHab "startPreHeat","stopPreHeat"
+        url = await self._async_get_home_region(vin.upper())
+        security_token = await self._async_get_security_token(
+            vin, "rheating_v1/operations/" + ("P_QSACT" if start else "P_QSTOPACT")
+        )
+        # duration = self._control_duration.get(vin, 60)
+        data = '<?xml version="1.0" encoding= "UTF-8" ?>'
+        data += '<performAction xmlns="http://audi.de/connect/rs">'
+        data += f'<quickstart><active>{"true" if start else "false"}</active></quickstart></performAction>'
+        headers = await self._auth.async_get_action_headers(
+            "application/vnd.vwg.mbb.RemoteStandheizung_v2_0_0+xml", security_token
+        )
+
+        # headers = await self._auth.async_get_action_headers(
+        #     "application/vnd.vwg.mbb.RemoteStandheizung_v2_0_2+json", security_token
+        # )
+        # data = (
+        #     {
+        #         "performAction": {
+        #             "quickstart": {
+        #                 "startMode": "heating",
+        #                 "active": True,
+        #                 "climatisationDuration": duration,
+        #             }
+        #         }
+        #     }
+        #     if start
+        #     else {"performAction": {"quickstop": {"active": False}}}
+        # )
+
+        await self._auth.post(
+            f"{url}/bs/rs/v1/{self.brand}/{self.country}/vehicles/{vin.upper()}/action",
+            headers=headers,
+            data=data,
+            use_json=False,
+        )
+
+    async def async_ventilation(self, vin: str, start: bool) -> None:
+        """Set ventilation."""
+        # OpenHab "startVentilation","stopVentilation"
+        url = await self._async_get_home_region(vin.upper())
+        duration = self._control_duration.get(vin, 60)
+        security_token = await self._async_get_security_token(
+            vin, "rheating_v1/operations/" + ("P_QSACT" if start else "P_QSTOPACT")
+        )
+        # data = '<?xml version="1.0" encoding= "UTF-8" ?>'
+        # data += '<performAction xmlns="http://audi.de/connect/rs">'
+        # data += f'<quickstart><active>{"true" if start else "false"}</active>'
+        # data += (
+        #     f"<climatisationDuration>{self._control_duration}</climatisationDuration>"
+        # )
+        # data += " <startMode>ventilation</startMode></quickstart></performAction>"
+        # headers = await self._auth.async_get_action_headers(
+        #     "application/vnd.vwg.mbb.RemoteStandheizung_v2_0_0+xml", security_token
+        # )
+
+        headers = await self._auth.async_get_action_headers(
+            "application/vnd.vwg.mbb.RemoteStandheizung_v2_0_2+json", security_token
+        )
+        data = (
+            {
+                "performAction": {
+                    "quickstart": {
+                        "startMode": "ventilation",
+                        "active": True,
+                        "climatisationDuration": duration,
+                    }
+                }
+            }
+            if start
+            else {"performAction": {"quickstop": {"active": False}}}
         )
 
-        return _attributes
-
-
-@dataclass
-class ClimaterDataResponse:
-    """Climater class."""
-
-    data: dict[str, Any]
-
-    @property
-    def is_supported(self) -> bool:
-        """Supported status."""
-        return self.attributes is not None
-
-    @property
-    def attributes(self) -> dict[Any, dict[str, Any]]:
-        """Attributes properties."""
-        _attributes = {}
-        _settings = get_attr(self.data, "climater.settings")
-        _status = get_attr(self.data, "climater.status")
-        _attributes.update(
-            set_attr(
-                "CLIMATISATION_STATE",
-                get_attr(
-                    _status,
-                    "climatisationStatusData.climatisationState.content",
-                ),
-            )
-        )
-        _attributes.update(
-            set_attr(
-                "OUTDOOR_TEMPERATURE",
-                get_attr(
-                    _status,
-                    "temperatureStatusData.outdoorTemperature.content",
-                ),
-            )
-        )
-        _attributes.update(
-            set_attr(
-                "CLIMATISATION_HEATER_SRC",
-                get_attr(_settings, "heaterSource.content"),
-            )
+        await self._auth.post(
+            f"{url}/bs/rs/v1/{self.brand}/{self.country}/vehicles/{vin.upper()}/action",
+            headers=headers,
+            data=data,
+            use_json=True,
+        )
+
+    async def async_charger(self, vin: str, start: bool) -> None:
+        """Set charger."""
+        # OpenHab "startCharging","stopCharging"
+        url = await self._async_get_home_region(vin.upper())
+        data = '<?xml version="1.0" encoding= "UTF-8" ?>'
+        data += f'<action><type>{"true" if start else "false"}</type></action>'
+        headers = await self._auth.async_get_action_headers(
+            "application/vnd.vwg.mbb.ChargerAction_v1_0_0+xml", None
+        )
+        rsp = await self._auth.post(
+            f"{url}/bs/batterycharge/v1/{self.brand}/{self.country}/vehicles/{vin.upper()}/charger/actions",
+            headers=headers,
+            data=data,
+            use_json=False,
+        )
+
+        actionid = rsp.getr("action.actionId")
+        await self.async_check_request_succeeded(
+            f"{url}/bs/batterycharge/v1/{self.brand}/{self.country}/vehicles/{vin.upper()}/charger/actions/{actionid}",
+            "start charger" if start else "stop charger",
+            SUCCEEDED,
+            FAILED,
+            "action.actionState",
+        )
+
+    async def async_set_charger_max(self, vin: str, current: float = 32) -> None:
+        """Set max current."""
+        url = await self._async_get_home_region(vin.upper())
+        data = '<?xml version="1.0" encoding= "UTF-8" ?>'
+        data += f"<action><type>setSettings</type><settings><maxChargeCurrent>{int(current)}</maxChargeCurrent></settings></action>"
+        headers = await self._auth.async_get_action_headers(
+            "application/vnd.vwg.mbb.ChargerAction_v1_0_0+xml", None
+        )
+        rsp = await self._auth.post(
+            f"{url}/bs/batterycharge/v1/{self.brand}/{self.country}/vehicles/{vin.upper()}/charger/actions",
+            headers=headers,
+            data=data,
+            use_json=False,
+        )
+        actionid = rsp.getr("action.actionId")
+        await self.async_check_request_succeeded(
+            f"{url}/bs/batterycharge/v1/{self.brand}/{self.country}/vehicles/{vin.upper()}/charger/actions/{actionid}",
+            "set charger max current",
+            SUCCEEDED,
+            FAILED,
+            "action.actionState",
         )
-        _attributes.update(
-            set_attr(
-                "CLIMATISATION_TARGET_TEMP",
-                get_attr(_settings, "targetTemperature.content"),
-            )
-        )
-
-        return _attributes
 
+    async def set_heater_source(
+        self, vin: str, mode: Literal["electric", "auxiliary", "automatic"]
+    ) -> None:
+        """Set max current."""
+        if mode in ["electric", "auxiliary", "automatic"]:
+            self._heater_source[vin] = mode
+
+    async def async_window_heating(self, vin: str, start: bool) -> None:
+        """Set window heating."""
+        # OpenHab "startWindowHeating","stopWindowHeating"
+        url = await self._async_get_home_region(vin.upper())
+        data = '<?xml version="1.0" encoding= "UTF-8" ?>'
+        data += f"<action><type>{'startWindowHeating' if start else 'stopWindowHeating'}</type></action>"
+        headers = await self._auth.async_get_action_headers(
+            "application/vnd.vwg.mbb.ClimaterAction_v1_0_0+xml", None
+        )
+        rsp = await self._auth.post(
+            f"{url}/bs/climatisation/v1/{self.brand}/{self.country}/vehicles/{vin.upper()}/climater/actions",
+            headers=headers,
+            data=data,
+            use_json=False,
+        )
+        actionid = rsp.getr("action.actionId")
+        await self.async_check_request_succeeded(
+            f"{url}/bs/climatisation/v1/{self.brand}/{self.country}/vehicles/{vin.upper()}/climater/actions/{actionid}",
+            "start window heating" if start else "stop window heating",
+            SUCCEEDED,
+            FAILED,
+            "action.actionState",
+        )
+
+    async def set_control_duration(self, vin: str, duration: int) -> None:
+        """Set max current."""
+        self._control_duration[vin] = duration
 
-@dataclass
-class DestinationDataResponse:
-    """Destination."""
-
-    data: dict[str, Any]
-
-    @property
-    def is_supported(self) -> bool:
-        """Supported status."""
-        return self.attributes is not None
-
-    @property
-    def attributes(self) -> dict[Any, dict[str, Any]]:
-        """Attributes properties."""
-        _attributes = {}
-        _attributes = self.data
-        return _attributes
-
-
-@dataclass
-class HistoryDataResponse:
-    """Destination."""
-
-    data: dict[str, Any]
-
-    @property
-    def is_supported(self) -> bool:
-        """Supported status."""
-        return self.attributes is not None
-
-    @property
-    def attributes(self) -> dict[Any, dict[str, Any]]:
-        """Attributes properties."""
-        _attributes = {}
-        _attributes = self.data
-        return _attributes
-
-
-@dataclass
-class UsersDataResponse:
-    """Destination."""
-
-    data: dict[str, Any]
-
-    @property
-    def is_supported(self) -> bool:
-        """Supported status."""
-        return self.attributes is not None
-
-    @property
-    def attributes(self) -> dict[Any, dict[str, Any]]:
-        """Attributes properties."""
-        _attributes = {}
-        _attributes = self.data
-        return _attributes
-
-
-@dataclass
-class PositionDataResponse:
-    """Position class."""
-
-    data: dict[str, Any]
-
-    @property
-    def is_supported(self) -> bool:
-        """Supported status."""
-        return get_attr(self.data, "findCarResponse.Position") is not None
-
-    @property
-    def attributes(self) -> dict[Any, dict[str, Any]]:
-        """Attributes properties."""
-        _attributes = {}
-        car = self.data.get("findCarResponse", {})
-        position = car.get("Position", {})
-        if coordinate := position.get("carCoordinate"):
-            value = {
-                "latitude": coordinate["latitude"] / 1000000,
-                "longitude": coordinate["longitude"] / 1000000,
-                "timestamp": position["timestampCarSentUTC"],
-                "parktime": car.get("parkingTimeUTC", position["timestampCarSentUTC"]),
+    async def async_set_honkflash(
+        self, vin: str, mode: Literal["honk", "flash"], duration: int = 15
+    ) -> None:
+        """Set honk and flash light."""
+        # OpenHab "FLASH_ONLY","HONK_AND_FLASH"
+        url = await self._async_get_home_region(vin.upper())
+        rsp_position = await self._auth.get(
+            f"{url}/bs/cf/v1/{self.brand}/{self.country}/vehicles/{vin.upper()}/position"
+        )
+        position = (
+            rsp_position.get("findCarResponse", {})
+            .get("Position", {})
+            .get("carCoordinate")
+        )
+
+        headers = await self._auth.async_get_action_headers("application/json", None)
+        data = {
+            "honkAndFlashRequest": {
+                "serviceOperationCode": "HONK_AND_FLASH"
+                if mode == "honk"
+                else "FLASH_ONLY",
+                "serviceDuration": duration,
+                "userPosition": {
+                    "latitude": position["latitude"],
+                    "longitude": position["longitude"],
+                },
             }
-            _attributes.update(set_attr("POSITION", value))
-        return _attributes
-
-
-@dataclass
-class TripDataResponse:
-    """Trip class."""
-
-    data: dict[str, Any]
-
-    @property
-    def is_supported(self) -> bool:
-        """Supported status."""
-        return self.data is not None
-
-    @property
-    def attributes(self) -> dict[str, Any]:
-        """Attributes properties."""
-        trip_id = self.data["tripID"]
-        average_electricengine_consumption = (
-            (float(self.data["averageElectricEngineConsumption"]) / 10)
-            if "averageElectricEngineConsumption" in self.data
-            else None
-        )
-        average_fuel_consumption = (
-            float(self.data["averageFuelConsumption"]) / 10
-            if "averageFuelConsumption" in self.data
-            else None
-        )
-        average_speed = (
-            int(self.data["averageSpeed"]) if "averageSpeed" in self.data else None
-        )
-        mileage = int(self.data["mileage"]) if "mileage" in self.data else None
-        start_mileage = (
-            int(self.data["startMileage"]) if "startMileage" in self.data else None
-        )
-        travel_time = (
-            int(self.data["traveltime"]) if "traveltime" in self.data else None
-        )
-        timestamp = self.data["timestamp"] if "timestamp" in self.data else None
-        overall_mileage = (
-            int(self.data["overallMileage"]) if "overallMileage" in self.data else None
-        )
-
-        return {
-            "tripID": trip_id,
-            "averageElectricEngineConsumption": average_electricengine_consumption,
-            "averageFuelConsumption": average_fuel_consumption,
-            "averageSpeed": average_speed,
-            "mileage": mileage,
-            "startMileage": start_mileage,
-            "traveltime": travel_time,
-            "timestamp": timestamp,
-            "overallMileage": overall_mileage,
         }
+        await self._auth.post(
+            f"{url}/bs/rhf/v1/{self.brand}/{self.country}/vehicles/{vin.upper()}/honkAndFlash",
+            headers=headers,
+            data=data,
+        )
 
-
-class Vehicle:
-    """Vehicle class."""
-
-    def __init__(self, data: Any, audi_service: AudiService) -> None:
-        """Initialize."""
-        self._audi_service = audi_service
-        self.vin = data.get("vin")
-        self.csid = data.get("csid")
-        self.model = get_attr(data, "vehicle.media.longName", "")
-        self.model_year = get_attr(data, "vehicle.core.modelYear")
-        if (nickname := data.get("nickname")) is not None and len(nickname) > 0:
-            self.title = nickname
-        else:
-            self.title = get_attr(data, "vehicle.media.shortName", self.vin)
-
-        self.states: dict[Any, dict[str, Any]] = {}
-        self.support_charger: bool | None = None
-        self.support_climater: bool | None = None
-        self.support_position: bool | None = None
-        self.support_preheater: bool | None = None
-        self.support_trip_cyclic: bool | None = None
-        self.support_trip_long: bool | None = None
-        self.support_trip_short: bool | None = None
-        self.support_vehicle: bool | None = None
-
-    async def async_fetch_data(self) -> bool:
-        """Update."""
-        info = ""
+    async def async_check_request_succeeded(
+        self, url: str, action: str, success: str, failed: str, path: str
+    ) -> None:
+        """Check request succeeded."""
+        stauts_good = False
+        for _ in range(MAX_RESPONSE_ATTEMPTS):
+            await asyncio.sleep(REQUEST_STATUS_SLEEP)
+
+            rsp = await self._auth.get(url)
+
+            status = rsp.getr(path)
+
+            if status is None or (failed is not None and status == failed):
+                raise HttpRequestError(("Cannot %s, return code '%s'", action, status))
+
+            if status == success:
+                stauts_good = True
+                break
+
+        if stauts_good is False:
+            raise TimeoutExceededError(("Cannot %s, operation timed out", action))
+
+    def _generate_security_pin_hash(self, challenge: str) -> str:
+        """Generate security pin hash."""
+        pin = to_byte_array(str(self._spin))
+        byte_challenge = to_byte_array(challenge)
+        b_pin = bytes(pin + byte_challenge)
+        return sha512(b_pin).hexdigest().upper()
+
+    async def _async_fill_home_region(self, vin: str) -> None:
+        """Fill region."""
+        self._home_region[vin] = "https://msg.volkswagen.de/fs-car"
+        self._home_region_setter[vin] = "https://mal-1a.prd.ece.vwg-connect.com/api"
         try:
-            info = "status"
-            await self.async_update_vehicle()
-            info = "position"
-            await self.async_update_position()
-            info = "climater"
-            await self.async_update_climater()
-            info = "charger"
-            await self.async_update_charger()
-            info = "preheater"
-            await self.async_update_preheater()
-            for kind in ["short", "long", "cyclic"]:
-                info = kind
-                await self.async_update_tripdata(kind)
-        except Exception as error:  # pylint: disable=broad-except
-            _LOGGER.error(
-                "Unable to update vehicle data %s of %s: %s",
-                info,
-                self.vin,
-                str(error).rstrip("\n"),
+            rsp = await self._auth.get(
+                f"{self._home_region_setter[vin]}/cs/vds/v1/vehicles/{vin}/homeRegion"
             )
-            return False
-        return True
-
-    @retry(exceptions=TimeoutExceededError, tries=3, delay=2)
-    async def async_update_vehicle(self) -> None:
-        """Update vehicle status."""
-        if self.support_vehicle is not False:
-            try:
-                result = await self._audi_service.async_get_vehicle(self.vin)
-                if result.is_supported:
-                    self.states.update(result.attributes)
-            except ServiceNotFoundError as error:
-                if error.args[0] in (401, 403, 502):
-                    self.support_vehicle = False
-                else:
-                    _LOGGER.error(
-                        "Unable to obtain the vehicle  status report of %s: %s",
-                        self.vin,
-                        str(error).rstrip("\n"),
-                    )
-            except HttpRequestError as error:
-                _LOGGER.error(
-                    "Unable to obtain the vehicle  status report of %s: %s",
-                    self.vin,
-                    str(error).rstrip("\n"),
-                )
-            else:
-                self.support_vehicle = result.is_supported
-
-    @retry(exceptions=TimeoutExceededError, tries=3, delay=2)
-    async def async_update_position(self) -> None:
-        """Update vehicle position."""
-        if self.support_position is not False:
-            try:
-                result = await self._audi_service.async_get_stored_position(self.vin)
-                if result.is_supported:
-                    self.states.update(result.attributes)
-            except ServiceNotFoundError as error:
-                if error.args[0] in (401, 403, 502):
-                    self.support_position = False
-                # If error is 204 is returned, the position is currently not available
-                elif error.args[0] != 204:
-                    _LOGGER.error(
-                        "Unable to update the vehicle position of %s: %s",
-                        self.vin,
-                        str(error).rstrip("\n"),
-                    )
-            except HttpRequestError as error:
-                _LOGGER.error(
-                    "Unable to obtain the vehicle position of %s: %s",
-                    self.vin,
-                    str(error).rstrip("\n"),
-                )
-            else:
-                self.support_position = result.is_supported
-
-    @retry(exceptions=TimeoutExceededError, tries=3, delay=2)
-    async def async_update_climater(self) -> None:
-        """Update vehicle climater."""
-        if self.support_climater is not False:
-            try:
-                result = await self._audi_service.async_get_climater(self.vin)
-                if result.is_supported:
-                    self.states.update(result.attributes)
-            except ServiceNotFoundError as error:
-                if error.args[0] in (401, 403, 502):
-                    self.support_climater = False
-                else:
-                    _LOGGER.error(
-                        "Unable to obtain the vehicle climatisation state for %s: %s",
-                        self.vin,
-                        str(error).rstrip("\n"),
-                    )
-            except HttpRequestError as error:
-                _LOGGER.error(
-                    "Unable to obtain the vehicle climatisation state for %s: %s",
-                    self.vin,
-                    str(error).rstrip("\n"),
-                )
-            else:
-                self.support_climater = result.is_supported
-
-    @retry(exceptions=TimeoutExceededError, tries=3, delay=2)
-    async def async_update_preheater(self) -> None:
-        """Update vehicle preheater."""
-        if self.support_preheater is not False:
-            try:
-                result = await self._audi_service.async_get_preheater(self.vin)
-                if result.is_supported:
-                    self.states.update(result.attributes)
-            except ServiceNotFoundError as error:
-                if error.args[0] in (401, 403, 502):
-                    self.support_preheater = False
-                else:
-                    _LOGGER.error(
-                        "Unable to obtain the vehicle preheater state for %s: %s",
-                        self.vin,
-                        str(error).rstrip("\n"),
-                    )
-            except HttpRequestError as error:
-                _LOGGER.error(
-                    "Unable to obtain the vehicle preheater state for %s: %s",
-                    self.vin,
-                    str(error).rstrip("\n"),
-                )
-            else:
-                self.support_preheater = result.is_supported
-
-    @retry(exceptions=TimeoutExceededError, tries=3, delay=2)
-    async def async_update_charger(self) -> None:
-        """Update vehicle charger."""
-        if self.support_charger is not False:
-            try:
-                result = await self._audi_service.async_get_charger(self.vin)
-                if result.is_supported:
-                    self.states.update(result.attributes)
-            except ServiceNotFoundError as error:
-                if error.args[0] in (401, 403, 502):
-                    self.support_charger = False
-                else:
-                    _LOGGER.error(
-                        "Unable to obtain the vehicle charger state for %s: %s",
-                        self.vin,
-                        str(error).rstrip("\n"),
-                    )
-            except HttpRequestError as error:
-                _LOGGER.error(
-                    "Unable to obtain the vehicle charger state for %s: %s",
-                    self.vin,
-                    str(error).rstrip("\n"),
+            uri = rsp.getr("homeRegion.baseUri.content")
+            if uri and uri != self._home_region_setter[vin]:
+                self._home_region[vin] = uri.replace("mal-", "fal-").replace(
+                    "/api", "/fs-car"
                 )
-            else:
-                self.support_charger = result.is_supported
+                self._home_region_setter[vin] = uri
+        except Exception:  # pylint: disable=broad-except
+            pass
+
+    async def _async_get_home_region(self, vin: str) -> str:
+        """Get region."""
+        if self._home_region.get(vin):
+            return self._home_region[vin]
+        await self._async_fill_home_region(vin)
+        return self._home_region[vin]
+
+    async def _async_get_home_region_setter(self, vin: str) -> str:
+        """Get region setter."""
+        if self._home_region_setter.get(vin):
+            return self._home_region_setter[vin]
+        await self._async_fill_home_region(vin)
+        return self._home_region_setter[vin]
+
+    async def _async_get_security_token(self, vin: str, action: str) -> Any:
+        """Get security token."""
+        self._spin = "" if self._spin is None else self._spin
+        url = await self._async_get_home_region_setter(vin.upper())
+
+        # Challenge
+        headers = await self._auth.async_get_headers(token_type="mbb", okhttp=True)
+        rsp = await self._auth.get(
+            f"{url}/rolesrights/authorization/v2/vehicles/{vin.upper()}/services/{action}/security-pin-auth-requested",
+            headers=headers,
+        )
+
+        sec_token = rsp.getr("securityPinAuthInfo.securityToken")
+        challenge: str = rsp.getr(
+            "securityPinAuthInfo.securityPinTransmission.challenge"
+        )
+
+        # Response
+        security_pin_hash = self._generate_security_pin_hash(challenge)
+        data = {
+            "securityPinAuthentication": {
+                "securityPin": {
+                    "challenge": challenge,
+                    "securityPinHash": security_pin_hash,
+                },
+                "securityToken": sec_token,
+            }
+        }
 
-    @retry(exceptions=TimeoutExceededError, tries=3, delay=2)
-    async def async_update_tripdata(
-        self, kind: Literal["short", "long", "cyclic"]
-    ) -> None:
-        """Update vehicle trip."""
-        if getattr(self, f"support_trip_{kind}") is not False:
-            try:
-                td_cur, td_rst = await self._audi_service.async_get_tripdata(
-                    self.vin, kind
-                )
-                if td_cur.is_supported:
-                    self.states.update(
-                        set_attr(f"trip_{kind}_current", td_cur.attributes)
-                    )
-
-                if td_rst.is_supported:
-                    self.states.update(
-                        set_attr(f"trip_{kind}_reset", td_rst.attributes)
-                    )
-            except ServiceNotFoundError as error:
-                if error.args[0] in (400, 401, 403, 502):
-                    setattr(self, f"support_trip_{kind}", False)
-                else:
-                    _LOGGER.error(
-                        "Unable to obtain the vehicle %s tripdata of %s: %s",
-                        kind,
-                        self.vin,
-                        str(error).rstrip("\n"),
-                    )
-            except HttpRequestError as error:
-                _LOGGER.error(
-                    "Unable to obtain the vehicle %s tripdata of %s: %s",
-                    kind,
-                    self.vin,
-                    str(error).rstrip("\n"),
-                )
-            else:
-                setattr(self, f"support_trip_{kind}", True)
+        headers["Content-Type"] = "application/json"
+        body = await self._auth.post(
+            f"{url}/rolesrights/authorization/v2/security-pin-auth-completed",
+            headers=headers,
+            data=data,
+        )
+        return body["securityToken"]
```

### Comparing `audiconnectpy-1.3.2/audiconnectpy.egg-info/PKG-INFO` & `audiconnectpy-1.3.3/audiconnectpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiconnectpy
-Version: 1.3.2
+Version: 1.3.3
 Summary: Provides asynchronous authentication and access to Audi Connect
 Home-page: https://github.com/cyr-ius/audiconnectpy/tree/master/audiconnectpy
 Author: cyr-ius
 Author-email: cyr-ius@ipocus.net
 License: GPL-3
 Keywords: connect,async
 Classifier: Programming Language :: Python
```

### Comparing `audiconnectpy-1.3.2/pyproject.toml` & `audiconnectpy-1.3.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.3.2/setup.py` & `audiconnectpy-1.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # Get the long description from the README file
 with open(os.path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 
 setup(
     name="audiconnectpy",
-    version="1.3.2",
+    version="1.3.3",
     packages=find_packages(),
     author="cyr-ius",
     author_email="cyr-ius@ipocus.net",
     description="Provides asynchronous authentication and access to Audi Connect",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=["aiohttp>=3.8.1", "beautifulsoup4>=4.11.2"],
```

