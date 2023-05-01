# Comparing `tmp/wsiserver-1.0.2.tar.gz` & `tmp/wsiserver-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wsiserver-1.0.2.tar", last modified: Thu Apr 27 13:02:42 2023, max compression
+gzip compressed data, was "wsiserver-1.0.3.tar", last modified: Mon May  1 00:44:59 2023, max compression
```

## Comparing `wsiserver-1.0.2.tar` & `wsiserver-1.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 takumi     (501) staff       (20)        0 2023-04-27 13:02:42.877958 wsiserver-1.0.2/
--rw-r--r--   0 takumi     (501) staff       (20)    11357 2023-04-19 13:54:50.000000 wsiserver-1.0.2/LICENSE
--rw-r--r--   0 takumi     (501) staff       (20)    13576 2023-04-27 13:02:42.877407 wsiserver-1.0.2/PKG-INFO
--rw-r--r--   0 takumi     (501) staff       (20)      326 2023-04-22 01:08:13.000000 wsiserver-1.0.2/README.md
--rw-r--r--   0 takumi     (501) staff       (20)      677 2023-04-22 01:03:50.000000 wsiserver-1.0.2/pyproject.toml
--rw-r--r--   0 takumi     (501) staff       (20)       38 2023-04-27 13:02:42.878104 wsiserver-1.0.2/setup.cfg
-drwxr-xr-x   0 takumi     (501) staff       (20)        0 2023-04-27 13:02:42.869905 wsiserver-1.0.2/src/
-drwxr-xr-x   0 takumi     (501) staff       (20)        0 2023-04-27 13:02:42.872683 wsiserver-1.0.2/src/wsiserver/
--rw-r--r--   0 takumi     (501) staff       (20)       22 2023-04-27 13:01:57.000000 wsiserver-1.0.2/src/wsiserver/__init__.py
--rw-r--r--   0 takumi     (501) staff       (20)     2391 2023-04-27 13:00:06.000000 wsiserver-1.0.2/src/wsiserver/app.py
-drwxr-xr-x   0 takumi     (501) staff       (20)        0 2023-04-27 13:02:42.876155 wsiserver-1.0.2/src/wsiserver.egg-info/
--rw-r--r--   0 takumi     (501) staff       (20)    13576 2023-04-27 13:02:42.000000 wsiserver-1.0.2/src/wsiserver.egg-info/PKG-INFO
--rw-r--r--   0 takumi     (501) staff       (20)      303 2023-04-27 13:02:42.000000 wsiserver-1.0.2/src/wsiserver.egg-info/SOURCES.txt
--rw-r--r--   0 takumi     (501) staff       (20)        1 2023-04-27 13:02:42.000000 wsiserver-1.0.2/src/wsiserver.egg-info/dependency_links.txt
--rw-r--r--   0 takumi     (501) staff       (20)       49 2023-04-27 13:02:42.000000 wsiserver-1.0.2/src/wsiserver.egg-info/entry_points.txt
--rw-r--r--   0 takumi     (501) staff       (20)       40 2023-04-27 13:02:42.000000 wsiserver-1.0.2/src/wsiserver.egg-info/requires.txt
--rw-r--r--   0 takumi     (501) staff       (20)       10 2023-04-27 13:02:42.000000 wsiserver-1.0.2/src/wsiserver.egg-info/top_level.txt
+drwxr-xr-x   0 takumi     (501) staff       (20)        0 2023-05-01 00:44:59.181815 wsiserver-1.0.3/
+-rw-r--r--   0 takumi     (501) staff       (20)    11357 2023-04-19 13:54:50.000000 wsiserver-1.0.3/LICENSE
+-rw-r--r--   0 takumi     (501) staff       (20)    13576 2023-05-01 00:44:59.180962 wsiserver-1.0.3/PKG-INFO
+-rw-r--r--   0 takumi     (501) staff       (20)      326 2023-04-22 01:08:13.000000 wsiserver-1.0.3/README.md
+-rw-r--r--   0 takumi     (501) staff       (20)      677 2023-04-22 01:03:50.000000 wsiserver-1.0.3/pyproject.toml
+-rw-r--r--   0 takumi     (501) staff       (20)       38 2023-05-01 00:44:59.181905 wsiserver-1.0.3/setup.cfg
+drwxr-xr-x   0 takumi     (501) staff       (20)        0 2023-05-01 00:44:59.176277 wsiserver-1.0.3/src/
+drwxr-xr-x   0 takumi     (501) staff       (20)        0 2023-05-01 00:44:59.178164 wsiserver-1.0.3/src/wsiserver/
+-rw-r--r--   0 takumi     (501) staff       (20)       22 2023-05-01 00:44:29.000000 wsiserver-1.0.3/src/wsiserver/__init__.py
+-rw-r--r--   0 takumi     (501) staff       (20)     2498 2023-05-01 00:43:06.000000 wsiserver-1.0.3/src/wsiserver/app.py
+drwxr-xr-x   0 takumi     (501) staff       (20)        0 2023-05-01 00:44:59.180490 wsiserver-1.0.3/src/wsiserver.egg-info/
+-rw-r--r--   0 takumi     (501) staff       (20)    13576 2023-05-01 00:44:59.000000 wsiserver-1.0.3/src/wsiserver.egg-info/PKG-INFO
+-rw-r--r--   0 takumi     (501) staff       (20)      303 2023-05-01 00:44:59.000000 wsiserver-1.0.3/src/wsiserver.egg-info/SOURCES.txt
+-rw-r--r--   0 takumi     (501) staff       (20)        1 2023-05-01 00:44:59.000000 wsiserver-1.0.3/src/wsiserver.egg-info/dependency_links.txt
+-rw-r--r--   0 takumi     (501) staff       (20)       49 2023-05-01 00:44:59.000000 wsiserver-1.0.3/src/wsiserver.egg-info/entry_points.txt
+-rw-r--r--   0 takumi     (501) staff       (20)       40 2023-05-01 00:44:59.000000 wsiserver-1.0.3/src/wsiserver.egg-info/requires.txt
+-rw-r--r--   0 takumi     (501) staff       (20)       10 2023-05-01 00:44:59.000000 wsiserver-1.0.3/src/wsiserver.egg-info/top_level.txt
```

### Comparing `wsiserver-1.0.2/LICENSE` & `wsiserver-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `wsiserver-1.0.2/PKG-INFO` & `wsiserver-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wsiserver
-Version: 1.0.2
+Version: 1.0.3
 Summary: Very simple wsi server
 Author-email: Takumi Ando <takumi.ando826@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `wsiserver-1.0.2/pyproject.toml` & `wsiserver-1.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `wsiserver-1.0.2/src/wsiserver/app.py` & `wsiserver-1.0.3/src/wsiserver/app.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 from io import BytesIO
 import math
+import argparse
 
 from fastapi import FastAPI
 from fastapi.responses import Response
 from fastapi.middleware.cors import CORSMiddleware
 import uvicorn
 from PIL import Image
 import openslide
 from openslide.deepzoom import DeepZoomGenerator
 
-import argparse
+import wsiserver
+
+
 parser = argparse.ArgumentParser()
 parser.add_argument("wsi", type=str, help="path to the WSI to load")
 parser.add_argument("--host", type=str, default="0.0.0.0", help="host to listen on")
 parser.add_argument("--port", type=int, default=31791, help="port to listen on")
 parser.add_argument("--tile_size", type=int, default=256, help="tile size")
+parser.add_argument("--version", "-v", action="version" ,versino=wsiserver.__version__)
 args = parser.parse_args()
 
 app = FastAPI()
 app.add_middleware(
     CORSMiddleware,
     allow_origins=["*"],
     allow_credentials=True,
```

### Comparing `wsiserver-1.0.2/src/wsiserver.egg-info/PKG-INFO` & `wsiserver-1.0.3/src/wsiserver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wsiserver
-Version: 1.0.2
+Version: 1.0.3
 Summary: Very simple wsi server
 Author-email: Takumi Ando <takumi.ando826@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

