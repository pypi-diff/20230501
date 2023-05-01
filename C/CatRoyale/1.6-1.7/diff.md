# Comparing `tmp/CatRoyale-1.6.tar.gz` & `tmp/CatRoyale-1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CatRoyale-1.6.tar", last modified: Mon May  1 11:05:39 2023, max compression
+gzip compressed data, was "CatRoyale-1.7.tar", last modified: Mon May  1 11:08:50 2023, max compression
```

## Comparing `CatRoyale-1.6.tar` & `CatRoyale-1.7.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 11:05:39.338607 CatRoyale-1.6/
-drwxrwxrwx   0        0        0        0 2023-05-01 11:05:39.278610 CatRoyale-1.6/CatRoyale.egg-info/
--rw-rw-rw-   0        0        0      222 2023-05-01 11:05:39.000000 CatRoyale-1.6/CatRoyale.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      858 2023-05-01 11:05:39.000000 CatRoyale-1.6/CatRoyale.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 11:05:39.000000 CatRoyale-1.6/CatRoyale.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2023-05-01 11:05:39.000000 CatRoyale-1.6/CatRoyale.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-05-01 11:05:39.000000 CatRoyale-1.6/CatRoyale.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       78 2023-05-01 11:05:27.000000 CatRoyale-1.6/MANIFEST.in
--rw-rw-rw-   0        0        0      222 2023-05-01 11:05:39.337607 CatRoyale-1.6/PKG-INFO
--rw-rw-rw-   0        0        0      107 2023-05-01 10:48:10.000000 CatRoyale-1.6/README.md
-drwxrwxrwx   0        0        0        0 2023-05-01 11:05:39.281605 CatRoyale-1.6/assets/
--rw-rw-rw-   0        0        0        0 2023-05-01 10:54:38.000000 CatRoyale-1.6/assets/__init__.py
--rw-rw-rw-   0        0        0      528 2023-04-23 11:35:23.000000 CatRoyale-1.6/assets/image_locations.json
-drwxrwxrwx   0        0        0        0 2023-05-01 11:05:39.312610 CatRoyale-1.6/assets/images/
--rw-rw-rw-   0        0        0      455 2023-03-25 12:46:51.000000 CatRoyale-1.6/assets/images/Inventory_Bar.png
--rw-rw-rw-   0        0        0      212 2023-03-25 12:46:51.000000 CatRoyale-1.6/assets/images/Inventory_Slot.png
--rw-rw-rw-   0        0        0      214 2023-03-25 12:46:51.000000 CatRoyale-1.6/assets/images/Inventory_select.png
--rw-rw-rw-   0        0        0      498 2023-04-24 15:22:32.000000 CatRoyale-1.6/assets/images/arrow.png
--rw-rw-rw-   0        0        0    12841 2023-03-25 16:24:31.000000 CatRoyale-1.6/assets/images/cat.png
--rw-rw-rw-   0        0        0    27199 2023-04-22 14:53:45.000000 CatRoyale-1.6/assets/images/enemy_cat.png
--rw-rw-rw-   0        0        0     2170 2023-03-22 21:48:06.000000 CatRoyale-1.6/assets/images/grass.png
--rw-rw-rw-   0        0        0   127269 2023-03-22 20:35:26.000000 CatRoyale-1.6/assets/images/items.png
--rw-rw-rw-   0        0        0    19155 2023-03-28 16:20:17.000000 CatRoyale-1.6/assets/images/loading_screen.png
-drwxrwxrwx   0        0        0        0 2023-05-01 11:05:39.314608 CatRoyale-1.6/assets/images/map/
--rw-rw-rw-   0        0        0     2795 2023-04-26 18:20:17.000000 CatRoyale-1.6/assets/images/map/level00.png
-drwxrwxrwx   0        0        0        0 2023-05-01 11:05:39.333611 CatRoyale-1.6/classes/
--rw-rw-rw-   0        0        0        0 2023-04-22 13:48:02.000000 CatRoyale-1.6/classes/__init__.py
--rw-rw-rw-   0        0        0     5339 2023-05-01 10:16:04.000000 CatRoyale-1.6/classes/box.py
--rw-rw-rw-   0        0        0    24994 2023-05-01 10:34:53.000000 CatRoyale-1.6/classes/character.py
--rw-rw-rw-   0        0        0      996 2023-05-01 10:31:13.000000 CatRoyale-1.6/classes/config.py
--rw-rw-rw-   0        0        0     2077 2023-05-01 10:14:35.000000 CatRoyale-1.6/classes/event_stack.py
--rw-rw-rw-   0        0        0     1054 2023-05-01 10:23:12.000000 CatRoyale-1.6/classes/functions.py
--rw-rw-rw-   0        0        0     3741 2023-05-01 10:26:03.000000 CatRoyale-1.6/classes/game_map.py
--rw-rw-rw-   0        0        0     2193 2023-05-01 08:26:56.000000 CatRoyale-1.6/classes/health_bars.py
--rw-rw-rw-   0        0        0    14266 2023-05-01 10:27:16.000000 CatRoyale-1.6/classes/inventory.py
--rw-rw-rw-   0        0        0     4440 2023-05-01 10:05:02.000000 CatRoyale-1.6/classes/item.py
--rw-rw-rw-   0        0        0      521 2023-05-01 10:06:08.000000 CatRoyale-1.6/classes/map_reader.py
--rw-rw-rw-   0        0        0      362 2023-05-01 10:10:10.000000 CatRoyale-1.6/classes/message_service.py
--rw-rw-rw-   0        0        0     1718 2023-04-30 19:32:21.000000 CatRoyale-1.6/classes/text_display.py
-drwxrwxrwx   0        0        0        0 2023-05-01 11:05:39.335609 CatRoyale-1.6/config/
--rw-rw-rw-   0        0        0        0 2023-05-01 11:05:20.000000 CatRoyale-1.6/config/__init__.py
--rw-rw-rw-   0        0        0     2684 2023-04-30 19:34:37.000000 CatRoyale-1.6/config/config.json
--rw-rw-rw-   0        0        0    15824 2023-05-01 10:34:59.000000 CatRoyale-1.6/main.py
--rw-rw-rw-   0        0        0       88 2023-05-01 10:53:12.000000 CatRoyale-1.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-01 11:05:39.338607 CatRoyale-1.6/setup.cfg
--rw-rw-rw-   0        0        0      440 2023-05-01 11:04:28.000000 CatRoyale-1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 11:08:50.033003 CatRoyale-1.7/
+drwxrwxrwx   0        0        0        0 2023-05-01 11:08:49.868003 CatRoyale-1.7/CatRoyale.egg-info/
+-rw-rw-rw-   0        0        0      222 2023-05-01 11:08:49.000000 CatRoyale-1.7/CatRoyale.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      858 2023-05-01 11:08:49.000000 CatRoyale-1.7/CatRoyale.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 11:08:49.000000 CatRoyale-1.7/CatRoyale.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-05-01 11:08:49.000000 CatRoyale-1.7/CatRoyale.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2023-05-01 11:08:49.000000 CatRoyale-1.7/CatRoyale.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       78 2023-05-01 11:05:27.000000 CatRoyale-1.7/MANIFEST.in
+-rw-rw-rw-   0        0        0      222 2023-05-01 11:08:50.032001 CatRoyale-1.7/PKG-INFO
+-rw-rw-rw-   0        0        0      107 2023-05-01 10:48:10.000000 CatRoyale-1.7/README.md
+drwxrwxrwx   0        0        0        0 2023-05-01 11:08:49.870003 CatRoyale-1.7/assets/
+-rw-rw-rw-   0        0        0        0 2023-05-01 10:54:38.000000 CatRoyale-1.7/assets/__init__.py
+-rw-rw-rw-   0        0        0      528 2023-04-23 11:35:23.000000 CatRoyale-1.7/assets/image_locations.json
+drwxrwxrwx   0        0        0        0 2023-05-01 11:08:50.010002 CatRoyale-1.7/assets/images/
+-rw-rw-rw-   0        0        0      455 2023-03-25 12:46:51.000000 CatRoyale-1.7/assets/images/Inventory_Bar.png
+-rw-rw-rw-   0        0        0      212 2023-03-25 12:46:51.000000 CatRoyale-1.7/assets/images/Inventory_Slot.png
+-rw-rw-rw-   0        0        0      214 2023-03-25 12:46:51.000000 CatRoyale-1.7/assets/images/Inventory_select.png
+-rw-rw-rw-   0        0        0      498 2023-04-24 15:22:32.000000 CatRoyale-1.7/assets/images/arrow.png
+-rw-rw-rw-   0        0        0    12841 2023-03-25 16:24:31.000000 CatRoyale-1.7/assets/images/cat.png
+-rw-rw-rw-   0        0        0    27199 2023-04-22 14:53:45.000000 CatRoyale-1.7/assets/images/enemy_cat.png
+-rw-rw-rw-   0        0        0     2170 2023-03-22 21:48:06.000000 CatRoyale-1.7/assets/images/grass.png
+-rw-rw-rw-   0        0        0   127269 2023-03-22 20:35:26.000000 CatRoyale-1.7/assets/images/items.png
+-rw-rw-rw-   0        0        0    19155 2023-03-28 16:20:17.000000 CatRoyale-1.7/assets/images/loading_screen.png
+drwxrwxrwx   0        0        0        0 2023-05-01 11:08:50.011006 CatRoyale-1.7/assets/images/map/
+-rw-rw-rw-   0        0        0     2795 2023-04-26 18:20:17.000000 CatRoyale-1.7/assets/images/map/level00.png
+drwxrwxrwx   0        0        0        0 2023-05-01 11:08:50.029002 CatRoyale-1.7/classes/
+-rw-rw-rw-   0        0        0        0 2023-04-22 13:48:02.000000 CatRoyale-1.7/classes/__init__.py
+-rw-rw-rw-   0        0        0     5339 2023-05-01 10:16:04.000000 CatRoyale-1.7/classes/box.py
+-rw-rw-rw-   0        0        0    24994 2023-05-01 10:34:53.000000 CatRoyale-1.7/classes/character.py
+-rw-rw-rw-   0        0        0      996 2023-05-01 10:31:13.000000 CatRoyale-1.7/classes/config.py
+-rw-rw-rw-   0        0        0     2077 2023-05-01 10:14:35.000000 CatRoyale-1.7/classes/event_stack.py
+-rw-rw-rw-   0        0        0     1054 2023-05-01 10:23:12.000000 CatRoyale-1.7/classes/functions.py
+-rw-rw-rw-   0        0        0     3741 2023-05-01 10:26:03.000000 CatRoyale-1.7/classes/game_map.py
+-rw-rw-rw-   0        0        0     2193 2023-05-01 08:26:56.000000 CatRoyale-1.7/classes/health_bars.py
+-rw-rw-rw-   0        0        0    14266 2023-05-01 10:27:16.000000 CatRoyale-1.7/classes/inventory.py
+-rw-rw-rw-   0        0        0     4440 2023-05-01 10:05:02.000000 CatRoyale-1.7/classes/item.py
+-rw-rw-rw-   0        0        0      521 2023-05-01 10:06:08.000000 CatRoyale-1.7/classes/map_reader.py
+-rw-rw-rw-   0        0        0      362 2023-05-01 10:10:10.000000 CatRoyale-1.7/classes/message_service.py
+-rw-rw-rw-   0        0        0     1718 2023-04-30 19:32:21.000000 CatRoyale-1.7/classes/text_display.py
+drwxrwxrwx   0        0        0        0 2023-05-01 11:08:50.031007 CatRoyale-1.7/config/
+-rw-rw-rw-   0        0        0        0 2023-05-01 11:05:20.000000 CatRoyale-1.7/config/__init__.py
+-rw-rw-rw-   0        0        0     2684 2023-04-30 19:34:37.000000 CatRoyale-1.7/config/config.json
+-rw-rw-rw-   0        0        0    15824 2023-05-01 10:34:59.000000 CatRoyale-1.7/main.py
+-rw-rw-rw-   0        0        0       88 2023-05-01 10:53:12.000000 CatRoyale-1.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-01 11:08:50.034008 CatRoyale-1.7/setup.cfg
+-rw-rw-rw-   0        0        0      453 2023-05-01 11:08:42.000000 CatRoyale-1.7/setup.py
```

### Comparing `CatRoyale-1.6/CatRoyale.egg-info/SOURCES.txt` & `CatRoyale-1.7/CatRoyale.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `CatRoyale-1.6/assets/image_locations.json` & `CatRoyale-1.7/assets/image_locations.json`

 * *Files identical despite different names*

### Comparing `CatRoyale-1.6/assets/images/cat.png` & `CatRoyale-1.7/assets/images/cat.png`

 * *Files identical despite different names*

### Comparing `CatRoyale-1.6/assets/images/enemy_cat.png` & `CatRoyale-1.7/assets/images/enemy_cat.png`

 * *Files identical despite different names*

### Comparing `CatRoyale-1.6/assets/images/grass.png` & `CatRoyale-1.7/assets/images/grass.png`

 * *Files identical despite different names*

### Comparing `CatRoyale-1.6/assets/images/items.png` & `CatRoyale-1.7/assets/images/items.png`

 * *Files identical despite different names*

### Comparing `CatRoyale-1.6/assets/images/loading_screen.png` & `CatRoyale-1.7/assets/images/loading_screen.png`

 * *Files identical despite different names*

### Comparing `CatRoyale-1.6/assets/images/map/level00.png` & `CatRoyale-1.7/assets/images/map/level00.png`

 * *Files identical despite different names*

### Comparing `CatRoyale-1.6/classes/box.py` & `CatRoyale-1.7/classes/box.py`

 * *Files identical despite different names*

### Comparing `CatRoyale-1.6/classes/character.py` & `CatRoyale-1.7/classes/character.py`

 * *Files identical despite different names*

### Comparing `CatRoyale-1.6/classes/config.py` & `CatRoyale-1.7/classes/config.py`

 * *Files identical despite different names*

### Comparing `CatRoyale-1.6/classes/event_stack.py` & `CatRoyale-1.7/classes/event_stack.py`

 * *Files identical despite different names*

### Comparing `CatRoyale-1.6/classes/functions.py` & `CatRoyale-1.7/classes/functions.py`

 * *Files identical despite different names*

### Comparing `CatRoyale-1.6/classes/game_map.py` & `CatRoyale-1.7/classes/game_map.py`

 * *Files identical despite different names*

### Comparing `CatRoyale-1.6/classes/health_bars.py` & `CatRoyale-1.7/classes/health_bars.py`

 * *Files identical despite different names*

### Comparing `CatRoyale-1.6/classes/inventory.py` & `CatRoyale-1.7/classes/inventory.py`

 * *Files identical despite different names*

### Comparing `CatRoyale-1.6/classes/item.py` & `CatRoyale-1.7/classes/item.py`

 * *Files identical despite different names*

### Comparing `CatRoyale-1.6/classes/map_reader.py` & `CatRoyale-1.7/classes/map_reader.py`

 * *Files identical despite different names*

### Comparing `CatRoyale-1.6/classes/text_display.py` & `CatRoyale-1.7/classes/text_display.py`

 * *Files identical despite different names*

### Comparing `CatRoyale-1.6/config/config.json` & `CatRoyale-1.7/config/config.json`

 * *Files identical despite different names*

### Comparing `CatRoyale-1.6/main.py` & `CatRoyale-1.7/main.py`

 * *Files identical despite different names*

