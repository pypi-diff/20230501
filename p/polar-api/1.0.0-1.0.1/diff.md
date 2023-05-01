# Comparing `tmp/polar_api-1.0.0.tar.gz` & `tmp/polar_api-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polar_api-1.0.0.tar", last modified: Mon May  1 08:09:22 2023, max compression
+gzip compressed data, was "polar_api-1.0.1.tar", last modified: Mon May  1 08:29:56 2023, max compression
```

## Comparing `polar_api-1.0.0.tar` & `polar_api-1.0.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 cronsholt   (501) staff       (20)        0 2023-05-01 08:09:22.544161 polar_api-1.0.0/
--rw-r--r--   0 cronsholt   (501) staff       (20)      156 2023-05-01 08:09:22.544014 polar_api-1.0.0/PKG-INFO
--rw-r--r--   0 cronsholt   (501) staff       (20)      896 2023-04-14 08:55:43.000000 polar_api-1.0.0/README.md
-drwxr-xr-x   0 cronsholt   (501) staff       (20)        0 2023-05-01 08:09:22.540397 polar_api-1.0.0/polar_api/
--rw-r--r--   0 cronsholt   (501) staff       (20)     7314 2023-05-01 07:55:40.000000 polar_api-1.0.0/polar_api/PolarAPI.py
--rw-r--r--   0 cronsholt   (501) staff       (20)       94 2023-04-22 06:14:40.000000 polar_api-1.0.0/polar_api/__init__.py
--rw-r--r--   0 cronsholt   (501) staff       (20)    30259 2023-04-14 08:55:43.000000 polar_api-1.0.0/polar_api/cleaning.py
--rw-r--r--   0 cronsholt   (501) staff       (20)     6417 2023-04-14 10:45:49.000000 polar_api-1.0.0/polar_api/polar_api.py
-drwxr-xr-x   0 cronsholt   (501) staff       (20)        0 2023-05-01 08:09:22.541529 polar_api-1.0.0/polar_api.egg-info/
--rw-r--r--   0 cronsholt   (501) staff       (20)      156 2023-05-01 08:09:22.000000 polar_api-1.0.0/polar_api.egg-info/PKG-INFO
--rw-r--r--   0 cronsholt   (501) staff       (20)      533 2023-05-01 08:09:22.000000 polar_api-1.0.0/polar_api.egg-info/SOURCES.txt
--rw-r--r--   0 cronsholt   (501) staff       (20)        1 2023-05-01 08:09:22.000000 polar_api-1.0.0/polar_api.egg-info/dependency_links.txt
--rw-r--r--   0 cronsholt   (501) staff       (20)       46 2023-05-01 08:09:22.000000 polar_api-1.0.0/polar_api.egg-info/requires.txt
--rw-r--r--   0 cronsholt   (501) staff       (20)       28 2023-05-01 08:09:22.000000 polar_api-1.0.0/polar_api.egg-info/top_level.txt
-drwxr-xr-x   0 cronsholt   (501) staff       (20)        0 2023-05-01 08:09:22.542886 polar_api-1.0.0/scripts/
--rw-r--r--   0 cronsholt   (501) staff       (20)        0 2023-04-14 08:55:43.000000 polar_api-1.0.0/scripts/__init__.py
--rw-r--r--   0 cronsholt   (501) staff       (20)     3063 2023-04-14 08:55:43.000000 polar_api-1.0.0/scripts/download_raw_data.py
--rw-r--r--   0 cronsholt   (501) staff       (20)      999 2023-04-14 08:55:43.000000 polar_api-1.0.0/scripts/get_player_session_trimmed.py
--rw-r--r--   0 cronsholt   (501) staff       (20)     3929 2023-04-14 08:55:43.000000 polar_api-1.0.0/scripts/get_session_raw_gps.py
--rw-r--r--   0 cronsholt   (501) staff       (20)     1828 2023-04-14 08:55:43.000000 polar_api-1.0.0/scripts/gps_data_project.py
--rw-r--r--   0 cronsholt   (501) staff       (20)     7680 2023-04-14 08:55:43.000000 polar_api-1.0.0/scripts/session_viz.py
--rw-r--r--   0 cronsholt   (501) staff       (20)       38 2023-05-01 08:09:22.544213 polar_api-1.0.0/setup.cfg
--rw-r--r--   0 cronsholt   (501) staff       (20)      330 2023-05-01 08:08:19.000000 polar_api-1.0.0/setup.py
-drwxr-xr-x   0 cronsholt   (501) staff       (20)        0 2023-05-01 08:09:22.543492 polar_api-1.0.0/utilities/
--rw-r--r--   0 cronsholt   (501) staff       (20)        0 2023-04-14 08:55:43.000000 polar_api-1.0.0/utilities/__init__.py
--rw-r--r--   0 cronsholt   (501) staff       (20)     1595 2023-04-14 08:55:43.000000 polar_api-1.0.0/utilities/metadata.py
--rw-r--r--   0 cronsholt   (501) staff       (20)      548 2023-04-14 08:55:43.000000 polar_api-1.0.0/utilities/polar_IO.py
--rw-r--r--   0 cronsholt   (501) staff       (20)    27284 2023-04-26 06:29:30.000000 polar_api-1.0.0/utilities/polar_api_old.py
+drwxr-xr-x   0 cronsholt   (501) staff       (20)        0 2023-05-01 08:29:56.037336 polar_api-1.0.1/
+-rw-r--r--   0 cronsholt   (501) staff       (20)      156 2023-05-01 08:29:56.037215 polar_api-1.0.1/PKG-INFO
+-rw-r--r--   0 cronsholt   (501) staff       (20)      896 2023-04-14 08:55:43.000000 polar_api-1.0.1/README.md
+drwxr-xr-x   0 cronsholt   (501) staff       (20)        0 2023-05-01 08:29:56.034212 polar_api-1.0.1/polar_api/
+-rw-r--r--   0 cronsholt   (501) staff       (20)     7284 2023-05-01 08:26:23.000000 polar_api-1.0.1/polar_api/PolarAPI.py
+-rw-r--r--   0 cronsholt   (501) staff       (20)       94 2023-04-22 06:14:40.000000 polar_api-1.0.1/polar_api/__init__.py
+-rw-r--r--   0 cronsholt   (501) staff       (20)    30259 2023-04-14 08:55:43.000000 polar_api-1.0.1/polar_api/cleaning.py
+-rw-r--r--   0 cronsholt   (501) staff       (20)     6417 2023-04-14 10:45:49.000000 polar_api-1.0.1/polar_api/polar_api.py
+drwxr-xr-x   0 cronsholt   (501) staff       (20)        0 2023-05-01 08:29:56.035003 polar_api-1.0.1/polar_api.egg-info/
+-rw-r--r--   0 cronsholt   (501) staff       (20)      156 2023-05-01 08:29:56.000000 polar_api-1.0.1/polar_api.egg-info/PKG-INFO
+-rw-r--r--   0 cronsholt   (501) staff       (20)      533 2023-05-01 08:29:56.000000 polar_api-1.0.1/polar_api.egg-info/SOURCES.txt
+-rw-r--r--   0 cronsholt   (501) staff       (20)        1 2023-05-01 08:29:56.000000 polar_api-1.0.1/polar_api.egg-info/dependency_links.txt
+-rw-r--r--   0 cronsholt   (501) staff       (20)       69 2023-05-01 08:29:56.000000 polar_api-1.0.1/polar_api.egg-info/requires.txt
+-rw-r--r--   0 cronsholt   (501) staff       (20)       28 2023-05-01 08:29:56.000000 polar_api-1.0.1/polar_api.egg-info/top_level.txt
+drwxr-xr-x   0 cronsholt   (501) staff       (20)        0 2023-05-01 08:29:56.036063 polar_api-1.0.1/scripts/
+-rw-r--r--   0 cronsholt   (501) staff       (20)        0 2023-04-14 08:55:43.000000 polar_api-1.0.1/scripts/__init__.py
+-rw-r--r--   0 cronsholt   (501) staff       (20)     3063 2023-04-14 08:55:43.000000 polar_api-1.0.1/scripts/download_raw_data.py
+-rw-r--r--   0 cronsholt   (501) staff       (20)      999 2023-04-14 08:55:43.000000 polar_api-1.0.1/scripts/get_player_session_trimmed.py
+-rw-r--r--   0 cronsholt   (501) staff       (20)     3929 2023-04-14 08:55:43.000000 polar_api-1.0.1/scripts/get_session_raw_gps.py
+-rw-r--r--   0 cronsholt   (501) staff       (20)     1828 2023-04-14 08:55:43.000000 polar_api-1.0.1/scripts/gps_data_project.py
+-rw-r--r--   0 cronsholt   (501) staff       (20)     7680 2023-04-14 08:55:43.000000 polar_api-1.0.1/scripts/session_viz.py
+-rw-r--r--   0 cronsholt   (501) staff       (20)       38 2023-05-01 08:29:56.037378 polar_api-1.0.1/setup.cfg
+-rw-r--r--   0 cronsholt   (501) staff       (20)      364 2023-05-01 08:29:27.000000 polar_api-1.0.1/setup.py
+drwxr-xr-x   0 cronsholt   (501) staff       (20)        0 2023-05-01 08:29:56.036609 polar_api-1.0.1/utilities/
+-rw-r--r--   0 cronsholt   (501) staff       (20)        0 2023-04-14 08:55:43.000000 polar_api-1.0.1/utilities/__init__.py
+-rw-r--r--   0 cronsholt   (501) staff       (20)     1595 2023-04-14 08:55:43.000000 polar_api-1.0.1/utilities/metadata.py
+-rw-r--r--   0 cronsholt   (501) staff       (20)      548 2023-04-14 08:55:43.000000 polar_api-1.0.1/utilities/polar_IO.py
+-rw-r--r--   0 cronsholt   (501) staff       (20)    27284 2023-04-26 06:29:30.000000 polar_api-1.0.1/utilities/polar_api_old.py
```

### Comparing `polar_api-1.0.0/README.md` & `polar_api-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `polar_api-1.0.0/polar_api/PolarAPI.py` & `polar_api-1.0.1/polar_api/PolarAPI.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import os
 import time
 import webbrowser
 from typing import Union
 from urllib.parse import parse_qs, urlencode, urlparse
 
 import requests
-from bs4 import BeautifulSoup
 
 
 class PolarTeamproAPI:
     BASE_URL = "https://teampro.api.polar.com"
     AUTH_URL = "https://auth.polar.com/"
     AUTH_ENDPOINT = "oauth/authorize?"
     TOKEN_ENDPOINT = "oauth/token?"
```

### Comparing `polar_api-1.0.0/polar_api/cleaning.py` & `polar_api-1.0.1/polar_api/cleaning.py`

 * *Files identical despite different names*

### Comparing `polar_api-1.0.0/polar_api/polar_api.py` & `polar_api-1.0.1/polar_api/polar_api.py`

 * *Files identical despite different names*

### Comparing `polar_api-1.0.0/polar_api.egg-info/SOURCES.txt` & `polar_api-1.0.1/polar_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `polar_api-1.0.0/scripts/download_raw_data.py` & `polar_api-1.0.1/scripts/download_raw_data.py`

 * *Files identical despite different names*

### Comparing `polar_api-1.0.0/scripts/get_player_session_trimmed.py` & `polar_api-1.0.1/scripts/get_player_session_trimmed.py`

 * *Files identical despite different names*

### Comparing `polar_api-1.0.0/scripts/get_session_raw_gps.py` & `polar_api-1.0.1/scripts/get_session_raw_gps.py`

 * *Files identical despite different names*

### Comparing `polar_api-1.0.0/scripts/gps_data_project.py` & `polar_api-1.0.1/scripts/gps_data_project.py`

 * *Files identical despite different names*

### Comparing `polar_api-1.0.0/scripts/session_viz.py` & `polar_api-1.0.1/scripts/session_viz.py`

 * *Files identical despite different names*

### Comparing `polar_api-1.0.0/utilities/metadata.py` & `polar_api-1.0.1/utilities/metadata.py`

 * *Files identical despite different names*

### Comparing `polar_api-1.0.0/utilities/polar_IO.py` & `polar_api-1.0.1/utilities/polar_IO.py`

 * *Files identical despite different names*

### Comparing `polar_api-1.0.0/utilities/polar_api_old.py` & `polar_api-1.0.1/utilities/polar_api_old.py`

 * *Files identical despite different names*

