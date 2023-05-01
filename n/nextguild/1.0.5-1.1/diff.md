# Comparing `tmp/nextguild-1.0.5.tar.gz` & `tmp/nextguild-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nextguild-1.0.5.tar", last modified: Sat Mar 25 20:37:12 2023, max compression
+gzip compressed data, was "nextguild-1.1.tar", last modified: Mon May  1 13:43:23 2023, max compression
```

## Comparing `nextguild-1.0.5.tar` & `nextguild-1.1.tar`

### file list

```diff
@@ -1,13 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 20:37:12.131298 nextguild-1.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-03-25 20:36:57.000000 nextguild-1.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-03-25 20:37:12.131298 nextguild-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-03-25 20:36:57.000000 nextguild-1.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 20:37:12.131298 nextguild-1.0.5/nextguild/
--rw-r--r--   0 runner    (1001) docker     (123)    36587 2023-03-25 20:36:57.000000 nextguild-1.0.5/nextguild/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 20:37:12.131298 nextguild-1.0.5/nextguild.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-03-25 20:37:12.000000 nextguild-1.0.5/nextguild.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-03-25 20:37:12.000000 nextguild-1.0.5/nextguild.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-25 20:37:12.000000 nextguild-1.0.5/nextguild.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-25 20:37:12.000000 nextguild-1.0.5/nextguild.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-03-25 20:36:57.000000 nextguild-1.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-25 20:37:12.131298 nextguild-1.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 13:43:23.928362 nextguild-1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-01 13:43:12.000000 nextguild-1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-05-01 13:43:23.928362 nextguild-1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-05-01 13:43:12.000000 nextguild-1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 13:43:23.928362 nextguild-1.1/nextguild/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-01 13:43:12.000000 nextguild-1.1/nextguild/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-01 13:43:12.000000 nextguild-1.1/nextguild/channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36763 2023-05-01 13:43:12.000000 nextguild-1.1/nextguild/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-05-01 13:43:12.000000 nextguild-1.1/nextguild/embed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42723 2023-05-01 13:43:12.000000 nextguild-1.1/nextguild/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-05-01 13:43:12.000000 nextguild-1.1/nextguild/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-05-01 13:43:12.000000 nextguild-1.1/nextguild/reaction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 13:43:23.928362 nextguild-1.1/nextguild.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-05-01 13:43:23.000000 nextguild-1.1/nextguild.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-01 13:43:23.000000 nextguild-1.1/nextguild.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 13:43:23.000000 nextguild-1.1/nextguild.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-01 13:43:23.000000 nextguild-1.1/nextguild.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-01 13:43:12.000000 nextguild-1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 13:43:23.928362 nextguild-1.1/setup.cfg
```

### Comparing `nextguild-1.0.5/LICENSE` & `nextguild-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nextguild-1.0.5/PKG-INFO` & `nextguild-1.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nextguild
-Version: 1.0.5
+Version: 1.1
 Summary: Interactions with the Guilded API made simpler
 Author-email: Arjun Sharda <sharda.aj17@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Arjun Sharda
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -31,28 +31,27 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # NextGuild
-![image](https://user-images.githubusercontent.com/77706434/225704407-da247647-9c9f-4115-a2f1-93d567f46ea7.png)
+![image](https://user-images.githubusercontent.com/108808053/235311374-bdcdcdac-3c04-4b86-b336-1d2a02f5e914.png)
+
+
+
 
 # About
 
 NextGuild is a Guilded API wrapper written in Python.
 
 Planning on being the most simplest python library interacting with the Guilded API, Nextguild is planning to be beginner-friendly and be a great resource to learn Python programming, this is a library, with easy configuration.
 
 Made from a team of 2 people, this was a simple project originally thought for a fun purpose and for testing the Guilded API, which eventually turned into a bot library for multi-purpose use.
 
-
-# Development
-
-Currently, NextGuild is not at a stable version and it is not recommended to use the package until a stable version is released.
 ## Installation
 
 Use the Python Package Index package manager [pip](https://pip.pypa.io/en/stable/) to install NextGuild to start using this package for your project.
 
 ```bash
 pip install nextguild
 ```
```

### Comparing `nextguild-1.0.5/README.md` & `nextguild-1.1/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 # NextGuild
-![image](https://user-images.githubusercontent.com/77706434/225704407-da247647-9c9f-4115-a2f1-93d567f46ea7.png)
+![image](https://user-images.githubusercontent.com/108808053/235311374-bdcdcdac-3c04-4b86-b336-1d2a02f5e914.png)
+
+
+
 
 # About
 
 NextGuild is a Guilded API wrapper written in Python.
 
 Planning on being the most simplest python library interacting with the Guilded API, Nextguild is planning to be beginner-friendly and be a great resource to learn Python programming, this is a library, with easy configuration.
 
 Made from a team of 2 people, this was a simple project originally thought for a fun purpose and for testing the Guilded API, which eventually turned into a bot library for multi-purpose use.
 
-
-# Development
-
-Currently, NextGuild is not at a stable version and it is not recommended to use the package until a stable version is released.
 ## Installation
 
 Use the Python Package Index package manager [pip](https://pip.pypa.io/en/stable/) to install NextGuild to start using this package for your project.
 
 ```bash
 pip install nextguild
 ```
```

### Comparing `nextguild-1.0.5/nextguild.egg-info/PKG-INFO` & `nextguild-1.1/nextguild.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nextguild
-Version: 1.0.5
+Version: 1.1
 Summary: Interactions with the Guilded API made simpler
 Author-email: Arjun Sharda <sharda.aj17@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Arjun Sharda
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -31,28 +31,27 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # NextGuild
-![image](https://user-images.githubusercontent.com/77706434/225704407-da247647-9c9f-4115-a2f1-93d567f46ea7.png)
+![image](https://user-images.githubusercontent.com/108808053/235311374-bdcdcdac-3c04-4b86-b336-1d2a02f5e914.png)
+
+
+
 
 # About
 
 NextGuild is a Guilded API wrapper written in Python.
 
 Planning on being the most simplest python library interacting with the Guilded API, Nextguild is planning to be beginner-friendly and be a great resource to learn Python programming, this is a library, with easy configuration.
 
 Made from a team of 2 people, this was a simple project originally thought for a fun purpose and for testing the Guilded API, which eventually turned into a bot library for multi-purpose use.
 
-
-# Development
-
-Currently, NextGuild is not at a stable version and it is not recommended to use the package until a stable version is released.
 ## Installation
 
 Use the Python Package Index package manager [pip](https://pip.pypa.io/en/stable/) to install NextGuild to start using this package for your project.
 
 ```bash
 pip install nextguild
 ```
```

### Comparing `nextguild-1.0.5/pyproject.toml` & `nextguild-1.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "requests", "asyncio", "websockets"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nextguild"
-version = "1.0.5"
+version = "1.1"
 authors = [
     { name="Arjun Sharda", email="sharda.aj17@gmail.com" },
 ]
 description = "Interactions with the Guilded API made simpler"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
```

