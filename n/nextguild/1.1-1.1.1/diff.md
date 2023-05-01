# Comparing `tmp/nextguild-1.1.tar.gz` & `tmp/nextguild-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nextguild-1.1.tar", last modified: Mon May  1 13:43:23 2023, max compression
+gzip compressed data, was "nextguild-1.1.1.tar", last modified: Mon May  1 17:48:41 2023, max compression
```

## Comparing `nextguild-1.1.tar` & `nextguild-1.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 13:43:23.928362 nextguild-1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-01 13:43:12.000000 nextguild-1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-05-01 13:43:23.928362 nextguild-1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-05-01 13:43:12.000000 nextguild-1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 13:43:23.928362 nextguild-1.1/nextguild/
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-01 13:43:12.000000 nextguild-1.1/nextguild/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-01 13:43:12.000000 nextguild-1.1/nextguild/channel.py
--rw-r--r--   0 runner    (1001) docker     (123)    36763 2023-05-01 13:43:12.000000 nextguild-1.1/nextguild/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-05-01 13:43:12.000000 nextguild-1.1/nextguild/embed.py
--rw-r--r--   0 runner    (1001) docker     (123)    42723 2023-05-01 13:43:12.000000 nextguild-1.1/nextguild/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-05-01 13:43:12.000000 nextguild-1.1/nextguild/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-05-01 13:43:12.000000 nextguild-1.1/nextguild/reaction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 13:43:23.928362 nextguild-1.1/nextguild.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-05-01 13:43:23.000000 nextguild-1.1/nextguild.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-01 13:43:23.000000 nextguild-1.1/nextguild.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 13:43:23.000000 nextguild-1.1/nextguild.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-01 13:43:23.000000 nextguild-1.1/nextguild.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-01 13:43:12.000000 nextguild-1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 13:43:23.928362 nextguild-1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:48:41.162407 nextguild-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-01 17:48:25.000000 nextguild-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-05-01 17:48:41.162407 nextguild-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-05-01 17:48:25.000000 nextguild-1.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:48:41.162407 nextguild-1.1.1/nextguild/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-01 17:48:25.000000 nextguild-1.1.1/nextguild/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-01 17:48:25.000000 nextguild-1.1.1/nextguild/channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36763 2023-05-01 17:48:25.000000 nextguild-1.1.1/nextguild/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-05-01 17:48:25.000000 nextguild-1.1.1/nextguild/embed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42723 2023-05-01 17:48:25.000000 nextguild-1.1.1/nextguild/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-05-01 17:48:25.000000 nextguild-1.1.1/nextguild/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-05-01 17:48:25.000000 nextguild-1.1.1/nextguild/reaction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:48:41.162407 nextguild-1.1.1/nextguild.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-05-01 17:48:41.000000 nextguild-1.1.1/nextguild.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-01 17:48:41.000000 nextguild-1.1.1/nextguild.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 17:48:41.000000 nextguild-1.1.1/nextguild.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-01 17:48:41.000000 nextguild-1.1.1/nextguild.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-05-01 17:48:25.000000 nextguild-1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 17:48:41.166407 nextguild-1.1.1/setup.cfg
```

### Comparing `nextguild-1.1/LICENSE` & `nextguild-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nextguild-1.1/PKG-INFO` & `nextguild-1.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: nextguild
-Version: 1.1
+Version: 1.1.1
 Summary: Interactions with the Guilded API made simpler
-Author-email: Arjun Sharda <sharda.aj17@gmail.com>
+Author-email: Arjun Sharda <sharda.aj17@gmail.com>, Erik Thorsell <contact@erikthorsell.com>
 License: MIT License
         
         Copyright (c) 2023 Arjun Sharda
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `nextguild-1.1/README.md` & `nextguild-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `nextguild-1.1/nextguild/channel.py` & `nextguild-1.1.1/nextguild/channel.py`

 * *Files identical despite different names*

### Comparing `nextguild-1.1/nextguild/client.py` & `nextguild-1.1.1/nextguild/client.py`

 * *Files identical despite different names*

### Comparing `nextguild-1.1/nextguild/embed.py` & `nextguild-1.1.1/nextguild/embed.py`

 * *Files identical despite different names*

### Comparing `nextguild-1.1/nextguild/events.py` & `nextguild-1.1.1/nextguild/events.py`

 * *Files identical despite different names*

### Comparing `nextguild-1.1/nextguild/message.py` & `nextguild-1.1.1/nextguild/message.py`

 * *Files identical despite different names*

### Comparing `nextguild-1.1/nextguild/reaction.py` & `nextguild-1.1.1/nextguild/reaction.py`

 * *Files identical despite different names*

### Comparing `nextguild-1.1/nextguild.egg-info/PKG-INFO` & `nextguild-1.1.1/nextguild.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: nextguild
-Version: 1.1
+Version: 1.1.1
 Summary: Interactions with the Guilded API made simpler
-Author-email: Arjun Sharda <sharda.aj17@gmail.com>
+Author-email: Arjun Sharda <sharda.aj17@gmail.com>, Erik Thorsell <contact@erikthorsell.com>
 License: MIT License
         
         Copyright (c) 2023 Arjun Sharda
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `nextguild-1.1/pyproject.toml` & `nextguild-1.1.1/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 [build-system]
 requires = ["setuptools", "requests", "asyncio", "websockets"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nextguild"
-version = "1.1"
+version = "1.1.1"
 authors = [
     { name="Arjun Sharda", email="sharda.aj17@gmail.com" },
+    { name="Erik Thorsell", email="contact@erikthorsell.com" },
 ]
 description = "Interactions with the Guilded API made simpler"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
```

