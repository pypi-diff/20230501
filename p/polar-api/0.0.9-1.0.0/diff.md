# Comparing `tmp/polar_api-0.0.9.tar.gz` & `tmp/polar_api-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/polar_api-0.0.9.tar", last modified: Wed Mar  8 10:57:54 2023, max compression
+gzip compressed data, was "polar_api-1.0.0.tar", last modified: Mon May  1 08:09:22 2023, max compression
```

## Comparing `polar_api-0.0.9.tar` & `polar_api-1.0.0.tar`

### file list

```diff
@@ -1,26 +1,28 @@
-drwxr-xr-x   0 franekl    (501) staff       (20)        0 2023-03-08 10:57:54.772863 polar_api-0.0.9/
--rw-r--r--   0 franekl    (501) staff       (20)      205 2023-03-08 10:57:54.772682 polar_api-0.0.9/PKG-INFO
--rw-r--r--   0 franekl    (501) staff       (20)      896 2023-03-08 10:55:43.000000 polar_api-0.0.9/README.md
-drwxr-xr-x   0 franekl    (501) staff       (20)        0 2023-03-08 10:57:54.770423 polar_api-0.0.9/polar_api/
--rw-r--r--   0 franekl    (501) staff       (20)       57 2022-10-26 12:34:03.000000 polar_api-0.0.9/polar_api/__init__.py
--rw-r--r--   0 franekl    (501) staff       (20)    30259 2023-03-08 10:56:08.000000 polar_api-0.0.9/polar_api/cleaning.py
--rw-r--r--   0 franekl    (501) staff       (20)     6453 2023-03-08 10:55:43.000000 polar_api-0.0.9/polar_api/polar_api.py
-drwxr-xr-x   0 franekl    (501) staff       (20)        0 2023-03-08 10:57:54.770977 polar_api-0.0.9/polar_api.egg-info/
--rw-r--r--   0 franekl    (501) staff       (20)      205 2023-03-08 10:57:54.000000 polar_api-0.0.9/polar_api.egg-info/PKG-INFO
--rw-r--r--   0 franekl    (501) staff       (20)      479 2023-03-08 10:57:54.000000 polar_api-0.0.9/polar_api.egg-info/SOURCES.txt
--rw-r--r--   0 franekl    (501) staff       (20)        1 2023-03-08 10:57:54.000000 polar_api-0.0.9/polar_api.egg-info/dependency_links.txt
--rw-r--r--   0 franekl    (501) staff       (20)       28 2023-03-08 10:57:54.000000 polar_api-0.0.9/polar_api.egg-info/top_level.txt
-drwxr-xr-x   0 franekl    (501) staff       (20)        0 2023-03-08 10:57:54.771841 polar_api-0.0.9/scripts/
--rw-r--r--   0 franekl    (501) staff       (20)        0 2022-10-19 07:37:58.000000 polar_api-0.0.9/scripts/__init__.py
--rw-r--r--   0 franekl    (501) staff       (20)     3063 2022-10-30 08:35:09.000000 polar_api-0.0.9/scripts/download_raw_data.py
--rw-r--r--   0 franekl    (501) staff       (20)      999 2022-10-19 07:37:58.000000 polar_api-0.0.9/scripts/get_player_session_trimmed.py
--rw-r--r--   0 franekl    (501) staff       (20)     3929 2022-10-19 07:37:58.000000 polar_api-0.0.9/scripts/get_session_raw_gps.py
--rw-r--r--   0 franekl    (501) staff       (20)     1828 2022-10-19 07:37:58.000000 polar_api-0.0.9/scripts/gps_data_project.py
--rw-r--r--   0 franekl    (501) staff       (20)     7680 2022-10-19 07:37:58.000000 polar_api-0.0.9/scripts/session_viz.py
--rw-r--r--   0 franekl    (501) staff       (20)       38 2023-03-08 10:57:54.772927 polar_api-0.0.9/setup.cfg
--rw-r--r--   0 franekl    (501) staff       (20)      221 2023-03-08 10:57:17.000000 polar_api-0.0.9/setup.py
-drwxr-xr-x   0 franekl    (501) staff       (20)        0 2023-03-08 10:57:54.772425 polar_api-0.0.9/utilities/
--rw-r--r--   0 franekl    (501) staff       (20)        0 2022-10-30 08:34:25.000000 polar_api-0.0.9/utilities/__init__.py
--rw-r--r--   0 franekl    (501) staff       (20)     1595 2022-10-30 08:34:25.000000 polar_api-0.0.9/utilities/metadata.py
--rw-r--r--   0 franekl    (501) staff       (20)      548 2022-10-19 07:37:58.000000 polar_api-0.0.9/utilities/polar_IO.py
--rw-r--r--   0 franekl    (501) staff       (20)    27356 2022-10-30 08:35:09.000000 polar_api-0.0.9/utilities/polar_api_old.py
+drwxr-xr-x   0 cronsholt   (501) staff       (20)        0 2023-05-01 08:09:22.544161 polar_api-1.0.0/
+-rw-r--r--   0 cronsholt   (501) staff       (20)      156 2023-05-01 08:09:22.544014 polar_api-1.0.0/PKG-INFO
+-rw-r--r--   0 cronsholt   (501) staff       (20)      896 2023-04-14 08:55:43.000000 polar_api-1.0.0/README.md
+drwxr-xr-x   0 cronsholt   (501) staff       (20)        0 2023-05-01 08:09:22.540397 polar_api-1.0.0/polar_api/
+-rw-r--r--   0 cronsholt   (501) staff       (20)     7314 2023-05-01 07:55:40.000000 polar_api-1.0.0/polar_api/PolarAPI.py
+-rw-r--r--   0 cronsholt   (501) staff       (20)       94 2023-04-22 06:14:40.000000 polar_api-1.0.0/polar_api/__init__.py
+-rw-r--r--   0 cronsholt   (501) staff       (20)    30259 2023-04-14 08:55:43.000000 polar_api-1.0.0/polar_api/cleaning.py
+-rw-r--r--   0 cronsholt   (501) staff       (20)     6417 2023-04-14 10:45:49.000000 polar_api-1.0.0/polar_api/polar_api.py
+drwxr-xr-x   0 cronsholt   (501) staff       (20)        0 2023-05-01 08:09:22.541529 polar_api-1.0.0/polar_api.egg-info/
+-rw-r--r--   0 cronsholt   (501) staff       (20)      156 2023-05-01 08:09:22.000000 polar_api-1.0.0/polar_api.egg-info/PKG-INFO
+-rw-r--r--   0 cronsholt   (501) staff       (20)      533 2023-05-01 08:09:22.000000 polar_api-1.0.0/polar_api.egg-info/SOURCES.txt
+-rw-r--r--   0 cronsholt   (501) staff       (20)        1 2023-05-01 08:09:22.000000 polar_api-1.0.0/polar_api.egg-info/dependency_links.txt
+-rw-r--r--   0 cronsholt   (501) staff       (20)       46 2023-05-01 08:09:22.000000 polar_api-1.0.0/polar_api.egg-info/requires.txt
+-rw-r--r--   0 cronsholt   (501) staff       (20)       28 2023-05-01 08:09:22.000000 polar_api-1.0.0/polar_api.egg-info/top_level.txt
+drwxr-xr-x   0 cronsholt   (501) staff       (20)        0 2023-05-01 08:09:22.542886 polar_api-1.0.0/scripts/
+-rw-r--r--   0 cronsholt   (501) staff       (20)        0 2023-04-14 08:55:43.000000 polar_api-1.0.0/scripts/__init__.py
+-rw-r--r--   0 cronsholt   (501) staff       (20)     3063 2023-04-14 08:55:43.000000 polar_api-1.0.0/scripts/download_raw_data.py
+-rw-r--r--   0 cronsholt   (501) staff       (20)      999 2023-04-14 08:55:43.000000 polar_api-1.0.0/scripts/get_player_session_trimmed.py
+-rw-r--r--   0 cronsholt   (501) staff       (20)     3929 2023-04-14 08:55:43.000000 polar_api-1.0.0/scripts/get_session_raw_gps.py
+-rw-r--r--   0 cronsholt   (501) staff       (20)     1828 2023-04-14 08:55:43.000000 polar_api-1.0.0/scripts/gps_data_project.py
+-rw-r--r--   0 cronsholt   (501) staff       (20)     7680 2023-04-14 08:55:43.000000 polar_api-1.0.0/scripts/session_viz.py
+-rw-r--r--   0 cronsholt   (501) staff       (20)       38 2023-05-01 08:09:22.544213 polar_api-1.0.0/setup.cfg
+-rw-r--r--   0 cronsholt   (501) staff       (20)      330 2023-05-01 08:08:19.000000 polar_api-1.0.0/setup.py
+drwxr-xr-x   0 cronsholt   (501) staff       (20)        0 2023-05-01 08:09:22.543492 polar_api-1.0.0/utilities/
+-rw-r--r--   0 cronsholt   (501) staff       (20)        0 2023-04-14 08:55:43.000000 polar_api-1.0.0/utilities/__init__.py
+-rw-r--r--   0 cronsholt   (501) staff       (20)     1595 2023-04-14 08:55:43.000000 polar_api-1.0.0/utilities/metadata.py
+-rw-r--r--   0 cronsholt   (501) staff       (20)      548 2023-04-14 08:55:43.000000 polar_api-1.0.0/utilities/polar_IO.py
+-rw-r--r--   0 cronsholt   (501) staff       (20)    27284 2023-04-26 06:29:30.000000 polar_api-1.0.0/utilities/polar_api_old.py
```

### Comparing `polar_api-0.0.9/README.md` & `polar_api-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `polar_api-0.0.9/polar_api/cleaning.py` & `polar_api-1.0.0/polar_api/cleaning.py`

 * *Files identical despite different names*

### Comparing `polar_api-0.0.9/polar_api/polar_api.py` & `polar_api-1.0.0/polar_api/polar_api.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,178 +1,202 @@
-import requests
-import webbrowser
 import base64
+import webbrowser
+
+import requests
 
 # POLAR API DOCUMENTATION
 # https://www.polar.com/teampro-api/?python#teampro-api
 
 # -------- AUTHORIZATION AND ACCESS TOKENS --------- #
 
 
 class POLAR_API:
     def __init__(self, client_id, client_secret, team):
-
         self.client_id = client_id
         self.client_secret = client_secret
         self.team = team
-        self.authorize_url = 'https://auth.polar.com/oauth/authorize'
-        self.access_token_url = 'https://auth.polar.com/oauth/token'
-        self.authorize_params = {'client_id': self.client_id,
-                                 'response_type': 'code',
-                                 'scope': 'team_read'}
+        self.authorize_url = "https://auth.polar.com/oauth/authorize"
+        self.access_token_url = "https://auth.polar.com/oauth/token"
+        self.authorize_params = {
+            "client_id": self.client_id,
+            "response_type": "code",
+            "scope": "team_read",
+        }
 
-# Authorization
+    # Authorization
 
     def _get_authorization_code(self):
         r = requests.get(self.authorize_url, params=self.authorize_params)
 
         webbrowser.open(r.history[0].url, new=2)
         authorization_code = input("Authorization Code: ")
 
         return authorization_code
 
     def get_tokens(self):
-
-        encoding = self.client_id+':'+self.client_secret
-        message_bytes = encoding.encode('ascii')
+        encoding = self.client_id + ":" + self.client_secret
+        message_bytes = encoding.encode("ascii")
         base64_bytes = base64.b64encode(message_bytes)
-        base64_encoding = base64_bytes.decode('ascii')
-        headers = {'Authorization': 'Basic '+base64_encoding}
+        base64_encoding = base64_bytes.decode("ascii")
+        headers = {"Authorization": "Basic " + base64_encoding}
 
         authorization_code = self._get_authorization_code()
 
         # POST request to get access token
-        access_token_data = {'grant_type': 'authorization_code',
-                             'code': authorization_code}
-        r_post = requests.post(self.access_token_url,
-                               data=access_token_data,
-                               headers=headers)
+        access_token_data = {
+            "grant_type": "authorization_code",
+            "code": authorization_code,
+        }
+        r_post = requests.post(
+            self.access_token_url, data=access_token_data, headers=headers
+        )
         tokens = r_post.json()
 
         return tokens
 
-# Team
+    # Team
 
     def get_teams_info(self, tokens):
-        access_token = tokens['access_token']
+        access_token = tokens["access_token"]
         headers = {
-            'Accept': 'application/json',
-            'Authorization': 'Bearer '+ access_token
+            "Accept": "application/json",
+            "Authorization": "Bearer " + access_token,
         }
-        r = requests.get('https://teampro.api.polar.com/v1/teams',
-                         params={},
-                         headers=headers)
+        r = requests.get(
+            "https://teampro.api.polar.com/v1/teams", params={}, headers=headers
+        )
         teams_info = r.json()
 
         return teams_info
 
     def get_team_players(self, tokens, team_id):
-        access_token = tokens['access_token']
+        access_token = tokens["access_token"]
         headers = {
-            'Accept': 'application/json',
-            'Authorization': 'Bearer '+access_token
+            "Accept": "application/json",
+            "Authorization": "Bearer " + access_token,
         }
-        r = requests.get(f'https://teampro.api.polar.com/v1/teams/{team_id}',
-                         params={},
-                         headers=headers)
+        r = requests.get(
+            f"https://teampro.api.polar.com/v1/teams/{team_id}",
+            params={},
+            headers=headers,
+        )
         players_and_staff = r.json()
 
         return players_and_staff
 
-# Session
+    # Session
 
     def get_session(self, tokens, team_id, date):
-        access_token = tokens['access_token']
+        access_token = tokens["access_token"]
         headers = {
-            'Accept': 'application/json',
-            'Authorization': 'Bearer '+access_token
+            "Accept": "application/json",
+            "Authorization": "Bearer " + access_token,
         }
 
-        day, month, year = date.split('-')
-        r = requests.get(f'https://teampro.api.polar.com/v1/teams/{team_id}/training_sessions',
-                        params={'since': f'{year}-{month}-{day}T00:00:00',
-                                'until': f'{year}-{month}-{day}T23:59:59',
-                                'per_page': '100'},
-                                headers=headers)
+        day, month, year = date.split("-")
+        r = requests.get(
+            f"https://teampro.api.polar.com/v1/teams/{team_id}/training_sessions",
+            params={
+                "since": f"{year}-{month}-{day}T00:00:00",
+                "until": f"{year}-{month}-{day}T23:59:59",
+                "per_page": "100",
+            },
+            headers=headers,
+        )
         sessions_metadata = r.json()
 
         return sessions_metadata
 
     def get_sessions(self, tokens, team_id, dates):
-        access_token = tokens['access_token']
+        access_token = tokens["access_token"]
         headers = {
-            'Accept': 'application/json',
-            'Authorization': 'Bearer '+access_token
+            "Accept": "application/json",
+            "Authorization": "Bearer " + access_token,
         }
 
-        day1, month1, year1 = dates[0].split('-')
-        day2, month2, year2 = dates[1].split('-')
-        r = requests.get(f'https://teampro.api.polar.com/v1/teams/{team_id}/training_sessions',
-                        params={'since': f'{year1}-{month1}-{day1}T00:00:00',
-                                'until': f'{year2}-{month2}-{day2}T23:59:59',
-                                'per_page': '100'},
-                                headers=headers)
-                            
+        day1, month1, year1 = dates[0].split("-")
+        day2, month2, year2 = dates[1].split("-")
+        r = requests.get(
+            f"https://teampro.api.polar.com/v1/teams/{team_id}/training_sessions",
+            params={
+                "since": f"{year1}-{month1}-{day1}T00:00:00",
+                "until": f"{year2}-{month2}-{day2}T23:59:59",
+                "per_page": "100",
+            },
+            headers=headers,
+        )
+
         sessions_metadata = r.json()
 
-        total_pages = sessions_metadata['page']['total_pages']
-        
+        total_pages = sessions_metadata["page"]["total_pages"]
+
         if total_pages > 0:
             all_sessions = []
             for i in range(total_pages):
-                r_new = requests.get(f'https://teampro.api.polar.com/v1/teams/{team_id}/training_sessions?page={i}',
-                                    params={'since': f'{year1}-{month1}-{day1}T00:00:00',
-                                            'until': f'{year2}-{month2}-{day2}T23:59:59'},
-                                    headers=headers)
+                r_new = requests.get(
+                    f"https://teampro.api.polar.com/v1/teams/{team_id}/training_sessions?page={i}",
+                    params={
+                        "since": f"{year1}-{month1}-{day1}T00:00:00",
+                        "until": f"{year2}-{month2}-{day2}T23:59:59",
+                    },
+                    headers=headers,
+                )
 
                 page_data = r_new.json()
-                session_data = page_data['data']
+                session_data = page_data["data"]
                 all_sessions.append(session_data)
-            
-            
+
             # concatenate list of sessions
             flatten_list = lambda l: [item for sublist in l for item in sublist]
             all_sessions = flatten_list(all_sessions)
             sessions_metadata = all_sessions
-            
-            # df_sessions = pd.json_normalize(all_sessions)
 
+            # df_sessions = pd.json_normalize(all_sessions)
 
         return sessions_metadata
 
-# Players
+    # Players
 
     def get_players_session_data(self, tokens, session_id):
-        access_token = tokens['access_token']
+        access_token = tokens["access_token"]
         headers = {
-            'Accept': 'application/json',
-            'Authorization': 'Bearer '+access_token
+            "Accept": "application/json",
+            "Authorization": "Bearer " + access_token,
         }
-        r = requests.get(f'https://teampro.api.polar.com/v1/teams/training_sessions/{session_id}',
-                         params={}, headers=headers)
+        r = requests.get(
+            f"https://teampro.api.polar.com/v1/teams/training_sessions/{session_id}",
+            params={},
+            headers=headers,
+        )
         session_data = r.json()
 
         return session_data
 
     def get_player_session_details(self, tokens, player_session_id):
-        access_token = tokens['access_token']
+        access_token = tokens["access_token"]
         headers = {
-            'Accept': 'application/json',
-            'Authorization': 'Bearer '+access_token
+            "Accept": "application/json",
+            "Authorization": "Bearer " + access_token,
         }
-        r = requests.get(f'https://teampro.api.polar.com/v1/training_sessions/{player_session_id}',
-                         params={'samples': 'all'}, headers=headers)
+        r = requests.get(
+            f"https://teampro.api.polar.com/v1/training_sessions/{player_session_id}",
+            params={"samples": "all"},
+            headers=headers,
+        )
         player_session_details = r.json()
 
         return player_session_details
 
     def get_trimmed_player_session_details(self, tokens, player_session_id):
-        access_token = tokens['access_token']
+        access_token = tokens["access_token"]
         headers = {
-            'Accept': 'application/json',
-            'Authorization': 'Bearer '+access_token
+            "Accept": "application/json",
+            "Authorization": "Bearer " + access_token,
         }
-        r = requests.get(f'https://teampro.api.polar.com/v1/training_sessions/{player_session_id}/session_summary',
-                         params={}, headers=headers)
+        r = requests.get(
+            f"https://teampro.api.polar.com/v1/training_sessions/{player_session_id}/session_summary",
+            params={},
+            headers=headers,
+        )
         session_details = r.json()
 
-        return session_details
+        return session_details
```

### Comparing `polar_api-0.0.9/scripts/download_raw_data.py` & `polar_api-1.0.0/scripts/download_raw_data.py`

 * *Files identical despite different names*

### Comparing `polar_api-0.0.9/scripts/get_player_session_trimmed.py` & `polar_api-1.0.0/scripts/get_player_session_trimmed.py`

 * *Files identical despite different names*

### Comparing `polar_api-0.0.9/scripts/get_session_raw_gps.py` & `polar_api-1.0.0/scripts/get_session_raw_gps.py`

 * *Files identical despite different names*

### Comparing `polar_api-0.0.9/scripts/gps_data_project.py` & `polar_api-1.0.0/scripts/gps_data_project.py`

 * *Files identical despite different names*

### Comparing `polar_api-0.0.9/scripts/session_viz.py` & `polar_api-1.0.0/scripts/session_viz.py`

 * *Files identical despite different names*

### Comparing `polar_api-0.0.9/utilities/metadata.py` & `polar_api-1.0.0/utilities/metadata.py`

 * *Files identical despite different names*

### Comparing `polar_api-0.0.9/utilities/polar_IO.py` & `polar_api-1.0.0/utilities/polar_IO.py`

 * *Files identical despite different names*

### Comparing `polar_api-0.0.9/utilities/polar_api_old.py` & `polar_api-1.0.0/utilities/polar_api_old.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,16 +15,16 @@
                             ACCESS_TOKEN_URL,
                             AUTHORIZE_PARAMS)
 
 # POLAR API
 # https://www.polar.com/teampro-api/?python#teampro-api
 
 # -------- Setup variables -------- #
-CLIENT_ID = 'e6e9caed-4705-4991-97c2-b0c9b66cff67'
-CLIENT_SECRET = 'b1adec70-302e-4209-adae-e031ecfd03fa'
+CLIENT_ID = ''
+CLIENT_SECRET = ''
 # -------- UTILITY FUNCTIONS -------- #
 
 
 def flatten_list(l):
     return [item for sublist in l for item in sublist]
 
 # from https://stackoverflow.com/questions/1060279/iterating-through-a-range-of-dates-in-python
```

