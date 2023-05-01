# Comparing `tmp/nextguild-1.1.2.tar.gz` & `tmp/nextguild-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nextguild-1.1.2.tar", last modified: Mon May  1 17:57:39 2023, max compression
+gzip compressed data, was "nextguild-1.1.3.tar", last modified: Mon May  1 21:38:00 2023, max compression
```

## Comparing `nextguild-1.1.2.tar` & `nextguild-1.1.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:57:39.787992 nextguild-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-01 17:57:26.000000 nextguild-1.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-05-01 17:57:39.787992 nextguild-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-05-01 17:57:26.000000 nextguild-1.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:57:39.787992 nextguild-1.1.2/nextguild/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-01 17:57:26.000000 nextguild-1.1.2/nextguild/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-01 17:57:26.000000 nextguild-1.1.2/nextguild/channel.py
--rw-r--r--   0 runner    (1001) docker     (123)    36765 2023-05-01 17:57:26.000000 nextguild-1.1.2/nextguild/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-05-01 17:57:26.000000 nextguild-1.1.2/nextguild/embed.py
--rw-r--r--   0 runner    (1001) docker     (123)    42726 2023-05-01 17:57:26.000000 nextguild-1.1.2/nextguild/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-05-01 17:57:26.000000 nextguild-1.1.2/nextguild/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-05-01 17:57:26.000000 nextguild-1.1.2/nextguild/reaction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:57:39.787992 nextguild-1.1.2/nextguild.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-05-01 17:57:39.000000 nextguild-1.1.2/nextguild.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-01 17:57:39.000000 nextguild-1.1.2/nextguild.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 17:57:39.000000 nextguild-1.1.2/nextguild.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-01 17:57:39.000000 nextguild-1.1.2/nextguild.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-05-01 17:57:26.000000 nextguild-1.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 17:57:39.787992 nextguild-1.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:38:00.486765 nextguild-1.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-01 21:37:43.000000 nextguild-1.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-05-01 21:38:00.482765 nextguild-1.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-05-01 21:37:43.000000 nextguild-1.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:38:00.482765 nextguild-1.1.3/nextguild/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-01 21:37:43.000000 nextguild-1.1.3/nextguild/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-01 21:37:43.000000 nextguild-1.1.3/nextguild/channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36828 2023-05-01 21:37:43.000000 nextguild-1.1.3/nextguild/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-05-01 21:37:43.000000 nextguild-1.1.3/nextguild/embed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42840 2023-05-01 21:37:43.000000 nextguild-1.1.3/nextguild/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-05-01 21:37:43.000000 nextguild-1.1.3/nextguild/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-05-01 21:37:43.000000 nextguild-1.1.3/nextguild/reaction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:38:00.482765 nextguild-1.1.3/nextguild.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-05-01 21:38:00.000000 nextguild-1.1.3/nextguild.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-01 21:38:00.000000 nextguild-1.1.3/nextguild.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 21:38:00.000000 nextguild-1.1.3/nextguild.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-01 21:38:00.000000 nextguild-1.1.3/nextguild.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-05-01 21:37:43.000000 nextguild-1.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 21:38:00.486765 nextguild-1.1.3/setup.cfg
```

### Comparing `nextguild-1.1.2/LICENSE` & `nextguild-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nextguild-1.1.2/PKG-INFO` & `nextguild-1.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nextguild
-Version: 1.1.2
+Version: 1.1.3
 Summary: Interactions with the Guilded API made simpler
 Author-email: Arjun Sharda <sharda.aj17@gmail.com>, Erik Thorsell <contact@erikthorsell.com>
 License: MIT License
         
         Copyright (c) 2023 Arjun Sharda
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `nextguild-1.1.2/README.md` & `nextguild-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `nextguild-1.1.2/nextguild/channel.py` & `nextguild-1.1.3/nextguild/channel.py`

 * *Files identical despite different names*

### Comparing `nextguild-1.1.2/nextguild/client.py` & `nextguild-1.1.3/nextguild/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1047,24 +1047,26 @@
             emote_id: int
     ):
         response = self.request(
             'PUT',
             f'{self.base_url}/channels/{channel_id}/messages/{message_id}/emotes/{emote_id}'
         )
         return response
-
+    
     def delete_message_reaction(
             self,
             channel_id: str,
             message_id: str,
-            emote_id: int
+            emote_id: int,
+            user_id: str
     ):
         response = self.request(
             'DELETE',
-            f'{self.base_url}/channels/{channel_id}/messages/{message_id}/emotes/{emote_id}'
+            f'{self.base_url}/channels/{channel_id}/messages/{message_id}/emotes/{emote_id}',
+            params={'userId': user_id}
         )
         return response
 
     def create_topic_reaction(
             self,
             channel_id: str,
             topic_id: int,
@@ -1331,15 +1333,15 @@
             f'{self.base_url}/channels/{channel_id}/docs/{doc_id}/comments/'
             f'{comment_id}'
         )
         return response
 
     def get_bot_user_id(self):
         response = self.request('GET', f'{self.base_url}/users/@me')
-        return response.json()['user']['id']
+        return response['user']['id']
     
     def get_user_servers(self, user_id: str):
         response = self.request('GET', f'{self.base_url}users/{user_id}/servers')
         return response
 
     def get_bot_servers(self):
         response = self.request('GET', f'{self.base_url}/users/@me/servers')
```

### Comparing `nextguild-1.1.2/nextguild/embed.py` & `nextguild-1.1.3/nextguild/embed.py`

 * *Files identical despite different names*

### Comparing `nextguild-1.1.2/nextguild/events.py` & `nextguild-1.1.3/nextguild/events.py`

 * *Files 0% similar despite different names*

```diff
@@ -978,24 +978,27 @@
             await handler(event_data)
 
     async def _handle_list_item_uncompleted(self, event_data):
         for handler in self._list_item_uncomplete_handlers:
             await handler(event_data)
 
     async def _handle_channel_message_reaction_created(self, event_data):
+        reaction = Reaction(event_data)
         for handler in self._channel_message_reaction_create_handlers:
-            await handler(event_data)
+            await handler(reaction)
 
     async def _handle_channel_message_reaction_deleted(self, event_data):
+        reaction = Reaction(event_data)
         for handler in self._channel_message_reaction_delete_handlers:
-            await handler(event_data)
+            await handler(reaction)
 
     async def _handle_channel_message_reaction_many_deleted(self, event_data):
+        reaction = Reaction(event_data)
         for handler in self._channel_message_reaction_many_delete_handlers:
-            await handler(event_data)
+            await handler(reaction)
     
     async def _handle_calendar_event_comment_created(self, event_data):
         for handler in self._calendar_event_comment_create_handlers:
             await handler(event_data)
 
     async def _handle_calendar_event_comment_updated(self, event_data):
         for handler in self._calendar_event_comment_update_handlers:
```

### Comparing `nextguild-1.1.2/nextguild/message.py` & `nextguild-1.1.3/nextguild/message.py`

 * *Files identical despite different names*

### Comparing `nextguild-1.1.2/nextguild/reaction.py` & `nextguild-1.1.3/nextguild/reaction.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # -*- coding: utf-8 -*-
 class Reaction:
     def __init__(self, event_data: dict):
         self.event_data: dict = event_data
+        self.message_id: str = event_data.get('reaction', {}).get('messageId')
         self.server_id: str = event_data.get('serverId')
         self.channel_id: str = event_data.get('reaction', {}).get('channelId')
         self.user_id: str = event_data.get('reaction', {}).get('createdBy')
         self.emote_name: str = event_data.get('reaction', {}).get(
             'emote', {}
         ).get('name')
         self.emote_id: str = event_data.get('reaction', {}).get(
```

### Comparing `nextguild-1.1.2/nextguild.egg-info/PKG-INFO` & `nextguild-1.1.3/nextguild.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nextguild
-Version: 1.1.2
+Version: 1.1.3
 Summary: Interactions with the Guilded API made simpler
 Author-email: Arjun Sharda <sharda.aj17@gmail.com>, Erik Thorsell <contact@erikthorsell.com>
 License: MIT License
         
         Copyright (c) 2023 Arjun Sharda
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `nextguild-1.1.2/pyproject.toml` & `nextguild-1.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "requests", "asyncio", "websockets"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nextguild"
-version = "1.1.2"
+version = "1.1.3"
 authors = [
     { name="Arjun Sharda", email="sharda.aj17@gmail.com" },
     { name="Erik Thorsell", email="contact@erikthorsell.com" },
 ]
 description = "Interactions with the Guilded API made simpler"
 readme = "README.md"
 license = { file="LICENSE" }
```

