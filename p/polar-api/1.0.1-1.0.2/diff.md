# Comparing `tmp/polar_api-1.0.1.tar.gz` & `tmp/polar_api-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polar_api-1.0.1.tar", last modified: Mon May  1 08:29:56 2023, max compression
+gzip compressed data, was "polar_api-1.0.2.tar", last modified: Mon May  1 08:39:48 2023, max compression
```

## Comparing `polar_api-1.0.1.tar` & `polar_api-1.0.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 cronsholt   (501) staff       (20)        0 2023-05-01 08:29:56.037336 polar_api-1.0.1/
--rw-r--r--   0 cronsholt   (501) staff       (20)      156 2023-05-01 08:29:56.037215 polar_api-1.0.1/PKG-INFO
--rw-r--r--   0 cronsholt   (501) staff       (20)      896 2023-04-14 08:55:43.000000 polar_api-1.0.1/README.md
-drwxr-xr-x   0 cronsholt   (501) staff       (20)        0 2023-05-01 08:29:56.034212 polar_api-1.0.1/polar_api/
--rw-r--r--   0 cronsholt   (501) staff       (20)     7284 2023-05-01 08:26:23.000000 polar_api-1.0.1/polar_api/PolarAPI.py
--rw-r--r--   0 cronsholt   (501) staff       (20)       94 2023-04-22 06:14:40.000000 polar_api-1.0.1/polar_api/__init__.py
--rw-r--r--   0 cronsholt   (501) staff       (20)    30259 2023-04-14 08:55:43.000000 polar_api-1.0.1/polar_api/cleaning.py
--rw-r--r--   0 cronsholt   (501) staff       (20)     6417 2023-04-14 10:45:49.000000 polar_api-1.0.1/polar_api/polar_api.py
-drwxr-xr-x   0 cronsholt   (501) staff       (20)        0 2023-05-01 08:29:56.035003 polar_api-1.0.1/polar_api.egg-info/
--rw-r--r--   0 cronsholt   (501) staff       (20)      156 2023-05-01 08:29:56.000000 polar_api-1.0.1/polar_api.egg-info/PKG-INFO
--rw-r--r--   0 cronsholt   (501) staff       (20)      533 2023-05-01 08:29:56.000000 polar_api-1.0.1/polar_api.egg-info/SOURCES.txt
--rw-r--r--   0 cronsholt   (501) staff       (20)        1 2023-05-01 08:29:56.000000 polar_api-1.0.1/polar_api.egg-info/dependency_links.txt
--rw-r--r--   0 cronsholt   (501) staff       (20)       69 2023-05-01 08:29:56.000000 polar_api-1.0.1/polar_api.egg-info/requires.txt
--rw-r--r--   0 cronsholt   (501) staff       (20)       28 2023-05-01 08:29:56.000000 polar_api-1.0.1/polar_api.egg-info/top_level.txt
-drwxr-xr-x   0 cronsholt   (501) staff       (20)        0 2023-05-01 08:29:56.036063 polar_api-1.0.1/scripts/
--rw-r--r--   0 cronsholt   (501) staff       (20)        0 2023-04-14 08:55:43.000000 polar_api-1.0.1/scripts/__init__.py
--rw-r--r--   0 cronsholt   (501) staff       (20)     3063 2023-04-14 08:55:43.000000 polar_api-1.0.1/scripts/download_raw_data.py
--rw-r--r--   0 cronsholt   (501) staff       (20)      999 2023-04-14 08:55:43.000000 polar_api-1.0.1/scripts/get_player_session_trimmed.py
--rw-r--r--   0 cronsholt   (501) staff       (20)     3929 2023-04-14 08:55:43.000000 polar_api-1.0.1/scripts/get_session_raw_gps.py
--rw-r--r--   0 cronsholt   (501) staff       (20)     1828 2023-04-14 08:55:43.000000 polar_api-1.0.1/scripts/gps_data_project.py
--rw-r--r--   0 cronsholt   (501) staff       (20)     7680 2023-04-14 08:55:43.000000 polar_api-1.0.1/scripts/session_viz.py
--rw-r--r--   0 cronsholt   (501) staff       (20)       38 2023-05-01 08:29:56.037378 polar_api-1.0.1/setup.cfg
--rw-r--r--   0 cronsholt   (501) staff       (20)      364 2023-05-01 08:29:27.000000 polar_api-1.0.1/setup.py
-drwxr-xr-x   0 cronsholt   (501) staff       (20)        0 2023-05-01 08:29:56.036609 polar_api-1.0.1/utilities/
--rw-r--r--   0 cronsholt   (501) staff       (20)        0 2023-04-14 08:55:43.000000 polar_api-1.0.1/utilities/__init__.py
--rw-r--r--   0 cronsholt   (501) staff       (20)     1595 2023-04-14 08:55:43.000000 polar_api-1.0.1/utilities/metadata.py
--rw-r--r--   0 cronsholt   (501) staff       (20)      548 2023-04-14 08:55:43.000000 polar_api-1.0.1/utilities/polar_IO.py
--rw-r--r--   0 cronsholt   (501) staff       (20)    27284 2023-04-26 06:29:30.000000 polar_api-1.0.1/utilities/polar_api_old.py
+drwxr-xr-x   0 cronsholt   (501) staff       (20)        0 2023-05-01 08:39:48.986368 polar_api-1.0.2/
+-rw-r--r--   0 cronsholt   (501) staff       (20)      156 2023-05-01 08:39:48.986256 polar_api-1.0.2/PKG-INFO
+-rw-r--r--   0 cronsholt   (501) staff       (20)      896 2023-04-14 08:55:43.000000 polar_api-1.0.2/README.md
+drwxr-xr-x   0 cronsholt   (501) staff       (20)        0 2023-05-01 08:39:48.983302 polar_api-1.0.2/polar_api/
+-rw-r--r--   0 cronsholt   (501) staff       (20)     7286 2023-05-01 08:38:20.000000 polar_api-1.0.2/polar_api/PolarAPI.py
+-rw-r--r--   0 cronsholt   (501) staff       (20)       94 2023-04-22 06:14:40.000000 polar_api-1.0.2/polar_api/__init__.py
+-rw-r--r--   0 cronsholt   (501) staff       (20)    30259 2023-04-14 08:55:43.000000 polar_api-1.0.2/polar_api/cleaning.py
+-rw-r--r--   0 cronsholt   (501) staff       (20)     6417 2023-04-14 10:45:49.000000 polar_api-1.0.2/polar_api/polar_api.py
+drwxr-xr-x   0 cronsholt   (501) staff       (20)        0 2023-05-01 08:39:48.984175 polar_api-1.0.2/polar_api.egg-info/
+-rw-r--r--   0 cronsholt   (501) staff       (20)      156 2023-05-01 08:39:48.000000 polar_api-1.0.2/polar_api.egg-info/PKG-INFO
+-rw-r--r--   0 cronsholt   (501) staff       (20)      533 2023-05-01 08:39:48.000000 polar_api-1.0.2/polar_api.egg-info/SOURCES.txt
+-rw-r--r--   0 cronsholt   (501) staff       (20)        1 2023-05-01 08:39:48.000000 polar_api-1.0.2/polar_api.egg-info/dependency_links.txt
+-rw-r--r--   0 cronsholt   (501) staff       (20)       69 2023-05-01 08:39:48.000000 polar_api-1.0.2/polar_api.egg-info/requires.txt
+-rw-r--r--   0 cronsholt   (501) staff       (20)       28 2023-05-01 08:39:48.000000 polar_api-1.0.2/polar_api.egg-info/top_level.txt
+drwxr-xr-x   0 cronsholt   (501) staff       (20)        0 2023-05-01 08:39:48.985255 polar_api-1.0.2/scripts/
+-rw-r--r--   0 cronsholt   (501) staff       (20)        0 2023-04-14 08:55:43.000000 polar_api-1.0.2/scripts/__init__.py
+-rw-r--r--   0 cronsholt   (501) staff       (20)     3063 2023-04-14 08:55:43.000000 polar_api-1.0.2/scripts/download_raw_data.py
+-rw-r--r--   0 cronsholt   (501) staff       (20)      999 2023-04-14 08:55:43.000000 polar_api-1.0.2/scripts/get_player_session_trimmed.py
+-rw-r--r--   0 cronsholt   (501) staff       (20)     3929 2023-04-14 08:55:43.000000 polar_api-1.0.2/scripts/get_session_raw_gps.py
+-rw-r--r--   0 cronsholt   (501) staff       (20)     1828 2023-04-14 08:55:43.000000 polar_api-1.0.2/scripts/gps_data_project.py
+-rw-r--r--   0 cronsholt   (501) staff       (20)     7680 2023-04-14 08:55:43.000000 polar_api-1.0.2/scripts/session_viz.py
+-rw-r--r--   0 cronsholt   (501) staff       (20)       38 2023-05-01 08:39:48.986413 polar_api-1.0.2/setup.cfg
+-rw-r--r--   0 cronsholt   (501) staff       (20)      364 2023-05-01 08:39:33.000000 polar_api-1.0.2/setup.py
+drwxr-xr-x   0 cronsholt   (501) staff       (20)        0 2023-05-01 08:39:48.985771 polar_api-1.0.2/utilities/
+-rw-r--r--   0 cronsholt   (501) staff       (20)        0 2023-04-14 08:55:43.000000 polar_api-1.0.2/utilities/__init__.py
+-rw-r--r--   0 cronsholt   (501) staff       (20)     1595 2023-04-14 08:55:43.000000 polar_api-1.0.2/utilities/metadata.py
+-rw-r--r--   0 cronsholt   (501) staff       (20)      548 2023-04-14 08:55:43.000000 polar_api-1.0.2/utilities/polar_IO.py
+-rw-r--r--   0 cronsholt   (501) staff       (20)    27284 2023-04-26 06:29:30.000000 polar_api-1.0.2/utilities/polar_api_old.py
```

### Comparing `polar_api-1.0.1/README.md` & `polar_api-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `polar_api-1.0.1/polar_api/PolarAPI.py` & `polar_api-1.0.2/polar_api/PolarAPI.py`

 * *Files 0% similar despite different names*

```diff
@@ -112,15 +112,15 @@
             "redirect_uri": self.REDIRECT_URI,
         }
 
         response = requests.post(
             self.AUTH_URL + self.TOKEN_ENDPOINT, headers=headers, data=data
         )
         token_data = response.json()
-        token_data["expires"] = time.time() + token_data["expires_in"]
+        # token_data["expires"] = time.time() + token_data["expires_in"]
 
         return token_data
 
     def set_access_token(self, authorization_code: str) -> None:
         tokens = self._fetch_tokens(authorization_code=authorization_code)
         self.ACCESS_TOKEN = tokens["access_token"]
         self.HEADERS = {
```

### Comparing `polar_api-1.0.1/polar_api/cleaning.py` & `polar_api-1.0.2/polar_api/cleaning.py`

 * *Files identical despite different names*

### Comparing `polar_api-1.0.1/polar_api/polar_api.py` & `polar_api-1.0.2/polar_api/polar_api.py`

 * *Files identical despite different names*

### Comparing `polar_api-1.0.1/polar_api.egg-info/SOURCES.txt` & `polar_api-1.0.2/polar_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `polar_api-1.0.1/scripts/download_raw_data.py` & `polar_api-1.0.2/scripts/download_raw_data.py`

 * *Files identical despite different names*

### Comparing `polar_api-1.0.1/scripts/get_player_session_trimmed.py` & `polar_api-1.0.2/scripts/get_player_session_trimmed.py`

 * *Files identical despite different names*

### Comparing `polar_api-1.0.1/scripts/get_session_raw_gps.py` & `polar_api-1.0.2/scripts/get_session_raw_gps.py`

 * *Files identical despite different names*

### Comparing `polar_api-1.0.1/scripts/gps_data_project.py` & `polar_api-1.0.2/scripts/gps_data_project.py`

 * *Files identical despite different names*

### Comparing `polar_api-1.0.1/scripts/session_viz.py` & `polar_api-1.0.2/scripts/session_viz.py`

 * *Files identical despite different names*

### Comparing `polar_api-1.0.1/utilities/metadata.py` & `polar_api-1.0.2/utilities/metadata.py`

 * *Files identical despite different names*

### Comparing `polar_api-1.0.1/utilities/polar_IO.py` & `polar_api-1.0.2/utilities/polar_IO.py`

 * *Files identical despite different names*

### Comparing `polar_api-1.0.1/utilities/polar_api_old.py` & `polar_api-1.0.2/utilities/polar_api_old.py`

 * *Files identical despite different names*

