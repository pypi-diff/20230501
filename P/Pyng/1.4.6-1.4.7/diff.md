# Comparing `tmp/Pyng-1.4.6.tar.gz` & `tmp/Pyng-1.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Pyng-1.4.6.tar", last modified: Wed Apr 19 19:54:18 2023, max compression
+gzip compressed data, was "Pyng-1.4.7.tar", last modified: Mon May  1 19:28:59 2023, max compression
```

## Comparing `Pyng-1.4.6.tar` & `Pyng-1.4.7.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 nat        (502) staff       (20)        0 2023-04-19 19:54:18.402196 Pyng-1.4.6/
--rw-r--r--   0 nat        (502) staff       (20)        9 2020-03-18 20:11:04.000000 Pyng-1.4.6/.gitignore
--rw-r--r--   0 nat        (502) staff       (20)     3358 2023-04-19 19:53:19.000000 Pyng-1.4.6/CHANGES.txt
--rw-r--r--   0 nat        (502) staff       (20)     1095 2020-03-18 20:10:27.000000 Pyng-1.4.6/LICENSE.txt
--rw-r--r--   0 nat        (502) staff       (20)       15 2020-03-18 20:10:27.000000 Pyng-1.4.6/MANIFEST.in
--rw-r--r--   0 nat        (502) staff       (20)     2002 2023-04-19 19:54:18.401473 Pyng-1.4.6/PKG-INFO
-drwxr-xr-x   0 nat        (502) staff       (20)        0 2023-04-19 19:54:18.223605 Pyng-1.4.6/Pyng.egg-info/
--rw-r--r--   0 nat        (502) staff       (20)     2002 2023-04-19 19:54:18.000000 Pyng-1.4.6/Pyng.egg-info/PKG-INFO
--rw-r--r--   0 nat        (502) staff       (20)      959 2023-04-19 19:54:18.000000 Pyng-1.4.6/Pyng.egg-info/SOURCES.txt
--rw-r--r--   0 nat        (502) staff       (20)        1 2023-04-19 19:54:18.000000 Pyng-1.4.6/Pyng.egg-info/dependency_links.txt
--rw-r--r--   0 nat        (502) staff       (20)       47 2023-04-19 19:54:18.000000 Pyng-1.4.6/Pyng.egg-info/entry_points.txt
--rw-r--r--   0 nat        (502) staff       (20)        5 2023-04-19 19:54:18.000000 Pyng-1.4.6/Pyng.egg-info/top_level.txt
--rw-r--r--   0 nat        (502) staff       (20)     1794 2020-03-18 20:10:27.000000 Pyng-1.4.6/README.txt
-drwxr-xr-x   0 nat        (502) staff       (20)        0 2023-04-19 19:54:18.341176 Pyng-1.4.6/pyng/
--rwxr-xr-x   0 nat        (502) staff       (20)    49420 2022-01-26 17:04:01.000000 Pyng-1.4.6/pyng/ProgressBar.py
--rw-r--r--   0 nat        (502) staff       (20)     5708 2022-01-26 17:04:01.000000 Pyng-1.4.6/pyng/ProgressMeter.py
--rw-r--r--   0 nat        (502) staff       (20)      151 2020-03-18 20:10:27.000000 Pyng-1.4.6/pyng/__init__.py
--rwxr-xr-x   0 nat        (502) staff       (20)     3559 2021-08-13 20:35:53.000000 Pyng-1.4.6/pyng/args.py
--rw-r--r--   0 nat        (502) staff       (20)    19962 2022-11-21 19:45:12.000000 Pyng-1.4.6/pyng/commands.py
--rw-r--r--   0 nat        (502) staff       (20)     4281 2020-10-29 21:16:26.000000 Pyng-1.4.6/pyng/deco.py
--rw-r--r--   0 nat        (502) staff       (20)     3847 2022-03-16 14:55:58.000000 Pyng-1.4.6/pyng/descrs.py
--rw-r--r--   0 nat        (502) staff       (20)    11376 2022-01-26 17:04:01.000000 Pyng-1.4.6/pyng/dicts.py
--rw-r--r--   0 nat        (502) staff       (20)    31509 2022-10-12 18:21:33.000000 Pyng-1.4.6/pyng/exc.py
--rw-r--r--   0 nat        (502) staff       (20)     2969 2022-01-31 17:04:02.000000 Pyng-1.4.6/pyng/exc3.py
--rw-r--r--   0 nat        (502) staff       (20)    15993 2022-08-04 21:36:14.000000 Pyng-1.4.6/pyng/file_arg.py
--rw-r--r--   0 nat        (502) staff       (20)     1759 2020-03-18 20:10:27.000000 Pyng-1.4.6/pyng/find.py
--rw-r--r--   0 nat        (502) staff       (20)     4333 2020-03-18 20:10:27.000000 Pyng-1.4.6/pyng/genio.py
--rw-r--r--   0 nat        (502) staff       (20)     7891 2020-03-18 20:10:27.000000 Pyng-1.4.6/pyng/graph.py
--rw-r--r--   0 nat        (502) staff       (20)     8434 2022-03-16 14:22:53.000000 Pyng-1.4.6/pyng/iters.py
--rw-r--r--   0 nat        (502) staff       (20)    10870 2022-01-26 17:04:01.000000 Pyng-1.4.6/pyng/janitor.py
--rw-r--r--   0 nat        (502) staff       (20)     4678 2022-02-03 15:30:19.000000 Pyng-1.4.6/pyng/logs.py
--rw-r--r--   0 nat        (502) staff       (20)     8372 2020-03-18 20:10:31.000000 Pyng-1.4.6/pyng/methods.py
--rw-r--r--   0 nat        (502) staff       (20)    23589 2021-02-24 18:13:01.000000 Pyng-1.4.6/pyng/out.py
--rw-r--r--   0 nat        (502) staff       (20)      167 2020-03-18 20:10:31.000000 Pyng-1.4.6/pyng/path.py
--rw-r--r--   0 nat        (502) staff       (20)     1672 2020-04-29 01:52:22.000000 Pyng-1.4.6/pyng/pickles.py
--rw-r--r--   0 nat        (502) staff       (20)      529 2020-03-18 20:10:27.000000 Pyng-1.4.6/pyng/raise_from3.py
--rw-r--r--   0 nat        (502) staff       (20)      381 2020-03-18 20:10:27.000000 Pyng-1.4.6/pyng/raise_with2.py
--rw-r--r--   0 nat        (502) staff       (20)     3812 2020-03-18 20:10:27.000000 Pyng-1.4.6/pyng/relwalk.py
--rw-r--r--   0 nat        (502) staff       (20)     6526 2023-04-12 15:16:27.000000 Pyng-1.4.6/pyng/replacefile.py
-drwxr-xr-x   0 nat        (502) staff       (20)        0 2023-04-19 19:54:18.372526 Pyng-1.4.6/pyng/test/
--rw-r--r--   0 nat        (502) staff       (20)      151 2020-03-18 20:10:27.000000 Pyng-1.4.6/pyng/test/__init__.py
--rw-r--r--   0 nat        (502) staff       (20)     4296 2020-10-29 21:32:14.000000 Pyng-1.4.6/pyng/test/test_deco.py
--rw-r--r--   0 nat        (502) staff       (20)    10602 2022-01-26 17:04:01.000000 Pyng-1.4.6/pyng/test/test_exc.py
--rw-r--r--   0 nat        (502) staff       (20)      151 2020-03-18 20:10:27.000000 Pyng-1.4.6/pyng/test/test_genio.py
--rw-r--r--   0 nat        (502) staff       (20)     5164 2022-01-26 17:04:01.000000 Pyng-1.4.6/pyng/test/test_iters.py
--rw-r--r--   0 nat        (502) staff       (20)     5309 2022-01-26 17:04:01.000000 Pyng-1.4.6/pyng/test/test_out.py
--rw-r--r--   0 nat        (502) staff       (20)      151 2020-03-18 20:10:27.000000 Pyng-1.4.6/pyng/test/test_relwalk.py
--rw-r--r--   0 nat        (502) staff       (20)     6332 2020-03-18 20:10:27.000000 Pyng-1.4.6/pyng/test/test_replacefile.py
--rw-r--r--   0 nat        (502) staff       (20)     8793 2022-01-26 17:04:01.000000 Pyng-1.4.6/pyng/timing.py
-drwxr-xr-x   0 nat        (502) staff       (20)        0 2023-04-19 19:54:18.400160 Pyng-1.4.6/pyng/tk/
--rw-r--r--   0 nat        (502) staff       (20)     3798 2015-11-05 23:25:02.000000 Pyng-1.4.6/pyng/tk/FitText.py
--rw-r--r--   0 nat        (502) staff       (20)     9320 2022-01-26 17:04:01.000000 Pyng-1.4.6/pyng/tk/__init__.py
--rw-r--r--   0 nat        (502) staff       (20)    16498 2022-01-26 17:04:01.000000 Pyng-1.4.6/pyng/tk/form.py
--rw-r--r--   0 nat        (502) staff       (20)      982 2020-03-18 20:10:27.000000 Pyng-1.4.6/pyng/tk/getpw.py
--rw-r--r--   0 nat        (502) staff       (20)     9488 2020-04-24 00:49:55.000000 Pyng-1.4.6/pyng/tk/multistatus.py
--rwxr-xr-x   0 nat        (502) staff       (20)     4969 2021-08-23 12:40:49.000000 Pyng-1.4.6/pyng/tk/popup.py
--rwxr-xr-x   0 nat        (502) staff       (20)     5862 2022-01-26 17:04:01.000000 Pyng-1.4.6/pyng/tk/printwindow.py
--rw-r--r--   0 nat        (502) staff       (20)     5140 2020-03-18 20:10:28.000000 Pyng-1.4.6/pyng/toposort.py
--rw-r--r--   0 nat        (502) staff       (20)       38 2023-04-19 19:54:18.402323 Pyng-1.4.6/setup.cfg
--rw-r--r--   0 nat        (502) staff       (20)      969 2022-01-26 17:04:01.000000 Pyng-1.4.6/setup.py
+drwxr-xr-x   0 nat        (502) staff       (20)        0 2023-05-01 19:28:59.266222 Pyng-1.4.7/
+-rw-r--r--   0 nat        (502) staff       (20)        9 2020-03-18 20:11:04.000000 Pyng-1.4.7/.gitignore
+-rw-r--r--   0 nat        (502) staff       (20)     3430 2023-05-01 19:27:57.000000 Pyng-1.4.7/CHANGES.txt
+-rw-r--r--   0 nat        (502) staff       (20)     1095 2020-03-18 20:10:27.000000 Pyng-1.4.7/LICENSE.txt
+-rw-r--r--   0 nat        (502) staff       (20)       15 2020-03-18 20:10:27.000000 Pyng-1.4.7/MANIFEST.in
+-rw-r--r--   0 nat        (502) staff       (20)     2002 2023-05-01 19:28:59.265557 Pyng-1.4.7/PKG-INFO
+drwxr-xr-x   0 nat        (502) staff       (20)        0 2023-05-01 19:28:59.085227 Pyng-1.4.7/Pyng.egg-info/
+-rw-r--r--   0 nat        (502) staff       (20)     2002 2023-05-01 19:28:58.000000 Pyng-1.4.7/Pyng.egg-info/PKG-INFO
+-rw-r--r--   0 nat        (502) staff       (20)      959 2023-05-01 19:28:58.000000 Pyng-1.4.7/Pyng.egg-info/SOURCES.txt
+-rw-r--r--   0 nat        (502) staff       (20)        1 2023-05-01 19:28:58.000000 Pyng-1.4.7/Pyng.egg-info/dependency_links.txt
+-rw-r--r--   0 nat        (502) staff       (20)       47 2023-05-01 19:28:58.000000 Pyng-1.4.7/Pyng.egg-info/entry_points.txt
+-rw-r--r--   0 nat        (502) staff       (20)        5 2023-05-01 19:28:58.000000 Pyng-1.4.7/Pyng.egg-info/top_level.txt
+-rw-r--r--   0 nat        (502) staff       (20)     1794 2020-03-18 20:10:27.000000 Pyng-1.4.7/README.txt
+drwxr-xr-x   0 nat        (502) staff       (20)        0 2023-05-01 19:28:59.206157 Pyng-1.4.7/pyng/
+-rwxr-xr-x   0 nat        (502) staff       (20)    49420 2022-01-26 17:04:01.000000 Pyng-1.4.7/pyng/ProgressBar.py
+-rw-r--r--   0 nat        (502) staff       (20)     5708 2022-01-26 17:04:01.000000 Pyng-1.4.7/pyng/ProgressMeter.py
+-rw-r--r--   0 nat        (502) staff       (20)      151 2020-03-18 20:10:27.000000 Pyng-1.4.7/pyng/__init__.py
+-rwxr-xr-x   0 nat        (502) staff       (20)     3559 2021-08-13 20:35:53.000000 Pyng-1.4.7/pyng/args.py
+-rw-r--r--   0 nat        (502) staff       (20)    19962 2022-11-21 19:45:12.000000 Pyng-1.4.7/pyng/commands.py
+-rw-r--r--   0 nat        (502) staff       (20)     4281 2020-10-29 21:16:26.000000 Pyng-1.4.7/pyng/deco.py
+-rw-r--r--   0 nat        (502) staff       (20)     3847 2022-03-16 14:55:58.000000 Pyng-1.4.7/pyng/descrs.py
+-rw-r--r--   0 nat        (502) staff       (20)    11376 2022-01-26 17:04:01.000000 Pyng-1.4.7/pyng/dicts.py
+-rw-r--r--   0 nat        (502) staff       (20)    31509 2022-10-12 18:21:33.000000 Pyng-1.4.7/pyng/exc.py
+-rw-r--r--   0 nat        (502) staff       (20)     2969 2022-01-31 17:04:02.000000 Pyng-1.4.7/pyng/exc3.py
+-rw-r--r--   0 nat        (502) staff       (20)    15993 2022-08-04 21:36:14.000000 Pyng-1.4.7/pyng/file_arg.py
+-rw-r--r--   0 nat        (502) staff       (20)     1759 2020-03-18 20:10:27.000000 Pyng-1.4.7/pyng/find.py
+-rw-r--r--   0 nat        (502) staff       (20)     4333 2020-03-18 20:10:27.000000 Pyng-1.4.7/pyng/genio.py
+-rw-r--r--   0 nat        (502) staff       (20)     7891 2020-03-18 20:10:27.000000 Pyng-1.4.7/pyng/graph.py
+-rw-r--r--   0 nat        (502) staff       (20)     8434 2022-03-16 14:22:53.000000 Pyng-1.4.7/pyng/iters.py
+-rw-r--r--   0 nat        (502) staff       (20)    10870 2022-01-26 17:04:01.000000 Pyng-1.4.7/pyng/janitor.py
+-rw-r--r--   0 nat        (502) staff       (20)     4678 2022-02-03 15:30:19.000000 Pyng-1.4.7/pyng/logs.py
+-rw-r--r--   0 nat        (502) staff       (20)     8372 2020-03-18 20:10:31.000000 Pyng-1.4.7/pyng/methods.py
+-rw-r--r--   0 nat        (502) staff       (20)    23696 2023-05-01 19:26:59.000000 Pyng-1.4.7/pyng/out.py
+-rw-r--r--   0 nat        (502) staff       (20)      167 2020-03-18 20:10:31.000000 Pyng-1.4.7/pyng/path.py
+-rw-r--r--   0 nat        (502) staff       (20)     1672 2020-04-29 01:52:22.000000 Pyng-1.4.7/pyng/pickles.py
+-rw-r--r--   0 nat        (502) staff       (20)      529 2020-03-18 20:10:27.000000 Pyng-1.4.7/pyng/raise_from3.py
+-rw-r--r--   0 nat        (502) staff       (20)      381 2020-03-18 20:10:27.000000 Pyng-1.4.7/pyng/raise_with2.py
+-rw-r--r--   0 nat        (502) staff       (20)     3812 2020-03-18 20:10:27.000000 Pyng-1.4.7/pyng/relwalk.py
+-rw-r--r--   0 nat        (502) staff       (20)     6526 2023-04-12 15:16:27.000000 Pyng-1.4.7/pyng/replacefile.py
+drwxr-xr-x   0 nat        (502) staff       (20)        0 2023-05-01 19:28:59.235821 Pyng-1.4.7/pyng/test/
+-rw-r--r--   0 nat        (502) staff       (20)      151 2020-03-18 20:10:27.000000 Pyng-1.4.7/pyng/test/__init__.py
+-rw-r--r--   0 nat        (502) staff       (20)     4296 2020-10-29 21:32:14.000000 Pyng-1.4.7/pyng/test/test_deco.py
+-rw-r--r--   0 nat        (502) staff       (20)    10602 2022-01-26 17:04:01.000000 Pyng-1.4.7/pyng/test/test_exc.py
+-rw-r--r--   0 nat        (502) staff       (20)      151 2020-03-18 20:10:27.000000 Pyng-1.4.7/pyng/test/test_genio.py
+-rw-r--r--   0 nat        (502) staff       (20)     5164 2022-01-26 17:04:01.000000 Pyng-1.4.7/pyng/test/test_iters.py
+-rw-r--r--   0 nat        (502) staff       (20)     5309 2022-01-26 17:04:01.000000 Pyng-1.4.7/pyng/test/test_out.py
+-rw-r--r--   0 nat        (502) staff       (20)      151 2020-03-18 20:10:27.000000 Pyng-1.4.7/pyng/test/test_relwalk.py
+-rw-r--r--   0 nat        (502) staff       (20)     6332 2020-03-18 20:10:27.000000 Pyng-1.4.7/pyng/test/test_replacefile.py
+-rw-r--r--   0 nat        (502) staff       (20)     8793 2022-01-26 17:04:01.000000 Pyng-1.4.7/pyng/timing.py
+drwxr-xr-x   0 nat        (502) staff       (20)        0 2023-05-01 19:28:59.264515 Pyng-1.4.7/pyng/tk/
+-rw-r--r--   0 nat        (502) staff       (20)     3798 2015-11-05 23:25:02.000000 Pyng-1.4.7/pyng/tk/FitText.py
+-rw-r--r--   0 nat        (502) staff       (20)     9320 2022-01-26 17:04:01.000000 Pyng-1.4.7/pyng/tk/__init__.py
+-rw-r--r--   0 nat        (502) staff       (20)    16498 2022-01-26 17:04:01.000000 Pyng-1.4.7/pyng/tk/form.py
+-rw-r--r--   0 nat        (502) staff       (20)      982 2020-03-18 20:10:27.000000 Pyng-1.4.7/pyng/tk/getpw.py
+-rw-r--r--   0 nat        (502) staff       (20)     9488 2020-04-24 00:49:55.000000 Pyng-1.4.7/pyng/tk/multistatus.py
+-rwxr-xr-x   0 nat        (502) staff       (20)     4969 2021-08-23 12:40:49.000000 Pyng-1.4.7/pyng/tk/popup.py
+-rwxr-xr-x   0 nat        (502) staff       (20)     5862 2022-01-26 17:04:01.000000 Pyng-1.4.7/pyng/tk/printwindow.py
+-rw-r--r--   0 nat        (502) staff       (20)     5140 2020-03-18 20:10:28.000000 Pyng-1.4.7/pyng/toposort.py
+-rw-r--r--   0 nat        (502) staff       (20)       38 2023-05-01 19:28:59.266341 Pyng-1.4.7/setup.cfg
+-rw-r--r--   0 nat        (502) staff       (20)      969 2022-01-26 17:04:01.000000 Pyng-1.4.7/setup.py
```

### Comparing `Pyng-1.4.6/CHANGES.txt` & `Pyng-1.4.7/CHANGES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -51,7 +51,8 @@
 v1.4.0,  2022-05-16 - add file_arg
 v1.4.1,  2022-05-18 - fix bug in file_arg.files_from()
 v1.4.2,  2022-06-15 - give commands.Commands subcommand parsers descriptions
 v1.4.3,  2022-06-15 - use exc.describe() for commands args.run() exception
 v1.4.4,  2022-08-04 - file_arg.files_from(), files_in_tree() get ignore_dirs
 v1.4.5,  2022-11-21 - make commands.Commands.get_parser(score) apply to params
 v1.4.6,  2023-04-19 - tweaks to exc.exceptlink, replacefile.ReplaceFile
+v1.4.7,  2023-05-01 - defend out from Windows: handle absence of syslog
```

### Comparing `Pyng-1.4.6/LICENSE.txt` & `Pyng-1.4.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Pyng-1.4.6/PKG-INFO` & `Pyng-1.4.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pyng
-Version: 1.4.6
+Version: 1.4.7
 Summary: Yet another collection of Python utility functions
 Home-page: https://pypi.org/project/Pyng/
 Author: Nat Goodspeed
 Author-email: nat.cognitoy@gmail.com
 License: LICENSE.txt
 License-File: LICENSE.txt
```

### Comparing `Pyng-1.4.6/Pyng.egg-info/PKG-INFO` & `Pyng-1.4.7/Pyng.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pyng
-Version: 1.4.6
+Version: 1.4.7
 Summary: Yet another collection of Python utility functions
 Home-page: https://pypi.org/project/Pyng/
 Author: Nat Goodspeed
 Author-email: nat.cognitoy@gmail.com
 License: LICENSE.txt
 License-File: LICENSE.txt
```

### Comparing `Pyng-1.4.6/Pyng.egg-info/SOURCES.txt` & `Pyng-1.4.7/Pyng.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Pyng-1.4.6/README.txt` & `Pyng-1.4.7/README.txt`

 * *Files identical despite different names*

### Comparing `Pyng-1.4.6/pyng/ProgressBar.py` & `Pyng-1.4.7/pyng/ProgressBar.py`

 * *Files identical despite different names*

### Comparing `Pyng-1.4.6/pyng/ProgressMeter.py` & `Pyng-1.4.7/pyng/ProgressMeter.py`

 * *Files identical despite different names*

### Comparing `Pyng-1.4.6/pyng/args.py` & `Pyng-1.4.7/pyng/args.py`

 * *Files identical despite different names*

### Comparing `Pyng-1.4.6/pyng/commands.py` & `Pyng-1.4.7/pyng/commands.py`

 * *Files identical despite different names*

### Comparing `Pyng-1.4.6/pyng/deco.py` & `Pyng-1.4.7/pyng/deco.py`

 * *Files identical despite different names*

### Comparing `Pyng-1.4.6/pyng/descrs.py` & `Pyng-1.4.7/pyng/descrs.py`

 * *Files identical despite different names*

### Comparing `Pyng-1.4.6/pyng/dicts.py` & `Pyng-1.4.7/pyng/dicts.py`

 * *Files identical despite different names*

### Comparing `Pyng-1.4.6/pyng/exc.py` & `Pyng-1.4.7/pyng/exc.py`

 * *Files identical despite different names*

### Comparing `Pyng-1.4.6/pyng/exc3.py` & `Pyng-1.4.7/pyng/exc3.py`

 * *Files identical despite different names*

### Comparing `Pyng-1.4.6/pyng/file_arg.py` & `Pyng-1.4.7/pyng/file_arg.py`

 * *Files identical despite different names*

### Comparing `Pyng-1.4.6/pyng/find.py` & `Pyng-1.4.7/pyng/find.py`

 * *Files identical despite different names*

### Comparing `Pyng-1.4.6/pyng/genio.py` & `Pyng-1.4.7/pyng/genio.py`

 * *Files identical despite different names*

### Comparing `Pyng-1.4.6/pyng/graph.py` & `Pyng-1.4.7/pyng/graph.py`

 * *Files identical despite different names*

### Comparing `Pyng-1.4.6/pyng/iters.py` & `Pyng-1.4.7/pyng/iters.py`

 * *Files identical despite different names*

### Comparing `Pyng-1.4.6/pyng/janitor.py` & `Pyng-1.4.7/pyng/janitor.py`

 * *Files identical despite different names*

### Comparing `Pyng-1.4.6/pyng/logs.py` & `Pyng-1.4.7/pyng/logs.py`

 * *Files identical despite different names*

### Comparing `Pyng-1.4.6/pyng/methods.py` & `Pyng-1.4.7/pyng/methods.py`

 * *Files identical despite different names*

### Comparing `Pyng-1.4.6/pyng/out.py` & `Pyng-1.4.7/pyng/out.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,19 @@
 from collections import namedtuple
 from contextlib import contextmanager
 import datetime
 from functools import wraps
 import json
 import logging
 from pyng.exc import exceptlink, describe
-import syslog
+try:
+    import syslog
+except ImportError:
+    # not Windows, just skip
+    pass
 
 class OutError(Exception):
     pass
 
 def push_generator(func):
     """
     Decorate a push generator such that calling it returns a handle on which
@@ -340,15 +344,17 @@
         syslog.syslog(kwds.pop("level", self.level), text)
 
     def flush(self):
         pass
 
 def syslogger(*args, **kwds):
     """
-    Wrap _syslogger so that we properly buffer lines to go to the log.
+    Wrap _syslogger so that we properly buffer lines to go to syslog.
+
+    This is, of course, Posix-specific.
     """
     return buffer_lines(_syslogger(*args, **kwds))
 
 logwrappers = namedtuple('logwrappers',
                          ('debug', 'info', 'warning', 'error', 'critical', 'exception'))
 
 def wraplogger(logger):
```

### Comparing `Pyng-1.4.6/pyng/pickles.py` & `Pyng-1.4.7/pyng/pickles.py`

 * *Files identical despite different names*

### Comparing `Pyng-1.4.6/pyng/raise_from3.py` & `Pyng-1.4.7/pyng/raise_from3.py`

 * *Files identical despite different names*

### Comparing `Pyng-1.4.6/pyng/relwalk.py` & `Pyng-1.4.7/pyng/relwalk.py`

 * *Files identical despite different names*

### Comparing `Pyng-1.4.6/pyng/replacefile.py` & `Pyng-1.4.7/pyng/replacefile.py`

 * *Files identical despite different names*

### Comparing `Pyng-1.4.6/pyng/test/test_deco.py` & `Pyng-1.4.7/pyng/test/test_deco.py`

 * *Files identical despite different names*

### Comparing `Pyng-1.4.6/pyng/test/test_exc.py` & `Pyng-1.4.7/pyng/test/test_exc.py`

 * *Files identical despite different names*

### Comparing `Pyng-1.4.6/pyng/test/test_iters.py` & `Pyng-1.4.7/pyng/test/test_iters.py`

 * *Files identical despite different names*

### Comparing `Pyng-1.4.6/pyng/test/test_out.py` & `Pyng-1.4.7/pyng/test/test_out.py`

 * *Files identical despite different names*

### Comparing `Pyng-1.4.6/pyng/test/test_replacefile.py` & `Pyng-1.4.7/pyng/test/test_replacefile.py`

 * *Files identical despite different names*

### Comparing `Pyng-1.4.6/pyng/timing.py` & `Pyng-1.4.7/pyng/timing.py`

 * *Files identical despite different names*

### Comparing `Pyng-1.4.6/pyng/tk/FitText.py` & `Pyng-1.4.7/pyng/tk/FitText.py`

 * *Files identical despite different names*

### Comparing `Pyng-1.4.6/pyng/tk/__init__.py` & `Pyng-1.4.7/pyng/tk/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyng-1.4.6/pyng/tk/form.py` & `Pyng-1.4.7/pyng/tk/form.py`

 * *Files identical despite different names*

### Comparing `Pyng-1.4.6/pyng/tk/getpw.py` & `Pyng-1.4.7/pyng/tk/getpw.py`

 * *Files identical despite different names*

### Comparing `Pyng-1.4.6/pyng/tk/multistatus.py` & `Pyng-1.4.7/pyng/tk/multistatus.py`

 * *Files identical despite different names*

### Comparing `Pyng-1.4.6/pyng/tk/popup.py` & `Pyng-1.4.7/pyng/tk/popup.py`

 * *Files identical despite different names*

### Comparing `Pyng-1.4.6/pyng/tk/printwindow.py` & `Pyng-1.4.7/pyng/tk/printwindow.py`

 * *Files identical despite different names*

### Comparing `Pyng-1.4.6/pyng/toposort.py` & `Pyng-1.4.7/pyng/toposort.py`

 * *Files identical despite different names*

### Comparing `Pyng-1.4.6/setup.py` & `Pyng-1.4.7/setup.py`

 * *Files identical despite different names*

