# Comparing `tmp/aiotubes-3.3.tar.gz` & `tmp/aiotubes-3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiotubes-3.3.tar", last modified: Mon May  1 10:18:05 2023, max compression
+gzip compressed data, was "aiotubes-3.4.tar", last modified: Mon May  1 10:29:33 2023, max compression
```

## Comparing `aiotubes-3.3.tar` & `aiotubes-3.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 10:18:05.671244 aiotubes-3.3/
--rw-rw-rw-   0        0        0     1084 2022-10-11 08:30:57.000000 aiotubes-3.3/LICENSE
--rw-rw-rw-   0        0        0      697 2023-05-01 10:18:05.670248 aiotubes-3.3/PKG-INFO
--rw-rw-rw-   0        0        0      361 2023-04-23 14:57:43.000000 aiotubes-3.3/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-01 10:18:05.632350 aiotubes-3.3/aiotube/
--rw-rw-rw-   0        0        0       58 2023-04-23 14:53:51.000000 aiotubes-3.3/aiotube/__init__.py
--rw-rw-rw-   0        0        0     2990 2023-05-01 10:10:21.000000 aiotubes-3.3/aiotube/client.py
--rw-rw-rw-   0        0        0     1122 2023-05-01 09:27:21.000000 aiotubes-3.3/aiotube/constants.py
--rw-rw-rw-   0        0        0     2511 2023-04-23 14:53:45.000000 aiotubes-3.3/aiotube/exceptions.py
--rw-rw-rw-   0        0        0     5405 2023-04-23 14:53:51.000000 aiotubes-3.3/aiotube/extractors.py
--rw-rw-rw-   0        0        0     2015 2023-04-24 06:32:12.000000 aiotubes-3.3/aiotube/helpers.py
--rw-rw-rw-   0        0        0     4427 2023-02-24 13:57:51.000000 aiotubes-3.3/aiotube/itags.py
--rw-rw-rw-   0        0        0     2226 2023-04-23 14:53:51.000000 aiotubes-3.3/aiotube/playlist.py
--rw-rw-rw-   0        0        0     8051 2023-04-23 17:42:43.000000 aiotubes-3.3/aiotube/streams.py
--rw-rw-rw-   0        0        0     4946 2023-05-01 10:10:39.000000 aiotubes-3.3/aiotube/video.py
-drwxrwxrwx   0        0        0        0 2023-05-01 10:18:05.669250 aiotubes-3.3/aiotubes.egg-info/
--rw-rw-rw-   0        0        0      697 2023-05-01 10:18:05.000000 aiotubes-3.3/aiotubes.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      381 2023-05-01 10:18:05.000000 aiotubes-3.3/aiotubes.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 10:18:05.000000 aiotubes-3.3/aiotubes.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-05-01 10:18:05.000000 aiotubes-3.3/aiotubes.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-01 10:18:05.000000 aiotubes-3.3/aiotubes.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-01 10:18:05.671244 aiotubes-3.3/setup.cfg
--rw-rw-rw-   0        0        0      666 2023-05-01 10:17:32.000000 aiotubes-3.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 10:29:33.292484 aiotubes-3.4/
+-rw-rw-rw-   0        0        0     1084 2022-10-11 08:30:57.000000 aiotubes-3.4/LICENSE
+-rw-rw-rw-   0        0        0      697 2023-05-01 10:29:33.292484 aiotubes-3.4/PKG-INFO
+-rw-rw-rw-   0        0        0      361 2023-04-23 14:57:43.000000 aiotubes-3.4/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-01 10:29:33.275530 aiotubes-3.4/aiotube/
+-rw-rw-rw-   0        0        0       58 2023-04-23 14:53:51.000000 aiotubes-3.4/aiotube/__init__.py
+-rw-rw-rw-   0        0        0     2990 2023-05-01 10:10:21.000000 aiotubes-3.4/aiotube/client.py
+-rw-rw-rw-   0        0        0     1122 2023-05-01 09:27:21.000000 aiotubes-3.4/aiotube/constants.py
+-rw-rw-rw-   0        0        0     2511 2023-04-23 14:53:45.000000 aiotubes-3.4/aiotube/exceptions.py
+-rw-rw-rw-   0        0        0     5405 2023-04-23 14:53:51.000000 aiotubes-3.4/aiotube/extractors.py
+-rw-rw-rw-   0        0        0     2015 2023-04-24 06:32:12.000000 aiotubes-3.4/aiotube/helpers.py
+-rw-rw-rw-   0        0        0     4427 2023-02-24 13:57:51.000000 aiotubes-3.4/aiotube/itags.py
+-rw-rw-rw-   0        0        0     2226 2023-04-23 14:53:51.000000 aiotubes-3.4/aiotube/playlist.py
+-rw-rw-rw-   0        0        0     8126 2023-05-01 10:28:02.000000 aiotubes-3.4/aiotube/streams.py
+-rw-rw-rw-   0        0        0     4946 2023-05-01 10:10:39.000000 aiotubes-3.4/aiotube/video.py
+drwxrwxrwx   0        0        0        0 2023-05-01 10:29:33.291489 aiotubes-3.4/aiotubes.egg-info/
+-rw-rw-rw-   0        0        0      697 2023-05-01 10:29:33.000000 aiotubes-3.4/aiotubes.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      381 2023-05-01 10:29:33.000000 aiotubes-3.4/aiotubes.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 10:29:33.000000 aiotubes-3.4/aiotubes.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-05-01 10:29:33.000000 aiotubes-3.4/aiotubes.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-01 10:29:33.000000 aiotubes-3.4/aiotubes.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-01 10:29:33.293481 aiotubes-3.4/setup.cfg
+-rw-rw-rw-   0        0        0      666 2023-05-01 10:29:25.000000 aiotubes-3.4/setup.py
```

### Comparing `aiotubes-3.3/LICENSE` & `aiotubes-3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `aiotubes-3.3/PKG-INFO` & `aiotubes-3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiotubes
-Version: 3.3
+Version: 3.4
 Summary: Asynchronous Youtube API
 Home-page: https://github.com/sheldygg/aiotube
 Author: sheldy
 License: MIT
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
```

### Comparing `aiotubes-3.3/aiotube/client.py` & `aiotubes-3.4/aiotube/client.py`

 * *Files identical despite different names*

### Comparing `aiotubes-3.3/aiotube/constants.py` & `aiotubes-3.4/aiotube/constants.py`

 * *Files identical despite different names*

### Comparing `aiotubes-3.3/aiotube/exceptions.py` & `aiotubes-3.4/aiotube/exceptions.py`

 * *Files identical despite different names*

### Comparing `aiotubes-3.3/aiotube/extractors.py` & `aiotubes-3.4/aiotube/extractors.py`

 * *Files identical despite different names*

### Comparing `aiotubes-3.3/aiotube/helpers.py` & `aiotubes-3.4/aiotube/helpers.py`

 * *Files identical despite different names*

### Comparing `aiotubes-3.3/aiotube/itags.py` & `aiotubes-3.4/aiotube/itags.py`

 * *Files identical despite different names*

### Comparing `aiotubes-3.3/aiotube/playlist.py` & `aiotubes-3.4/aiotube/playlist.py`

 * *Files identical despite different names*

### Comparing `aiotubes-3.3/aiotube/streams.py` & `aiotubes-3.4/aiotube/streams.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 from .client import RequestClient, HttpMethod
 from .extractors import mime_type_codec
 from .helpers import safe_filename, target_directory
 from .itags import get_format_profile
 
 
-class Stream(BaseModel, RequestClient):
+class Stream(BaseModel):
     title: str
     author: str
     url: HttpUrl
     itag: int
     mimeType: str
     bitrate: int
     width: Optional[int]
@@ -92,25 +92,27 @@
         """Whether the stream only contains video.
 
         :rtype: bool
         """
         return self.is_progressive or self.type == "video"
 
     async def filesize(self) -> int:
-        response = await self.request(method=HttpMethod.HEAD, url=self.url)
+        client = RequestClient("ANDROID")
+        response = await client.request(method=HttpMethod.HEAD, url=self.url)
         return int(response.get("headers", {}).get("Content-Length"))
 
     async def _download(self) -> AsyncGenerator[bytes, None]:
+        client = RequestClient("ANDROID")
         default_range_size = 9437184
         file_size: int = default_range_size
         downloaded = 0
         while downloaded < file_size:
             stop_pos = min(downloaded + default_range_size, file_size) - 1
             range_header = f"bytes={downloaded}-{stop_pos}"
-            request = await self.request(
+            request = await client.request(
                 method=HttpMethod.GET, url=self.url, headers={"Range": range_header}
             )
             headers = request.get("headers")
             chunk = request.get("response")
             if file_size == default_range_size:
                 content_range = headers.get("Content-Range")
                 file_size = int(content_range.split("/")[1])
```

### Comparing `aiotubes-3.3/aiotube/video.py` & `aiotubes-3.4/aiotube/video.py`

 * *Files identical despite different names*

### Comparing `aiotubes-3.3/aiotubes.egg-info/PKG-INFO` & `aiotubes-3.4/aiotubes.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiotubes
-Version: 3.3
+Version: 3.4
 Summary: Asynchronous Youtube API
 Home-page: https://github.com/sheldygg/aiotube
 Author: sheldy
 License: MIT
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
```

### Comparing `aiotubes-3.3/setup.py` & `aiotubes-3.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def get_description():
     with open('README.rst', 'r', encoding='utf-8') as f:
         return f.read()
 
 
 setuptools.setup(
     name="aiotubes",
-    version="3.3",
+    version="3.4",
     license='MIT',
     author="sheldy",
     description="Asynchronous Youtube API",
     url="https://github.com/sheldygg/aiotube",
     packages=setuptools.find_packages(),
     long_description_content_type='text/markdown',
     long_description=get_description(),
```

