# Comparing `tmp/moonglaive-0.0.8.tar.gz` & `tmp/moonglaive-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moonglaive-0.0.8.tar", last modified: Mon May  1 14:28:27 2023, max compression
+gzip compressed data, was "moonglaive-0.0.9.tar", last modified: Mon May  1 14:31:10 2023, max compression
```

## Comparing `moonglaive-0.0.8.tar` & `moonglaive-0.0.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 14:28:27.654206 moonglaive-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-01 14:28:21.000000 moonglaive-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-05-01 14:28:27.654206 moonglaive-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-05-01 14:28:21.000000 moonglaive-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 14:28:27.654206 moonglaive-0.0.8/moonglaive/
--rwxr-xr-x   0 runner    (1001) docker     (123)      158 2023-05-01 14:28:21.000000 moonglaive-0.0.8/moonglaive/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1570 2023-05-01 14:28:21.000000 moonglaive-0.0.8/moonglaive/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 14:28:27.654206 moonglaive-0.0.8/moonglaive/platforms/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 14:28:21.000000 moonglaive-0.0.8/moonglaive/platforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-05-01 14:28:21.000000 moonglaive-0.0.8/moonglaive/platforms/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-05-01 14:28:21.000000 moonglaive-0.0.8/moonglaive/platforms/code4rena.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-05-01 14:28:21.000000 moonglaive-0.0.8/moonglaive/platforms/sherlock.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 14:28:27.654206 moonglaive-0.0.8/moonglaive/services/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 14:28:21.000000 moonglaive-0.0.8/moonglaive/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-05-01 14:28:21.000000 moonglaive-0.0.8/moonglaive/services/discord.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 14:28:27.654206 moonglaive-0.0.8/moonglaive.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-05-01 14:28:27.000000 moonglaive-0.0.8/moonglaive.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-05-01 14:28:27.000000 moonglaive-0.0.8/moonglaive.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 14:28:27.000000 moonglaive-0.0.8/moonglaive.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-01 14:28:27.000000 moonglaive-0.0.8/moonglaive.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-01 14:28:27.000000 moonglaive-0.0.8/moonglaive.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 14:28:27.654206 moonglaive-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-05-01 14:28:21.000000 moonglaive-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 14:31:10.627965 moonglaive-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-01 14:31:07.000000 moonglaive-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-05-01 14:31:10.627965 moonglaive-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-05-01 14:31:07.000000 moonglaive-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 14:31:10.627965 moonglaive-0.0.9/moonglaive/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      158 2023-05-01 14:31:07.000000 moonglaive-0.0.9/moonglaive/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1592 2023-05-01 14:31:07.000000 moonglaive-0.0.9/moonglaive/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 14:31:10.627965 moonglaive-0.0.9/moonglaive/platforms/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 14:31:07.000000 moonglaive-0.0.9/moonglaive/platforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-05-01 14:31:07.000000 moonglaive-0.0.9/moonglaive/platforms/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-05-01 14:31:07.000000 moonglaive-0.0.9/moonglaive/platforms/code4rena.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-01 14:31:07.000000 moonglaive-0.0.9/moonglaive/platforms/sherlock.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 14:31:10.627965 moonglaive-0.0.9/moonglaive/services/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 14:31:07.000000 moonglaive-0.0.9/moonglaive/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-05-01 14:31:07.000000 moonglaive-0.0.9/moonglaive/services/discord.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 14:31:10.627965 moonglaive-0.0.9/moonglaive.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-05-01 14:31:10.000000 moonglaive-0.0.9/moonglaive.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-05-01 14:31:10.000000 moonglaive-0.0.9/moonglaive.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 14:31:10.000000 moonglaive-0.0.9/moonglaive.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-01 14:31:10.000000 moonglaive-0.0.9/moonglaive.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-01 14:31:10.000000 moonglaive-0.0.9/moonglaive.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 14:31:10.627965 moonglaive-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-05-01 14:31:07.000000 moonglaive-0.0.9/setup.py
```

### Comparing `moonglaive-0.0.8/LICENSE` & `moonglaive-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `moonglaive-0.0.8/PKG-INFO` & `moonglaive-0.0.9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moonglaive
-Version: 0.0.8
+Version: 0.0.9
 Summary: Three-bladed weapon of the night elf Sentinels
 Home-page: https://github.com/MalfurionWhitehat/moonglaive
 Author: MalfurionWhitehat
 Author-email: MalfurionWhitehat@proton.me
 License: MIT
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
```

### Comparing `moonglaive-0.0.8/README.md` & `moonglaive-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `moonglaive-0.0.8/moonglaive/__main__.py` & `moonglaive-0.0.9/moonglaive/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python3
 
 import argparse
 from tabulate import tabulate
 
-from platforms.code4rena import Code4rena
-from platforms.sherlock import Sherlock
+from moonglaive.platforms.code4rena import Code4rena
+from moonglaive.platforms.sherlock import Sherlock
 
 parser = argparse.ArgumentParser(
     description='Three-bladed weapon of the night elf Sentinels.')
 parser.add_argument('--active', help='Active audit contests',
                     action=argparse.BooleanOptionalAction)
 parser.add_argument('--upcoming', help='Upcoming audit contests',
                     action=argparse.BooleanOptionalAction)
```

### Comparing `moonglaive-0.0.8/moonglaive/platforms/base.py` & `moonglaive-0.0.9/moonglaive/platforms/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import re
 from typing import Dict
 from datetime import datetime
 from fuzzywuzzy import fuzz
 
-from services.discord import Channel, Discord
+from moonglaive.services.discord import Channel, Discord
 
 
 class Base():
     discord_guild_id = None
     discord = None
     channels = []
```

### Comparing `moonglaive-0.0.8/moonglaive/platforms/code4rena.py` & `moonglaive-0.0.9/moonglaive/platforms/code4rena.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Dict, List
 import requests
 from dateutil import parser as date
 from re import sub
 from decimal import Decimal
 
-from .base import Base
+from moonglaive.platforms.base import Base
 
 
 class Code4rena(Base):
     discord_guild_id = '810916927919620096'
 
     def __init__(self, discord_authorization: str):
         super().__init__(discord_authorization)
```

### Comparing `moonglaive-0.0.8/moonglaive/platforms/sherlock.py` & `moonglaive-0.0.9/moonglaive/platforms/sherlock.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Dict, List
 import requests
 
-from .base import Base
+from moonglaive.platforms.base import Base
 
 
 class Sherlock(Base):
     discord_guild_id = '812037309376495636'
 
     def __init__(self, discord_authorization: str):
         super().__init__(discord_authorization)
```

### Comparing `moonglaive-0.0.8/moonglaive/services/discord.py` & `moonglaive-0.0.9/moonglaive/services/discord.py`

 * *Files identical despite different names*

### Comparing `moonglaive-0.0.8/moonglaive.egg-info/PKG-INFO` & `moonglaive-0.0.9/moonglaive.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moonglaive
-Version: 0.0.8
+Version: 0.0.9
 Summary: Three-bladed weapon of the night elf Sentinels
 Home-page: https://github.com/MalfurionWhitehat/moonglaive
 Author: MalfurionWhitehat
 Author-email: MalfurionWhitehat@proton.me
 License: MIT
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
```

### Comparing `moonglaive-0.0.8/setup.py` & `moonglaive-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='moonglaive',
-    version='0.0.8',
+    version='0.0.9',
     description='Three-bladed weapon of the night elf Sentinels',
     url='https://github.com/MalfurionWhitehat/moonglaive',
     author='MalfurionWhitehat',
     author_email='MalfurionWhitehat@proton.me',
     license='MIT',
     packages=find_packages(),
     install_requires=[
```

