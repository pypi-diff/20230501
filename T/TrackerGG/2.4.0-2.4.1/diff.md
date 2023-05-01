# Comparing `tmp/TrackerGG-2.4.0.tar.gz` & `tmp/TrackerGG-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TrackerGG-2.4.0.tar", last modified: Mon May  1 02:09:58 2023, max compression
+gzip compressed data, was "TrackerGG-2.4.1.tar", last modified: Mon May  1 11:10:56 2023, max compression
```

## Comparing `TrackerGG-2.4.0.tar` & `TrackerGG-2.4.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 02:09:58.745123 TrackerGG-2.4.0/
--rw-rw-rw-   0        0        0     1085 2023-04-21 13:43:24.000000 TrackerGG-2.4.0/LICENSE
--rw-rw-rw-   0        0        0     1425 2023-05-01 02:09:58.736846 TrackerGG-2.4.0/PKG-INFO
--rw-rw-rw-   0        0        0     1042 2023-04-21 13:43:24.000000 TrackerGG-2.4.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-01 02:09:58.720262 TrackerGG-2.4.0/TrackerGG/
-drwxrwxrwx   0        0        0        0 2023-05-01 02:09:58.734848 TrackerGG-2.4.0/TrackerGG/Models/
--rw-rw-rw-   0        0        0      753 2023-05-01 01:41:24.000000 TrackerGG-2.4.0/TrackerGG/Models/__init__.py
--rw-rw-rw-   0        0        0     5759 2023-05-01 02:04:17.000000 TrackerGG-2.4.0/TrackerGG/Models/csgo.py
--rw-rw-rw-   0        0        0     1477 2023-04-21 13:43:24.000000 TrackerGG-2.4.0/TrackerGG/Models/platform.py
--rw-rw-rw-   0        0        0     1399 2023-04-21 13:43:24.000000 TrackerGG-2.4.0/TrackerGG/Models/segment.py
--rw-rw-rw-   0        0        0     2059 2023-04-21 13:43:24.000000 TrackerGG-2.4.0/TrackerGG/Models/user.py
--rw-rw-rw-   0        0        0      903 2023-05-01 01:41:24.000000 TrackerGG-2.4.0/TrackerGG/__init__.py
--rw-rw-rw-   0        0        0     3997 2023-05-01 01:05:59.000000 TrackerGG-2.4.0/TrackerGG/client.py
--rw-rw-rw-   0        0        0     3531 2023-04-21 13:43:24.000000 TrackerGG-2.4.0/TrackerGG/httpclient.py
--rw-rw-rw-   0        0        0     1143 2023-05-01 02:04:20.000000 TrackerGG-2.4.0/TrackerGG/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-01 02:09:58.726390 TrackerGG-2.4.0/TrackerGG.egg-info/
--rw-rw-rw-   0        0        0     1425 2023-05-01 02:09:58.000000 TrackerGG-2.4.0/TrackerGG.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      411 2023-05-01 02:09:58.000000 TrackerGG-2.4.0/TrackerGG.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 02:09:58.000000 TrackerGG-2.4.0/TrackerGG.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-05-01 02:09:58.000000 TrackerGG-2.4.0/TrackerGG.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-01 02:09:58.000000 TrackerGG-2.4.0/TrackerGG.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-01 02:09:58.746118 TrackerGG-2.4.0/setup.cfg
--rw-rw-rw-   0        0        0      655 2023-05-01 02:08:49.000000 TrackerGG-2.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 11:10:56.047335 TrackerGG-2.4.1/
+-rw-rw-rw-   0        0        0     1085 2023-04-21 13:43:24.000000 TrackerGG-2.4.1/LICENSE
+-rw-rw-rw-   0        0        0     1425 2023-05-01 11:10:56.039583 TrackerGG-2.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1042 2023-04-21 13:43:24.000000 TrackerGG-2.4.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-01 11:10:56.025067 TrackerGG-2.4.1/TrackerGG/
+drwxrwxrwx   0        0        0        0 2023-05-01 11:10:56.038586 TrackerGG-2.4.1/TrackerGG/Models/
+-rw-rw-rw-   0        0        0      753 2023-05-01 02:11:36.000000 TrackerGG-2.4.1/TrackerGG/Models/__init__.py
+-rw-rw-rw-   0        0        0     5759 2023-05-01 02:04:17.000000 TrackerGG-2.4.1/TrackerGG/Models/csgo.py
+-rw-rw-rw-   0        0        0     1477 2023-04-21 13:43:24.000000 TrackerGG-2.4.1/TrackerGG/Models/platform.py
+-rw-rw-rw-   0        0        0     1399 2023-04-21 13:43:24.000000 TrackerGG-2.4.1/TrackerGG/Models/segment.py
+-rw-rw-rw-   0        0        0     2059 2023-04-21 13:43:24.000000 TrackerGG-2.4.1/TrackerGG/Models/user.py
+-rw-rw-rw-   0        0        0      903 2023-05-01 02:11:19.000000 TrackerGG-2.4.1/TrackerGG/__init__.py
+-rw-rw-rw-   0        0        0     5390 2023-05-01 11:04:08.000000 TrackerGG-2.4.1/TrackerGG/client.py
+-rw-rw-rw-   0        0        0     3531 2023-04-21 13:43:24.000000 TrackerGG-2.4.1/TrackerGG/httpclient.py
+-rw-rw-rw-   0        0        0     1693 2023-05-01 10:58:10.000000 TrackerGG-2.4.1/TrackerGG/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-01 11:10:56.032582 TrackerGG-2.4.1/TrackerGG.egg-info/
+-rw-rw-rw-   0        0        0     1425 2023-05-01 11:10:55.000000 TrackerGG-2.4.1/TrackerGG.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      411 2023-05-01 11:10:55.000000 TrackerGG-2.4.1/TrackerGG.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 11:10:55.000000 TrackerGG-2.4.1/TrackerGG.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-05-01 11:10:55.000000 TrackerGG-2.4.1/TrackerGG.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-01 11:10:55.000000 TrackerGG-2.4.1/TrackerGG.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-01 11:10:56.047841 TrackerGG-2.4.1/setup.cfg
+-rw-rw-rw-   0        0        0      655 2023-05-01 11:10:13.000000 TrackerGG-2.4.1/setup.py
```

### Comparing `TrackerGG-2.4.0/LICENSE` & `TrackerGG-2.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `TrackerGG-2.4.0/PKG-INFO` & `TrackerGG-2.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TrackerGG
-Version: 2.4.0
+Version: 2.4.1
 Summary: TrackerGG API Wrapper Library
 Home-page: https://github.com/dev-ruby/TrackerGG
 Author: DevRuby
 Author-email: hiveruby@gmail.com
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.3
```

### Comparing `TrackerGG-2.4.0/README.md` & `TrackerGG-2.4.1/README.md`

 * *Files identical despite different names*

### Comparing `TrackerGG-2.4.0/TrackerGG/Models/__init__.py` & `TrackerGG-2.4.1/TrackerGG/Models/__init__.py`

 * *Files identical despite different names*

### Comparing `TrackerGG-2.4.0/TrackerGG/Models/csgo.py` & `TrackerGG-2.4.1/TrackerGG/Models/csgo.py`

 * *Files identical despite different names*

### Comparing `TrackerGG-2.4.0/TrackerGG/Models/platform.py` & `TrackerGG-2.4.1/TrackerGG/Models/platform.py`

 * *Files identical despite different names*

### Comparing `TrackerGG-2.4.0/TrackerGG/Models/segment.py` & `TrackerGG-2.4.1/TrackerGG/Models/segment.py`

 * *Files identical despite different names*

### Comparing `TrackerGG-2.4.0/TrackerGG/Models/user.py` & `TrackerGG-2.4.1/TrackerGG/Models/user.py`

 * *Files identical despite different names*

### Comparing `TrackerGG-2.4.0/TrackerGG/__init__.py` & `TrackerGG-2.4.1/TrackerGG/__init__.py`

 * *Files identical despite different names*

### Comparing `TrackerGG-2.4.0/TrackerGG/httpclient.py` & `TrackerGG-2.4.1/TrackerGG/httpclient.py`

 * *Files identical despite different names*

### Comparing `TrackerGG-2.4.0/TrackerGG/utils.py` & `TrackerGG-2.4.1/TrackerGG/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -21,20 +21,36 @@
 from .Models import CSGOWeapon
 from typing import List, Union
 
 
 def query_map_by_key(
     maps: List[CSGOMapSegment], key: str
 ) -> Union[CSGOMapSegment, int]:
+    """
+    Returns CSGOMapSegment that matches key
+    Returns -1 if there is no matching CSGOMapSegment Object
+
+    :param maps: List[:class:`CSGOMapSegment`]
+    :param key: :class:`str`
+    :return: Union[:class:`CSGOMapSegment`, :class:`int`]
+    """
     for _map in maps:
         if _map.attributes["key"] == key:
             return _map
     return -1
 
 
 def query_weapon(
     weapons: List[CSGOWeaponSegment], key: CSGOWeapon
 ) -> Union[CSGOWeaponSegment, int]:
+    """
+    Returns CSGOWeaponSegment that matches key
+    Returns -1 if there is no matching CSGOWeaponSegment Object
+
+    :param weapons: List[:class:`CSGOWeaponSegment`]
+    :param key: :class:`CSGOWeapon`
+    :return: Union[:class:`CSGOWeaponSegment`, :class:`int`]
+    """
     for _weapon in weapons:
         if _weapon.attributes["key"] == key.value:
             return _weapon
     return -1
```

### Comparing `TrackerGG-2.4.0/TrackerGG.egg-info/PKG-INFO` & `TrackerGG-2.4.1/TrackerGG.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TrackerGG
-Version: 2.4.0
+Version: 2.4.1
 Summary: TrackerGG API Wrapper Library
 Home-page: https://github.com/dev-ruby/TrackerGG
 Author: DevRuby
 Author-email: hiveruby@gmail.com
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.3
```

### Comparing `TrackerGG-2.4.0/setup.py` & `TrackerGG-2.4.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fs:
     long_description = fs.read()
 
 setuptools.setup(
     name="TrackerGG",
-    version="2.4.0",
+    version="2.4.1",
     author="DevRuby",
     author_email="hiveruby@gmail.com",
     description="TrackerGG API Wrapper Library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/dev-ruby/TrackerGG",
     packages=setuptools.find_packages(),
```

