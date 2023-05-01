# Comparing `tmp/aiotubes-3.2.tar.gz` & `tmp/aiotubes-3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiotubes-3.2.tar", last modified: Mon Apr 24 06:32:40 2023, max compression
+gzip compressed data, was "aiotubes-3.3.tar", last modified: Mon May  1 10:18:05 2023, max compression
```

## Comparing `aiotubes-3.2.tar` & `aiotubes-3.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 06:32:40.031362 aiotubes-3.2/
--rw-rw-rw-   0        0        0     1084 2022-10-11 08:30:57.000000 aiotubes-3.2/LICENSE
--rw-rw-rw-   0        0        0      697 2023-04-24 06:32:40.030363 aiotubes-3.2/PKG-INFO
--rw-rw-rw-   0        0        0      361 2023-04-23 14:57:43.000000 aiotubes-3.2/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-24 06:32:40.006302 aiotubes-3.2/aiotube/
--rw-rw-rw-   0        0        0       58 2023-04-23 14:53:51.000000 aiotubes-3.2/aiotube/__init__.py
--rw-rw-rw-   0        0        0     1766 2023-04-23 17:42:57.000000 aiotubes-3.2/aiotube/client.py
--rw-rw-rw-   0        0        0      994 2023-04-23 12:02:05.000000 aiotubes-3.2/aiotube/constants.py
--rw-rw-rw-   0        0        0     2511 2023-04-23 14:53:45.000000 aiotubes-3.2/aiotube/exceptions.py
--rw-rw-rw-   0        0        0     5405 2023-04-23 14:53:51.000000 aiotubes-3.2/aiotube/extractors.py
--rw-rw-rw-   0        0        0     2015 2023-04-24 06:32:12.000000 aiotubes-3.2/aiotube/helpers.py
--rw-rw-rw-   0        0        0     4427 2023-02-24 13:57:51.000000 aiotubes-3.2/aiotube/itags.py
--rw-rw-rw-   0        0        0     2226 2023-04-23 14:53:51.000000 aiotubes-3.2/aiotube/playlist.py
--rw-rw-rw-   0        0        0     8051 2023-04-23 17:42:43.000000 aiotubes-3.2/aiotube/streams.py
--rw-rw-rw-   0        0        0     5107 2023-04-24 06:32:12.000000 aiotubes-3.2/aiotube/video.py
-drwxrwxrwx   0        0        0        0 2023-04-24 06:32:40.030363 aiotubes-3.2/aiotubes.egg-info/
--rw-rw-rw-   0        0        0      697 2023-04-24 06:32:39.000000 aiotubes-3.2/aiotubes.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      381 2023-04-24 06:32:39.000000 aiotubes-3.2/aiotubes.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 06:32:39.000000 aiotubes-3.2/aiotubes.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-04-24 06:32:39.000000 aiotubes-3.2/aiotubes.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-24 06:32:39.000000 aiotubes-3.2/aiotubes.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-24 06:32:40.031362 aiotubes-3.2/setup.cfg
--rw-rw-rw-   0        0        0      666 2023-04-24 06:32:22.000000 aiotubes-3.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 10:18:05.671244 aiotubes-3.3/
+-rw-rw-rw-   0        0        0     1084 2022-10-11 08:30:57.000000 aiotubes-3.3/LICENSE
+-rw-rw-rw-   0        0        0      697 2023-05-01 10:18:05.670248 aiotubes-3.3/PKG-INFO
+-rw-rw-rw-   0        0        0      361 2023-04-23 14:57:43.000000 aiotubes-3.3/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-01 10:18:05.632350 aiotubes-3.3/aiotube/
+-rw-rw-rw-   0        0        0       58 2023-04-23 14:53:51.000000 aiotubes-3.3/aiotube/__init__.py
+-rw-rw-rw-   0        0        0     2990 2023-05-01 10:10:21.000000 aiotubes-3.3/aiotube/client.py
+-rw-rw-rw-   0        0        0     1122 2023-05-01 09:27:21.000000 aiotubes-3.3/aiotube/constants.py
+-rw-rw-rw-   0        0        0     2511 2023-04-23 14:53:45.000000 aiotubes-3.3/aiotube/exceptions.py
+-rw-rw-rw-   0        0        0     5405 2023-04-23 14:53:51.000000 aiotubes-3.3/aiotube/extractors.py
+-rw-rw-rw-   0        0        0     2015 2023-04-24 06:32:12.000000 aiotubes-3.3/aiotube/helpers.py
+-rw-rw-rw-   0        0        0     4427 2023-02-24 13:57:51.000000 aiotubes-3.3/aiotube/itags.py
+-rw-rw-rw-   0        0        0     2226 2023-04-23 14:53:51.000000 aiotubes-3.3/aiotube/playlist.py
+-rw-rw-rw-   0        0        0     8051 2023-04-23 17:42:43.000000 aiotubes-3.3/aiotube/streams.py
+-rw-rw-rw-   0        0        0     4946 2023-05-01 10:10:39.000000 aiotubes-3.3/aiotube/video.py
+drwxrwxrwx   0        0        0        0 2023-05-01 10:18:05.669250 aiotubes-3.3/aiotubes.egg-info/
+-rw-rw-rw-   0        0        0      697 2023-05-01 10:18:05.000000 aiotubes-3.3/aiotubes.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      381 2023-05-01 10:18:05.000000 aiotubes-3.3/aiotubes.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 10:18:05.000000 aiotubes-3.3/aiotubes.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-05-01 10:18:05.000000 aiotubes-3.3/aiotubes.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-01 10:18:05.000000 aiotubes-3.3/aiotubes.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-01 10:18:05.671244 aiotubes-3.3/setup.cfg
+-rw-rw-rw-   0        0        0      666 2023-05-01 10:17:32.000000 aiotubes-3.3/setup.py
```

### Comparing `aiotubes-3.2/LICENSE` & `aiotubes-3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aiotubes-3.2/PKG-INFO` & `aiotubes-3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiotubes
-Version: 3.2
+Version: 3.3
 Summary: Asynchronous Youtube API
 Home-page: https://github.com/sheldygg/aiotube
 Author: sheldy
 License: MIT
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
```

### Comparing `aiotubes-3.2/aiotube/client.py` & `aiotubes-3.3/aiotube/client.py`

 * *Files 23% similar despite different names*

```diff
@@ -16,43 +16,81 @@
     HEAD = "HEAD"
 
 
 class RequestClient:
     def __init__(self, client: str):
         self.context = default_clients[client]["context"]
         self.api_key = default_clients[client]["api_key"]
+        self.client_data = default_clients[client]
 
     @property
     def base_params(self) -> dict:
         return {"key": self.api_key, "contentCheckOk": True, "racyCheckOk": True}
 
     @property
     def base_data(self) -> dict:
-        return {"context": self.context}
+        self.context.update(
+            {
+                "androidSdkVersion": 30,
+                "userAgent": self.client_data.get("useragent"),
+                "hl": "en",
+                "timeZone": "UTC",
+                "utcOffsetMinutes": 0
+            }
+        )
+        data = {"context": self.context}
+        data.update(
+            {
+                "params": "8AEB",
+                "playbackContext": {
+                    "contentPlaybackContext":
+                        {"html5Preference": "HTML5_PREF_WANTS"}
+                    },
+                "contentCheckOk": True,
+                "racyCheckOk": True}
+        )
+        return data
+
+    @property
+    def base_headers(self) -> dict:
+        client_version = self.context.get("client").get("clientVersion")
+        headers = {
+            "User-Agent": self.client_data.get("useragent"),
+            "accept-language": "en-US,en",
+            "content-type": "application/json"
+        }
+        headers.update(
+            {
+                "X-YouTube-Client-Name": "3",
+                "X-YouTube-Client-Version": client_version,
+                "Origin": "https://www.youtube.com"
+            }
+        )
+        return headers
 
     async def request(
         self,
         method: HttpMethod,
         url: str,
         headers: dict = None,
         params: dict = None,
         data: dict = None,
     ):
-        base_headers = {"User-Agent": "Mozilla/5.0", "accept-language": "en-US,en"}
+        base_headers = self.base_headers
         if params:
             params = urlencode(params)
         if headers:
             base_headers.update(headers)
         if data:
-            data = json.dumps(data)
+            data = json.dumps(data).encode("utf-8")
         async with ClientSession() as session:
             async with session.request(
                 method=method.value,
                 url=url,
-                headers=base_headers,
+                headers=headers,
                 params=params,
                 data=data,
             ) as response:
                 headers = response.headers
                 try:
                     response_data = await response.json()
                 except ContentTypeError:
```

### Comparing `aiotubes-3.2/aiotube/exceptions.py` & `aiotubes-3.3/aiotube/exceptions.py`

 * *Files identical despite different names*

### Comparing `aiotubes-3.2/aiotube/extractors.py` & `aiotubes-3.3/aiotube/extractors.py`

 * *Files identical despite different names*

### Comparing `aiotubes-3.2/aiotube/helpers.py` & `aiotubes-3.3/aiotube/helpers.py`

 * *Files identical despite different names*

### Comparing `aiotubes-3.2/aiotube/itags.py` & `aiotubes-3.3/aiotube/itags.py`

 * *Files identical despite different names*

### Comparing `aiotubes-3.2/aiotube/playlist.py` & `aiotubes-3.3/aiotube/playlist.py`

 * *Files identical despite different names*

### Comparing `aiotubes-3.2/aiotube/streams.py` & `aiotubes-3.3/aiotube/streams.py`

 * *Files identical despite different names*

### Comparing `aiotubes-3.2/aiotube/video.py` & `aiotubes-3.3/aiotube/video.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,37 +25,36 @@
         if self._html is None:
             self._html = (
                 await self.client.request(method=HttpMethod.GET, url=self.watch_url)
             ).get("response")
         return self._html
 
     async def video_info(self):
-        if self._video_info is None:
-            endpoint = f"{self.base_url}/player"
-            query = {"videoId": self.video_id}
-            query.update(self.client.base_params)
-            headers = {"Content-Type": "application/json"}
-            response = await self.client.request(
-                method=HttpMethod.POST,
-                url=endpoint,
-                params=query,
-                headers=headers,
-                data=self.client.base_data,
-            )
-            self._video_info = response.get("response")
-        return self._video_info
+        endpoint = f"{self.base_url}/player"
+        query = {"videoId": self.video_id}
+        query.update(self.client.base_params)
+        data = self.client.base_data
+        data.update(
+            {"videoId": self.video_id}
+        )
+        response = await self.client.request(
+            method=HttpMethod.POST,
+            url=endpoint,
+            params=query,
+            data=data,
+        )
+        return response.get("response")
 
     @retry_if_none(max_retries=5)
     async def streaming_data(self):
         await self.check_availability()
         data = await self.video_info()
         if "streamingData" in data:
             return data["streamingData"]
-        await self.bypass_age_gate()
-        return self._video_info
+        return await self.bypass_age_gate()
 
     async def fmt_streams(self):
         await self.check_availability()
         if self._fmt_streams:
             return self._fmt_streams
         self._fmt_streams = []
         stream_manifest = apply_descrambler(await self.streaming_data())
@@ -78,15 +77,15 @@
         response = await client.request(
             method=HttpMethod.POST,
             url=endpoint,
             params=query,
             headers=headers,
             data=self.client.base_data,
         )
-        self._video_info = response.get("response")
+        return response.get("response")
 
     async def title(self) -> str:
         """Get the video title."""
         await self.check_availability()
         return (await self.video_info()).get("videoDetails", {}).get("title")
 
     async def author(self) -> str:
```

### Comparing `aiotubes-3.2/aiotubes.egg-info/PKG-INFO` & `aiotubes-3.3/aiotubes.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiotubes
-Version: 3.2
+Version: 3.3
 Summary: Asynchronous Youtube API
 Home-page: https://github.com/sheldygg/aiotube
 Author: sheldy
 License: MIT
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
```

### Comparing `aiotubes-3.2/setup.py` & `aiotubes-3.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def get_description():
     with open('README.rst', 'r', encoding='utf-8') as f:
         return f.read()
 
 
 setuptools.setup(
     name="aiotubes",
-    version="3.2",
+    version="3.3",
     license='MIT',
     author="sheldy",
     description="Asynchronous Youtube API",
     url="https://github.com/sheldygg/aiotube",
     packages=setuptools.find_packages(),
     long_description_content_type='text/markdown',
     long_description=get_description(),
```

