# Comparing `tmp/jiggybase-0.0.18.tar.gz` & `tmp/jiggybase-0.0.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jiggybase-0.0.18.tar", last modified: Sun Apr 30 01:07:28 2023, max compression
+gzip compressed data, was "jiggybase-0.0.19.tar", last modified: Mon May  1 01:50:45 2023, max compression
```

## Comparing `jiggybase-0.0.18.tar` & `jiggybase-0.0.19.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-04-30 01:07:28.806875 jiggybase-0.0.18/
--rw-r--r--   0 wsk        (501) staff       (20)    11357 2023-04-10 04:07:02.000000 jiggybase-0.0.18/LICENSE
--rw-r--r--   0 wsk        (501) staff       (20)      533 2023-04-30 01:07:28.806461 jiggybase-0.0.18/PKG-INFO
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-04-30 01:07:28.800026 jiggybase-0.0.18/jiggybase/
--rw-r--r--   0 wsk        (501) staff       (20)       30 2023-04-28 15:28:30.000000 jiggybase-0.0.18/jiggybase/__init__.py
--rw-r--r--   0 wsk        (501) staff       (20)     1769 2023-04-28 15:29:35.000000 jiggybase-0.0.18/jiggybase/client.py
--rw-r--r--   0 wsk        (501) staff       (20)     8508 2023-04-30 00:50:55.000000 jiggybase-0.0.18/jiggybase/collection.py
--rw-r--r--   0 wsk        (501) staff       (20)     2726 2023-04-05 03:30:00.000000 jiggybase-0.0.18/jiggybase/config.py
--rw-r--r--   0 wsk        (501) staff       (20)     4531 2023-04-29 04:12:14.000000 jiggybase-0.0.18/jiggybase/jiggybase_session.py
--rw-r--r--   0 wsk        (501) staff       (20)     1187 2023-03-30 18:09:13.000000 jiggybase-0.0.18/jiggybase/login.py
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-04-30 01:07:28.805604 jiggybase-0.0.18/jiggybase/models/
--rw-r--r--   0 wsk        (501) staff       (20)      273 2023-04-26 01:37:49.000000 jiggybase-0.0.18/jiggybase/models/__init__.py
--rw-r--r--   0 wsk        (501) staff       (20)     1236 2023-04-10 05:17:32.000000 jiggybase-0.0.18/jiggybase/models/auth.py
--rw-r--r--   0 wsk        (501) staff       (20)     1007 2023-04-23 16:10:39.000000 jiggybase-0.0.18/jiggybase/models/chat.py
--rw-r--r--   0 wsk        (501) staff       (20)      188 2023-04-23 04:17:06.000000 jiggybase-0.0.18/jiggybase/models/chatmodel.py
--rw-r--r--   0 wsk        (501) staff       (20)     1322 2023-04-10 16:54:34.000000 jiggybase-0.0.18/jiggybase/models/chunk.py
--rw-r--r--   0 wsk        (501) staff       (20)     4240 2023-04-20 21:45:37.000000 jiggybase-0.0.18/jiggybase/models/collection.py
--rw-r--r--   0 wsk        (501) staff       (20)      454 2023-04-23 05:06:00.000000 jiggybase-0.0.18/jiggybase/models/embedding.py
--rw-r--r--   0 wsk        (501) staff       (20)      696 2023-04-10 04:48:20.000000 jiggybase-0.0.18/jiggybase/models/metadata.py
--rw-r--r--   0 wsk        (501) staff       (20)     2214 2023-04-10 04:58:39.000000 jiggybase-0.0.18/jiggybase/models/org.py
--rw-r--r--   0 wsk        (501) staff       (20)     2777 2023-04-29 00:07:44.000000 jiggybase-0.0.18/jiggybase/models/plugin.py
--rw-r--r--   0 wsk        (501) staff       (20)     3452 2023-04-10 19:09:18.000000 jiggybase-0.0.18/jiggybase/models/plugin_config.py
--rw-r--r--   0 wsk        (501) staff       (20)     2834 2023-04-22 23:44:02.000000 jiggybase-0.0.18/jiggybase/models/prompt.py
--rw-r--r--   0 wsk        (501) staff       (20)     3012 2023-04-11 17:29:49.000000 jiggybase-0.0.18/jiggybase/models/providers.py
--rw-r--r--   0 wsk        (501) staff       (20)     1820 2023-04-17 16:14:19.000000 jiggybase-0.0.18/jiggybase/models/user.py
--rw-r--r--   0 wsk        (501) staff       (20)     4600 2023-04-29 15:22:54.000000 jiggybase-0.0.18/jiggybase/org.py
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-04-30 01:07:28.801386 jiggybase-0.0.18/jiggybase.egg-info/
--rw-r--r--   0 wsk        (501) staff       (20)      533 2023-04-30 01:07:28.000000 jiggybase-0.0.18/jiggybase.egg-info/PKG-INFO
--rw-r--r--   0 wsk        (501) staff       (20)      744 2023-04-30 01:07:28.000000 jiggybase-0.0.18/jiggybase.egg-info/SOURCES.txt
--rw-r--r--   0 wsk        (501) staff       (20)        1 2023-04-30 01:07:28.000000 jiggybase-0.0.18/jiggybase.egg-info/dependency_links.txt
--rw-r--r--   0 wsk        (501) staff       (20)       32 2023-04-30 01:07:28.000000 jiggybase-0.0.18/jiggybase.egg-info/requires.txt
--rw-r--r--   0 wsk        (501) staff       (20)       10 2023-04-30 01:07:28.000000 jiggybase-0.0.18/jiggybase.egg-info/top_level.txt
--rw-r--r--   0 wsk        (501) staff       (20)      669 2023-04-30 01:06:52.000000 jiggybase-0.0.18/pyproject.toml
--rw-r--r--   0 wsk        (501) staff       (20)       38 2023-04-30 01:07:28.806991 jiggybase-0.0.18/setup.cfg
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-04-30 01:07:28.805947 jiggybase-0.0.18/test/
--rw-r--r--   0 wsk        (501) staff       (20)      830 2023-04-28 15:38:35.000000 jiggybase-0.0.18/test/test.py
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-01 01:50:45.747926 jiggybase-0.0.19/
+-rw-r--r--   0 wsk        (501) staff       (20)    11357 2023-04-10 04:07:02.000000 jiggybase-0.0.19/LICENSE
+-rw-r--r--   0 wsk        (501) staff       (20)     4606 2023-05-01 01:50:45.747506 jiggybase-0.0.19/PKG-INFO
+-rw-r--r--   0 wsk        (501) staff       (20)     4071 2023-05-01 01:37:56.000000 jiggybase-0.0.19/README.md
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-01 01:50:45.740284 jiggybase-0.0.19/jiggybase/
+-rw-r--r--   0 wsk        (501) staff       (20)       30 2023-04-28 15:28:30.000000 jiggybase-0.0.19/jiggybase/__init__.py
+-rw-r--r--   0 wsk        (501) staff       (20)     2044 2023-05-01 01:40:42.000000 jiggybase-0.0.19/jiggybase/client.py
+-rw-r--r--   0 wsk        (501) staff       (20)     8508 2023-04-30 00:50:55.000000 jiggybase-0.0.19/jiggybase/collection.py
+-rw-r--r--   0 wsk        (501) staff       (20)     4531 2023-04-29 04:12:14.000000 jiggybase-0.0.19/jiggybase/jiggybase_session.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1187 2023-03-30 18:09:13.000000 jiggybase-0.0.19/jiggybase/login.py
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-01 01:50:45.746436 jiggybase-0.0.19/jiggybase/models/
+-rw-r--r--   0 wsk        (501) staff       (20)      273 2023-04-26 01:37:49.000000 jiggybase-0.0.19/jiggybase/models/__init__.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1236 2023-04-10 05:17:32.000000 jiggybase-0.0.19/jiggybase/models/auth.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1007 2023-04-23 16:10:39.000000 jiggybase-0.0.19/jiggybase/models/chat.py
+-rw-r--r--   0 wsk        (501) staff       (20)      188 2023-04-23 04:17:06.000000 jiggybase-0.0.19/jiggybase/models/chatmodel.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1322 2023-04-10 16:54:34.000000 jiggybase-0.0.19/jiggybase/models/chunk.py
+-rw-r--r--   0 wsk        (501) staff       (20)     4240 2023-04-20 21:45:37.000000 jiggybase-0.0.19/jiggybase/models/collection.py
+-rw-r--r--   0 wsk        (501) staff       (20)      454 2023-04-23 05:06:00.000000 jiggybase-0.0.19/jiggybase/models/embedding.py
+-rw-r--r--   0 wsk        (501) staff       (20)      696 2023-04-10 04:48:20.000000 jiggybase-0.0.19/jiggybase/models/metadata.py
+-rw-r--r--   0 wsk        (501) staff       (20)     2214 2023-04-10 04:58:39.000000 jiggybase-0.0.19/jiggybase/models/org.py
+-rw-r--r--   0 wsk        (501) staff       (20)     2777 2023-04-29 00:07:44.000000 jiggybase-0.0.19/jiggybase/models/plugin.py
+-rw-r--r--   0 wsk        (501) staff       (20)     3452 2023-04-10 19:09:18.000000 jiggybase-0.0.19/jiggybase/models/plugin_config.py
+-rw-r--r--   0 wsk        (501) staff       (20)     2834 2023-04-22 23:44:02.000000 jiggybase-0.0.19/jiggybase/models/prompt.py
+-rw-r--r--   0 wsk        (501) staff       (20)     3012 2023-04-11 17:29:49.000000 jiggybase-0.0.19/jiggybase/models/providers.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1820 2023-04-17 16:14:19.000000 jiggybase-0.0.19/jiggybase/models/user.py
+-rw-r--r--   0 wsk        (501) staff       (20)     4600 2023-04-29 15:22:54.000000 jiggybase-0.0.19/jiggybase/org.py
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-01 01:50:45.741782 jiggybase-0.0.19/jiggybase.egg-info/
+-rw-r--r--   0 wsk        (501) staff       (20)     4606 2023-05-01 01:50:45.000000 jiggybase-0.0.19/jiggybase.egg-info/PKG-INFO
+-rw-r--r--   0 wsk        (501) staff       (20)      734 2023-05-01 01:50:45.000000 jiggybase-0.0.19/jiggybase.egg-info/SOURCES.txt
+-rw-r--r--   0 wsk        (501) staff       (20)        1 2023-05-01 01:50:45.000000 jiggybase-0.0.19/jiggybase.egg-info/dependency_links.txt
+-rw-r--r--   0 wsk        (501) staff       (20)       32 2023-05-01 01:50:45.000000 jiggybase-0.0.19/jiggybase.egg-info/requires.txt
+-rw-r--r--   0 wsk        (501) staff       (20)       10 2023-05-01 01:50:45.000000 jiggybase-0.0.19/jiggybase.egg-info/top_level.txt
+-rw-r--r--   0 wsk        (501) staff       (20)      669 2023-05-01 01:38:08.000000 jiggybase-0.0.19/pyproject.toml
+-rw-r--r--   0 wsk        (501) staff       (20)       38 2023-05-01 01:50:45.748054 jiggybase-0.0.19/setup.cfg
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-01 01:50:45.746913 jiggybase-0.0.19/test/
+-rw-r--r--   0 wsk        (501) staff       (20)      830 2023-04-28 15:38:35.000000 jiggybase-0.0.19/test/test.py
```

### Comparing `jiggybase-0.0.18/LICENSE` & `jiggybase-0.0.19/LICENSE`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.18/jiggybase/client.py` & `jiggybase-0.0.19/jiggybase/client.py`

 * *Files 14% similar despite different names*

```diff
@@ -55,7 +55,14 @@
         return all Collections in all Orgs that the user is a member of
         """
         collections = []
         for org in self.orgs():
             for collection in org.collections():
                 collections.append(collection)
         return collections
+
+    def collection(self, name : str) -> Collection:
+        for org in self.orgs():
+            for collection in org.collections():
+                if collection.name == name:
+                    return collection
+        raise ValueError(f'Collection "{name}" not found')
```

### Comparing `jiggybase-0.0.18/jiggybase/collection.py` & `jiggybase-0.0.19/jiggybase/collection.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.18/jiggybase/jiggybase_session.py` & `jiggybase-0.0.19/jiggybase/jiggybase_session.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.18/jiggybase/login.py` & `jiggybase-0.0.19/jiggybase/login.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.18/jiggybase/models/auth.py` & `jiggybase-0.0.19/jiggybase/models/auth.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.18/jiggybase/models/chat.py` & `jiggybase-0.0.19/jiggybase/models/chat.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.18/jiggybase/models/chunk.py` & `jiggybase-0.0.19/jiggybase/models/chunk.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.18/jiggybase/models/collection.py` & `jiggybase-0.0.19/jiggybase/models/collection.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.18/jiggybase/models/metadata.py` & `jiggybase-0.0.19/jiggybase/models/metadata.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.18/jiggybase/models/org.py` & `jiggybase-0.0.19/jiggybase/models/org.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.18/jiggybase/models/plugin.py` & `jiggybase-0.0.19/jiggybase/models/plugin.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.18/jiggybase/models/plugin_config.py` & `jiggybase-0.0.19/jiggybase/models/plugin_config.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.18/jiggybase/models/prompt.py` & `jiggybase-0.0.19/jiggybase/models/prompt.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.18/jiggybase/models/providers.py` & `jiggybase-0.0.19/jiggybase/models/providers.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.18/jiggybase/models/user.py` & `jiggybase-0.0.19/jiggybase/models/user.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.18/jiggybase/org.py` & `jiggybase-0.0.19/jiggybase/org.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.18/jiggybase.egg-info/SOURCES.txt` & `jiggybase-0.0.19/jiggybase.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 LICENSE
+README.md
 pyproject.toml
 jiggybase/__init__.py
 jiggybase/client.py
 jiggybase/collection.py
-jiggybase/config.py
 jiggybase/jiggybase_session.py
 jiggybase/login.py
 jiggybase/org.py
 jiggybase.egg-info/PKG-INFO
 jiggybase.egg-info/SOURCES.txt
 jiggybase.egg-info/dependency_links.txt
 jiggybase.egg-info/requires.txt
```

### Comparing `jiggybase-0.0.18/pyproject.toml` & `jiggybase-0.0.19/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "jiggybase"
-version = "0.0.18"
+version = "0.0.19"
 authors = [
   { name="Bill Kish", email="bk@jiggy.ai" },
 ]
 dependencies=['loguru', 'pedantic[email]', 'requests']
 description = "Client for Jiggy AI JiggyBase, including ChatGPT Retriever Plugins"
 readme = "README.md"
 requires-python = ">=3.9"
```

### Comparing `jiggybase-0.0.18/test/test.py` & `jiggybase-0.0.19/test/test.py`

 * *Files identical despite different names*

