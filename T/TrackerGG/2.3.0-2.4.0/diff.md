# Comparing `tmp/TrackerGG-2.3.0.tar.gz` & `tmp/TrackerGG-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TrackerGG-2.3.0.tar", last modified: Fri Apr 21 13:35:00 2023, max compression
+gzip compressed data, was "TrackerGG-2.4.0.tar", last modified: Mon May  1 02:09:58 2023, max compression
```

## Comparing `TrackerGG-2.3.0.tar` & `TrackerGG-2.4.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 13:35:00.090427 TrackerGG-2.3.0/
--rw-rw-rw-   0        0        0     1085 2023-03-28 13:34:09.000000 TrackerGG-2.3.0/LICENSE
--rw-rw-rw-   0        0        0     1425 2023-04-21 13:35:00.089427 TrackerGG-2.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     1042 2023-04-05 02:22:42.000000 TrackerGG-2.3.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-21 13:35:00.042599 TrackerGG-2.3.0/TrackerGG/
-drwxrwxrwx   0        0        0        0 2023-04-21 13:35:00.087411 TrackerGG-2.3.0/TrackerGG/Models/
--rw-rw-rw-   0        0        0      652 2023-04-21 13:21:48.000000 TrackerGG-2.3.0/TrackerGG/Models/__init__.py
--rw-rw-rw-   0        0        0     4464 2023-04-21 13:26:31.000000 TrackerGG-2.3.0/TrackerGG/Models/csgo.py
--rw-rw-rw-   0        0        0     1477 2023-03-28 12:55:38.000000 TrackerGG-2.3.0/TrackerGG/Models/platform.py
--rw-rw-rw-   0        0        0     1399 2023-04-03 04:45:05.000000 TrackerGG-2.3.0/TrackerGG/Models/segment.py
--rw-rw-rw-   0        0        0     2059 2023-03-28 23:34:08.000000 TrackerGG-2.3.0/TrackerGG/Models/user.py
--rw-rw-rw-   0        0        0      802 2023-04-04 13:02:49.000000 TrackerGG-2.3.0/TrackerGG/__init__.py
--rw-rw-rw-   0        0        0     3220 2023-04-21 13:26:44.000000 TrackerGG-2.3.0/TrackerGG/client.py
--rw-rw-rw-   0        0        0     3531 2023-04-07 08:57:00.000000 TrackerGG-2.3.0/TrackerGG/httpclient.py
--rw-rw-rw-   0        0        0      833 2023-04-04 13:15:48.000000 TrackerGG-2.3.0/TrackerGG/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-21 13:35:00.073608 TrackerGG-2.3.0/TrackerGG.egg-info/
--rw-rw-rw-   0        0        0     1425 2023-04-21 13:34:59.000000 TrackerGG-2.3.0/TrackerGG.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      411 2023-04-21 13:34:59.000000 TrackerGG-2.3.0/TrackerGG.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 13:34:59.000000 TrackerGG-2.3.0/TrackerGG.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-04-21 13:34:59.000000 TrackerGG-2.3.0/TrackerGG.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-21 13:34:59.000000 TrackerGG-2.3.0/TrackerGG.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-21 13:35:00.091423 TrackerGG-2.3.0/setup.cfg
--rw-rw-rw-   0        0        0      655 2023-04-21 13:34:57.000000 TrackerGG-2.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 02:09:58.745123 TrackerGG-2.4.0/
+-rw-rw-rw-   0        0        0     1085 2023-04-21 13:43:24.000000 TrackerGG-2.4.0/LICENSE
+-rw-rw-rw-   0        0        0     1425 2023-05-01 02:09:58.736846 TrackerGG-2.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1042 2023-04-21 13:43:24.000000 TrackerGG-2.4.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-01 02:09:58.720262 TrackerGG-2.4.0/TrackerGG/
+drwxrwxrwx   0        0        0        0 2023-05-01 02:09:58.734848 TrackerGG-2.4.0/TrackerGG/Models/
+-rw-rw-rw-   0        0        0      753 2023-05-01 01:41:24.000000 TrackerGG-2.4.0/TrackerGG/Models/__init__.py
+-rw-rw-rw-   0        0        0     5759 2023-05-01 02:04:17.000000 TrackerGG-2.4.0/TrackerGG/Models/csgo.py
+-rw-rw-rw-   0        0        0     1477 2023-04-21 13:43:24.000000 TrackerGG-2.4.0/TrackerGG/Models/platform.py
+-rw-rw-rw-   0        0        0     1399 2023-04-21 13:43:24.000000 TrackerGG-2.4.0/TrackerGG/Models/segment.py
+-rw-rw-rw-   0        0        0     2059 2023-04-21 13:43:24.000000 TrackerGG-2.4.0/TrackerGG/Models/user.py
+-rw-rw-rw-   0        0        0      903 2023-05-01 01:41:24.000000 TrackerGG-2.4.0/TrackerGG/__init__.py
+-rw-rw-rw-   0        0        0     3997 2023-05-01 01:05:59.000000 TrackerGG-2.4.0/TrackerGG/client.py
+-rw-rw-rw-   0        0        0     3531 2023-04-21 13:43:24.000000 TrackerGG-2.4.0/TrackerGG/httpclient.py
+-rw-rw-rw-   0        0        0     1143 2023-05-01 02:04:20.000000 TrackerGG-2.4.0/TrackerGG/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-01 02:09:58.726390 TrackerGG-2.4.0/TrackerGG.egg-info/
+-rw-rw-rw-   0        0        0     1425 2023-05-01 02:09:58.000000 TrackerGG-2.4.0/TrackerGG.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      411 2023-05-01 02:09:58.000000 TrackerGG-2.4.0/TrackerGG.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 02:09:58.000000 TrackerGG-2.4.0/TrackerGG.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-05-01 02:09:58.000000 TrackerGG-2.4.0/TrackerGG.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-01 02:09:58.000000 TrackerGG-2.4.0/TrackerGG.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-01 02:09:58.746118 TrackerGG-2.4.0/setup.cfg
+-rw-rw-rw-   0        0        0      655 2023-05-01 02:08:49.000000 TrackerGG-2.4.0/setup.py
```

### Comparing `TrackerGG-2.3.0/LICENSE` & `TrackerGG-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `TrackerGG-2.3.0/PKG-INFO` & `TrackerGG-2.4.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TrackerGG
-Version: 2.3.0
+Version: 2.4.0
 Summary: TrackerGG API Wrapper Library
 Home-page: https://github.com/dev-ruby/TrackerGG
 Author: DevRuby
 Author-email: hiveruby@gmail.com
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.3
```

### Comparing `TrackerGG-2.3.0/README.md` & `TrackerGG-2.4.0/README.md`

 * *Files identical despite different names*

### Comparing `TrackerGG-2.3.0/TrackerGG/Models/__init__.py` & `TrackerGG-2.4.0/TrackerGG/Models/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,8 +14,11 @@
 FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
 OTHER DEALINGS IN THE SOFTWARE.
 
 """
 
 from .csgo import CSGOProfile
 from .csgo import CSGOMapSegment
-from .csgo import CSGOQueryData
+from .csgo import CSGOQueryData
+from .csgo import CSGOWeaponSegment
+from .csgo import CSGOWeapon
+from .platform import Platform
```

### Comparing `TrackerGG-2.3.0/TrackerGG/Models/csgo.py` & `TrackerGG-2.4.0/TrackerGG/Models/csgo.py`

 * *Files 14% similar despite different names*

```diff
@@ -56,23 +56,40 @@
 
 class CSGOMapStats:
     def __init__(self, data: Dict[str, dict]):
         self.rounds: Stat = Stat(data["rounds"])
         self.wins: Stat = Stat(data["wins"])
 
 
+class CSGOWeaponStats:
+    def __init__(self, data: Dict[str, dict]):
+        self.kills: Stat = Stat(data["kills"])
+        self.shots_fired: Stat = Stat(data["shotsFired"])
+        self.shots_hit: Stat = Stat(data["shotsHit"])
+        self.shots_accuracy: Stat = Stat(data["shotsAccuracy"])
+
+
 class CSGOMapSegment:
     def __init__(self, data: Dict[str, Union[str, dict]]):
         self.type: str = data["type"]
         self.attributes: dict = data["attributes"]
         self.metadata: dict = data["metadata"]
         self.expiry_date: str = data["expiryDate"]
         self.stats: CSGOMapStats = CSGOMapStats(data["stats"])
 
 
+class CSGOWeaponSegment:
+    def __init__(self, data: Dict[str, Union[str, dict]]):
+        self.type: str = data["type"]
+        self.attributes: dict = data["attributes"]
+        self.metadata = data["metadata"]
+        self.expiry_date: str = data["expiryDate"]
+        self.stats: CSGOWeaponStats = CSGOWeaponStats(data["stats"])
+
+
 class CSGOSegment:
     def __init__(self, data: Dict[str, Union[str, dict]]):
         self.type: str = data["type"]
         self.attributes: dict = data["attributes"]
         self.metadata: dict = data["metadata"]
         self.expiry_date: str = data["expiryDate"]
         self.stats: CSGOStats = CSGOStats(data["stats"])
@@ -103,7 +120,40 @@
         self.platform_id = int(data["platformId"])
         self.platform_user_id: Union[str, int] = data["platformUserId"]
         self.platform_user_handle: str = data["platformUserHandle"]
         self.platform_user_identifier: Union[str, int] = data["platformUserIdentifier"]
         self.avatar_url: str = data["avatarUrl"]
         self.additional_parameters: Any = data["additionalParameters"]
         self.status: Any = data["status"]
+
+
+class CSGOWeapon(Enum):
+    AK47 = "ak47"
+    AUG = "aug"
+    AWP = "awp"
+    BIZON = "bizon"
+    DEAGLE = "deagle"
+    DUALS = "elite"
+    FAMAS = "famas"
+    FIVESEVEN = "fiveseven"
+    G3SG1 = "g3sg1"
+    GALIL = "galilar"
+    GLOCK = "glock"
+    P2000 = "hkp2000"
+    M249 = "m249"
+    M4A1 = "m4a1"
+    MAC10 = "mac10"
+    MAG7 = "mag7"
+    MP7 = "mp7"
+    MP9 = "mp9"
+    NEGEV = "negev"
+    NOVA = "nova"
+    P250 = "p250"
+    P90 = "p90"
+    SAWED_OFF = "sawedoff"
+    SCAR = "scar20"
+    SG553 = "sg556"
+    SSG08 = "ssg08"
+    ZEUS = "taser"
+    TEC9 = "tec9"
+    UMP45 = "ump45"
+    XM1014 = "xm1014"
```

### Comparing `TrackerGG-2.3.0/TrackerGG/Models/platform.py` & `TrackerGG-2.4.0/TrackerGG/Models/platform.py`

 * *Files identical despite different names*

### Comparing `TrackerGG-2.3.0/TrackerGG/Models/segment.py` & `TrackerGG-2.4.0/TrackerGG/Models/segment.py`

 * *Files identical despite different names*

### Comparing `TrackerGG-2.3.0/TrackerGG/Models/user.py` & `TrackerGG-2.4.0/TrackerGG/Models/user.py`

 * *Files identical despite different names*

### Comparing `TrackerGG-2.3.0/TrackerGG/__init__.py` & `TrackerGG-2.4.0/TrackerGG/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -24,9 +24,12 @@
 FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
 OTHER DEALINGS IN THE SOFTWARE.
 
 """
 
 from .Models import CSGOProfile
 from .Models import CSGOMapSegment
+from .Models import CSGOWeaponSegment
+from .Models import CSGOWeapon
 from .client import CSGOClient
 from . import utils
+from .Models import Platform
```

### Comparing `TrackerGG-2.3.0/TrackerGG/client.py` & `TrackerGG-2.4.0/TrackerGG/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
 import asyncio
 import json
 from typing import List, Union
 
 from .Models import CSGOProfile
 from .Models import CSGOMapSegment
+from .Models import CSGOWeaponSegment
 from .Models import CSGOQueryData
 from .httpclient import HTTPClient
 from .httpclient import RequestMethod
 from .httpclient import ResponseData
 from .httpclient import Route
 
 
@@ -47,15 +48,15 @@
 
     async def get_profile(self, identifier: str) -> CSGOProfile:
         response: ResponseData = await self.http_client.request(
             Route(RequestMethod.GET, f"/csgo/standard/profile/steam/{identifier}")
         )
 
         assert response.status == 200, (
-                "HTTP Response Status Code is not 200\nStatus Code : %d" % response.status
+            "HTTP Response Status Code is not 200\nStatus Code : %d" % response.status
         )
 
         json_data: dict = json.loads(response.response_data)
 
         return CSGOProfile(json_data["data"])
 
     async def get_map_segment(self, identifier: str) -> List[CSGOMapSegment]:
@@ -75,26 +76,51 @@
         segments = []
 
         for segment in json_data["data"]:
             segments.append(CSGOMapSegment(segment))
 
         return segments
 
+    async def get_weapon_segment(self, identifier: str) -> List[CSGOWeaponSegment]:
+        response: ResponseData = await self.http_client.request(
+            Route(
+                RequestMethod.GET,
+                f"/csgo/standard/profile/steam/{identifier}/segments/weapon",
+            )
+        )
+
+        assert response.status == 200, (
+            "HTTP Response Status Code is not 200\nStatus Code : %d" % response.status
+        )
+
+        json_data: dict = json.loads(response.response_data)
+
+        segments = []
+
+        for segment in json_data["data"]:
+            segments.append(CSGOWeaponSegment(segment))
+
+        return segments
+
     async def search_profile(self, query: str) -> Union[None, List[CSGOQueryData]]:
         response: ResponseData = await self.http_client.request(
-            Route(RequestMethod.GET, f"/csgo/standard/search", params={"platform":"steam", "query":query})
+            Route(
+                RequestMethod.GET,
+                f"/csgo/standard/search",
+                params={"platform": "steam", "query": query},
+            )
         )
 
         assert response.status == 200, (
-                "HTTP Response Status Code is not 200\nStatus Code : %d" % response.status
+            "HTTP Response Status Code is not 200\nStatus Code : %d" % response.status
         )
 
         json_data: dict = json.loads(response.response_data)
 
         query_data = None
 
         if json_data["data"]:
             query_data = []
             for dat in json_data["data"]:
                 query_data.append(CSGOQueryData(dat))
 
-        return query_data
+        return query_data
```

### Comparing `TrackerGG-2.3.0/TrackerGG/httpclient.py` & `TrackerGG-2.4.0/TrackerGG/httpclient.py`

 * *Files identical despite different names*

### Comparing `TrackerGG-2.3.0/TrackerGG.egg-info/PKG-INFO` & `TrackerGG-2.4.0/TrackerGG.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TrackerGG
-Version: 2.3.0
+Version: 2.4.0
 Summary: TrackerGG API Wrapper Library
 Home-page: https://github.com/dev-ruby/TrackerGG
 Author: DevRuby
 Author-email: hiveruby@gmail.com
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.3
```

### Comparing `TrackerGG-2.3.0/setup.py` & `TrackerGG-2.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fs:
     long_description = fs.read()
 
 setuptools.setup(
     name="TrackerGG",
-    version="2.3.0",
+    version="2.4.0",
     author="DevRuby",
     author_email="hiveruby@gmail.com",
     description="TrackerGG API Wrapper Library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/dev-ruby/TrackerGG",
     packages=setuptools.find_packages(),
```

