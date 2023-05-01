# Comparing `tmp/edl-mod-0.0.31.tar.gz` & `tmp/edl-mod-0.0.32.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/srv/storage/projects/scripts/edl/dist/tmpgpuk7e31/edl-mod-0.0.31.tar", last modified: Thu Apr 27 20:51:54 2023, max compression
+gzip compressed data, was "/srv/storage/projects/scripts/edl/dist/tmpxkiu89xv/edl-mod-0.0.32.tar", last modified: Mon May  1 16:38:23 2023, max compression
```

## Comparing `edl-mod-0.0.31.tar` & `edl-mod-0.0.32.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwsr-x   0 ejohnfelt  (1500) storage   (1499)        0 2023-04-27 20:51:54.000000 edl-mod-0.0.31/
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      104 2022-03-11 14:46:04.000000 edl-mod-0.0.31/pyproject.toml
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)    46525 2023-04-27 20:51:12.000000 edl-mod-0.0.31/edl.py
-drwxrwsr-x   0 ejohnfelt  (1500) storage   (1499)        0 2023-04-27 20:51:54.000000 edl-mod-0.0.31/edl_mod.egg-info/
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)       14 2023-04-27 20:51:54.000000 edl-mod-0.0.31/edl_mod.egg-info/requires.txt
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)        1 2023-04-27 20:51:54.000000 edl-mod-0.0.31/edl_mod.egg-info/dependency_links.txt
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)        4 2023-04-27 20:51:54.000000 edl-mod-0.0.31/edl_mod.egg-info/top_level.txt
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      212 2023-04-27 20:51:54.000000 edl-mod-0.0.31/edl_mod.egg-info/SOURCES.txt
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      659 2023-04-27 20:51:54.000000 edl-mod-0.0.31/edl_mod.egg-info/PKG-INFO
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      100 2022-03-11 15:35:21.000000 edl-mod-0.0.31/README.md
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)     1070 2022-03-11 14:39:52.000000 edl-mod-0.0.31/LICENSE
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)       66 2022-03-13 05:45:40.000000 edl-mod-0.0.31/setup.py
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      659 2023-04-27 20:51:54.000000 edl-mod-0.0.31/PKG-INFO
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      734 2023-04-27 20:51:54.000000 edl-mod-0.0.31/setup.cfg
+drwxrwsr-x   0 ejohnfelt  (1500) storage   (1499)        0 2023-05-01 16:38:23.000000 edl-mod-0.0.32/
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      104 2022-03-11 14:46:04.000000 edl-mod-0.0.32/pyproject.toml
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)    46522 2023-05-01 16:37:11.000000 edl-mod-0.0.32/edl.py
+drwxrwsr-x   0 ejohnfelt  (1500) storage   (1499)        0 2023-05-01 16:38:23.000000 edl-mod-0.0.32/edl_mod.egg-info/
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)       14 2023-05-01 16:38:23.000000 edl-mod-0.0.32/edl_mod.egg-info/requires.txt
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)        1 2023-05-01 16:38:23.000000 edl-mod-0.0.32/edl_mod.egg-info/dependency_links.txt
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)        4 2023-05-01 16:38:23.000000 edl-mod-0.0.32/edl_mod.egg-info/top_level.txt
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      212 2023-05-01 16:38:23.000000 edl-mod-0.0.32/edl_mod.egg-info/SOURCES.txt
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      659 2023-05-01 16:38:23.000000 edl-mod-0.0.32/edl_mod.egg-info/PKG-INFO
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      100 2022-03-11 15:35:21.000000 edl-mod-0.0.32/README.md
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)     1070 2022-03-11 14:39:52.000000 edl-mod-0.0.32/LICENSE
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)       66 2022-03-13 05:45:40.000000 edl-mod-0.0.32/setup.py
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      659 2023-05-01 16:38:23.000000 edl-mod-0.0.32/PKG-INFO
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      734 2023-05-01 16:38:23.000000 edl-mod-0.0.32/setup.cfg
```

### Comparing `edl-mod-0.0.31/edl.py` & `edl-mod-0.0.32/edl.py`

 * *Files 0% similar despite different names*

```diff
@@ -714,15 +714,15 @@
 # Explicit No Prompt
 NoPrompt=False
 
 # Autosave EDLFIle
 AutoSave=False
 
 # Version
-VERSION=(0,0,31)
+VERSION=(0,0,32)
 Version = __version__ = ".".join([ str(x) for x in VERSION ])
 
 # Parser
 __Parser__ = None
 
 # Config File
 __Config__ = "/etc/edl/config"
@@ -1779,15 +1779,15 @@
 
 		items_culled = len(results)
 
 		if items_culled > 0:
 			Msg(f"{items_culled} records culled")
 
 			for item in results:
-				item.Print()
+				Msg(item)
 
 	elif op == "backup":
 		Backup(EDLMaster)
 		Backup(EDLFile)
 	elif op == "restore":
 		Restore(EDLMaster)
 		Restore(EDLFile)
```

### Comparing `edl-mod-0.0.31/edl_mod.egg-info/PKG-INFO` & `edl-mod-0.0.32/edl_mod.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edl-mod
-Version: 0.0.31
+Version: 0.0.32
 Summary: Module for editting and searching external dynamic lists (EDLs)
 Home-page: https://github.com/ejohnfel/edl
 Author: Eric Johnfelt
 Author-email: ejohnfel@hotmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/ejohnfel/edl/issues
 Platform: UNKNOWN
```

### Comparing `edl-mod-0.0.31/LICENSE` & `edl-mod-0.0.32/LICENSE`

 * *Files identical despite different names*

### Comparing `edl-mod-0.0.31/PKG-INFO` & `edl-mod-0.0.32/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edl-mod
-Version: 0.0.31
+Version: 0.0.32
 Summary: Module for editting and searching external dynamic lists (EDLs)
 Home-page: https://github.com/ejohnfel/edl
 Author: Eric Johnfelt
 Author-email: ejohnfel@hotmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/ejohnfel/edl/issues
 Platform: UNKNOWN
```

### Comparing `edl-mod-0.0.31/setup.cfg` & `edl-mod-0.0.32/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 formats = zip,tar
 
 [bdist_wheel]
 universal = 1
 
 [metadata]
 name = edl-mod
-version = 0.0.31
+version = 0.0.32
 author = Eric Johnfelt
 author_email = ejohnfel@hotmail.com
 description = Module for editting and searching external dynamic lists (EDLs)
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/ejohnfel/edl
 project_urls =
```

