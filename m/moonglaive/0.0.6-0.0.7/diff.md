# Comparing `tmp/moonglaive-0.0.6.tar.gz` & `tmp/moonglaive-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/moonglaive-0.0.6.tar", last modified: Sat Apr  8 16:47:41 2023, max compression
+gzip compressed data, was "moonglaive-0.0.7.tar", last modified: Mon May  1 13:32:22 2023, max compression
```

## Comparing `moonglaive-0.0.6.tar` & `moonglaive-0.0.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 user       (502) staff       (20)        0 2023-04-08 16:47:41.000000 moonglaive-0.0.6/
--rw-r--r--   0 user       (502) staff       (20)      730 2023-04-08 16:47:41.000000 moonglaive-0.0.6/PKG-INFO
-drwxr-xr-x   0 user       (502) staff       (20)        0 2023-04-08 16:47:41.000000 moonglaive-0.0.6/moonglaive.egg-info/
--rw-r--r--   0 user       (502) staff       (20)      730 2023-04-08 16:47:41.000000 moonglaive-0.0.6/moonglaive.egg-info/PKG-INFO
--rw-r--r--   0 user       (502) staff       (20)      433 2023-04-08 16:47:41.000000 moonglaive-0.0.6/moonglaive.egg-info/SOURCES.txt
--rw-r--r--   0 user       (502) staff       (20)       89 2023-04-08 16:47:41.000000 moonglaive-0.0.6/moonglaive.egg-info/requires.txt
--rw-r--r--   0 user       (502) staff       (20)       11 2023-04-08 16:47:41.000000 moonglaive-0.0.6/moonglaive.egg-info/top_level.txt
--rw-r--r--   0 user       (502) staff       (20)        1 2023-04-08 16:47:41.000000 moonglaive-0.0.6/moonglaive.egg-info/dependency_links.txt
--rw-r--r--   0 user       (502) staff       (20)     1074 2023-02-23 18:06:50.000000 moonglaive-0.0.6/LICENSE
--rw-r--r--   0 user       (502) staff       (20)       60 2023-02-23 18:06:50.000000 moonglaive-0.0.6/README.md
--rw-r--r--   0 user       (502) staff       (20)     1011 2023-04-08 16:47:32.000000 moonglaive-0.0.6/setup.py
-drwxr-xr-x   0 user       (502) staff       (20)        0 2023-04-08 16:47:41.000000 moonglaive-0.0.6/moonglaive/
-drwxr-xr-x   0 user       (502) staff       (20)        0 2023-04-08 16:47:41.000000 moonglaive-0.0.6/moonglaive/platforms/
--rw-r--r--   0 user       (502) staff       (20)      920 2023-04-08 16:47:25.000000 moonglaive-0.0.6/moonglaive/platforms/sherlock.py
--rw-r--r--   0 user       (502) staff       (20)     1234 2023-04-08 16:47:24.000000 moonglaive-0.0.6/moonglaive/platforms/code4rena.py
--rwxr-xr-x   0 user       (502) staff       (20)        0 2023-04-08 16:30:28.000000 moonglaive-0.0.6/moonglaive/platforms/__init__.py
--rw-r--r--   0 user       (502) staff       (20)     4050 2023-04-08 16:47:28.000000 moonglaive-0.0.6/moonglaive/platforms/base.py
--rwxr-xr-x   0 user       (502) staff       (20)      158 2023-04-08 16:21:54.000000 moonglaive-0.0.6/moonglaive/__init__.py
--rwxr-xr-x   0 user       (502) staff       (20)     1502 2023-04-08 16:47:21.000000 moonglaive-0.0.6/moonglaive/__main__.py
-drwxr-xr-x   0 user       (502) staff       (20)        0 2023-04-08 16:47:41.000000 moonglaive-0.0.6/moonglaive/services/
--rw-r--r--   0 user       (502) staff       (20)     1446 2023-03-04 05:16:49.000000 moonglaive-0.0.6/moonglaive/services/discord.py
--rwxr-xr-x   0 user       (502) staff       (20)        0 2023-04-08 16:30:32.000000 moonglaive-0.0.6/moonglaive/services/__init__.py
--rw-r--r--   0 user       (502) staff       (20)       38 2023-04-08 16:47:41.000000 moonglaive-0.0.6/setup.cfg
+drwxr-xr-x   0 user       (502) staff       (20)        0 2023-05-01 13:32:22.370720 moonglaive-0.0.7/
+-rw-r--r--   0 user       (502) staff       (20)     1074 2023-02-23 18:06:50.000000 moonglaive-0.0.7/LICENSE
+-rw-r--r--   0 user       (502) staff       (20)      713 2023-05-01 13:32:22.370593 moonglaive-0.0.7/PKG-INFO
+-rw-r--r--   0 user       (502) staff       (20)     1281 2023-04-08 16:51:21.000000 moonglaive-0.0.7/README.md
+drwxr-xr-x   0 user       (502) staff       (20)        0 2023-05-01 13:32:22.369079 moonglaive-0.0.7/moonglaive/
+-rwxr-xr-x   0 user       (502) staff       (20)      158 2023-04-08 16:21:54.000000 moonglaive-0.0.7/moonglaive/__init__.py
+-rwxr-xr-x   0 user       (502) staff       (20)     1555 2023-05-01 13:27:36.000000 moonglaive-0.0.7/moonglaive/__main__.py
+drwxr-xr-x   0 user       (502) staff       (20)        0 2023-05-01 13:32:22.370116 moonglaive-0.0.7/moonglaive/platforms/
+-rwxr-xr-x   0 user       (502) staff       (20)        0 2023-04-08 16:30:28.000000 moonglaive-0.0.7/moonglaive/platforms/__init__.py
+-rw-r--r--   0 user       (502) staff       (20)     4196 2023-05-01 13:28:56.000000 moonglaive-0.0.7/moonglaive/platforms/base.py
+-rw-r--r--   0 user       (502) staff       (20)     1234 2023-05-01 13:29:27.000000 moonglaive-0.0.7/moonglaive/platforms/code4rena.py
+-rw-r--r--   0 user       (502) staff       (20)      920 2023-04-08 16:47:25.000000 moonglaive-0.0.7/moonglaive/platforms/sherlock.py
+drwxr-xr-x   0 user       (502) staff       (20)        0 2023-05-01 13:32:22.370380 moonglaive-0.0.7/moonglaive/services/
+-rwxr-xr-x   0 user       (502) staff       (20)        0 2023-04-08 16:30:32.000000 moonglaive-0.0.7/moonglaive/services/__init__.py
+-rw-r--r--   0 user       (502) staff       (20)     1423 2023-05-01 13:27:08.000000 moonglaive-0.0.7/moonglaive/services/discord.py
+drwxr-xr-x   0 user       (502) staff       (20)        0 2023-05-01 13:32:22.369667 moonglaive-0.0.7/moonglaive.egg-info/
+-rw-r--r--   0 user       (502) staff       (20)      713 2023-05-01 13:32:22.000000 moonglaive-0.0.7/moonglaive.egg-info/PKG-INFO
+-rw-r--r--   0 user       (502) staff       (20)      433 2023-05-01 13:32:22.000000 moonglaive-0.0.7/moonglaive.egg-info/SOURCES.txt
+-rw-r--r--   0 user       (502) staff       (20)        1 2023-05-01 13:32:22.000000 moonglaive-0.0.7/moonglaive.egg-info/dependency_links.txt
+-rw-r--r--   0 user       (502) staff       (20)       89 2023-05-01 13:32:22.000000 moonglaive-0.0.7/moonglaive.egg-info/requires.txt
+-rw-r--r--   0 user       (502) staff       (20)       11 2023-05-01 13:32:22.000000 moonglaive-0.0.7/moonglaive.egg-info/top_level.txt
+-rw-r--r--   0 user       (502) staff       (20)       38 2023-05-01 13:32:22.370760 moonglaive-0.0.7/setup.cfg
+-rw-r--r--   0 user       (502) staff       (20)     1011 2023-05-01 13:30:28.000000 moonglaive-0.0.7/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `moonglaive-0.0.6/PKG-INFO` & `moonglaive-0.0.7/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,18 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: moonglaive
-Version: 0.0.6
+Version: 0.0.7
 Summary: Three-bladed weapon of the night elf Sentinels
 Home-page: https://github.com/MalfurionWhitehat/moonglaive
 Author: MalfurionWhitehat
 Author-email: MalfurionWhitehat@proton.me
 License: MIT
-Description: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
+License-File: LICENSE
```

### Comparing `moonglaive-0.0.6/moonglaive.egg-info/PKG-INFO` & `moonglaive-0.0.7/moonglaive.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,18 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: moonglaive
-Version: 0.0.6
+Version: 0.0.7
 Summary: Three-bladed weapon of the night elf Sentinels
 Home-page: https://github.com/MalfurionWhitehat/moonglaive
 Author: MalfurionWhitehat
 Author-email: MalfurionWhitehat@proton.me
 License: MIT
-Description: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
+License-File: LICENSE
```

### Comparing `moonglaive-0.0.6/LICENSE` & `moonglaive-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `moonglaive-0.0.6/setup.py` & `moonglaive-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='moonglaive',
-    version='0.0.6',
+    version='0.0.7',
     description='Three-bladed weapon of the night elf Sentinels',
     url='https://github.com/MalfurionWhitehat/moonglaive',
     author='MalfurionWhitehat',
     author_email='MalfurionWhitehat@proton.me',
     license='MIT',
     packages=find_packages(),
     install_requires=[
```

### Comparing `moonglaive-0.0.6/moonglaive/platforms/sherlock.py` & `moonglaive-0.0.7/moonglaive/platforms/sherlock.py`

 * *Files identical despite different names*

### Comparing `moonglaive-0.0.6/moonglaive/platforms/code4rena.py` & `moonglaive-0.0.7/moonglaive/platforms/code4rena.py`

 * *Files identical despite different names*

### Comparing `moonglaive-0.0.6/moonglaive/platforms/base.py` & `moonglaive-0.0.7/moonglaive/platforms/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -83,18 +83,21 @@
             contest_approx_channel_name, channel['name']),
             channels_with_specific_date))
 
         if fuzz_ratio_list:
             max_value = max(fuzz_ratio_list)
             index = fuzz_ratio_list.index(max_value)
             channel = channels_with_specific_date[index]
+            messages = self.discord.get_messages(channel['id'])
             return dict(channel,
                         **{
                             'users': self.discord.
-                            get_users_count_from_messages(channel['id'])
+                            get_users_count_from_messages(messages),
+                            'messages': len(messages)
                         })
         else:
             return {
                 'id': '',
                 'name': '',
-                'users': ''
+                'users': '',
+                'messages': ''
             }
```

### Comparing `moonglaive-0.0.6/moonglaive/__main__.py` & `moonglaive-0.0.7/moonglaive/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#!/usr/bin/env python3
+
 import argparse
 from tabulate import tabulate
 
 from moonglaive.platforms.code4rena import Code4rena
 from moonglaive.platforms.sherlock import Sherlock
 
 parser = argparse.ArgumentParser(
@@ -23,16 +25,16 @@
 contests = Code4rena(args.discord_authorization).get_contests(
     filters) + Sherlock(args.discord_authorization).get_contests(filters)
 
 
 header = ['platform', 'title', 'eta', 'reward']
 colalign = ['left', 'left', 'right', 'right']
 if args.discord_authorization is not None:
-    header += ['channel.name', 'channel.users']
-    colalign += ['right', 'right']
+    header += ['channel.name', 'channel.users', 'channel.messages']
+    colalign += ['right', 'right', 'right']
 
 rows = []
 for contest in contests:
     row = []
     for col in header:
         if '.' in col:
             [first, second] = col.split('.')
```

### Comparing `moonglaive-0.0.6/moonglaive/services/discord.py` & `moonglaive-0.0.7/moonglaive/services/discord.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from typing import List
 import requests
 
 
 class Channel:
     id: str
     name: str
-    users: int
+    users: str
+    messages: str
 
 
 class User:
     id: str
     username: str
     discriminator: int
 
@@ -41,16 +42,15 @@
         response = requests.get(
             f'https://discord.com/api/channels/{channel_id}/messages?limit=100',
             headers=headers
         )
         body = response.json()
         return body
 
-    def get_users_count_from_messages(self, channel_id: str) -> str:
-        messages = self.get_messages(channel_id)
+    def get_users_count_from_messages(self, messages: List[Message]) -> str:
         if type(messages) is list:
             users_list = list(map(
                 lambda message: message['author']['username'] +
                 message['author']['discriminator'], messages))
             counts = {user: users_list.count(user) for user in users_list}
             return str(len(counts))
         else:
```

