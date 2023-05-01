# Comparing `tmp/skainet-0.0.0.dev4.tar.gz` & `tmp/skainet-0.0.0.dev8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/skainet/skainet/dist/.tmp-27hju3ix/skainet-0.0.0.dev4.tar", last modified: Thu Apr 20 23:51:02 2023, max compression
+gzip compressed data, was "/home/runner/work/skainet/skainet/dist/.tmp-6ftqtqr_/skainet-0.0.0.dev8.tar", last modified: Mon May  1 17:23:31 2023, max compression
```

## Comparing `skainet-0.0.0.dev4.tar` & `skainet-0.0.0.dev8.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 23:51:02.000000 skainet-0.0.0.dev4/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-20 23:51:02.000000 skainet-0.0.0.dev4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-04-20 23:50:47.000000 skainet-0.0.0.dev4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-20 23:50:47.000000 skainet-0.0.0.dev4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 23:51:02.000000 skainet-0.0.0.dev4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 23:51:02.000000 skainet-0.0.0.dev4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 23:51:02.000000 skainet-0.0.0.dev4/src/skainet/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 23:50:47.000000 skainet-0.0.0.dev4/src/skainet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-04-20 23:50:47.000000 skainet-0.0.0.dev4/src/skainet/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-04-20 23:50:47.000000 skainet-0.0.0.dev4/src/skainet/audio.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-04-20 23:50:47.000000 skainet-0.0.0.dev4/src/skainet/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-04-20 23:50:47.000000 skainet-0.0.0.dev4/src/skainet/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-04-20 23:50:47.000000 skainet-0.0.0.dev4/src/skainet/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     4924 2023-04-20 23:50:47.000000 skainet-0.0.0.dev4/src/skainet/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-04-20 23:50:47.000000 skainet-0.0.0.dev4/src/skainet/model.py
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-20 23:50:47.000000 skainet-0.0.0.dev4/src/skainet/moderate.py
--rw-r--r--   0 runner    (1001) docker     (123)    11224 2023-04-20 23:50:47.000000 skainet-0.0.0.dev4/src/skainet/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-04-20 23:50:47.000000 skainet-0.0.0.dev4/src/skainet/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 23:51:02.000000 skainet-0.0.0.dev4/src/skainet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-20 23:51:02.000000 skainet-0.0.0.dev4/src/skainet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-20 23:51:02.000000 skainet-0.0.0.dev4/src/skainet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 23:51:02.000000 skainet-0.0.0.dev4/src/skainet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-20 23:51:02.000000 skainet-0.0.0.dev4/src/skainet.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-20 23:51:02.000000 skainet-0.0.0.dev4/src/skainet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-20 23:51:02.000000 skainet-0.0.0.dev4/src/skainet.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:23:31.000000 skainet-0.0.0.dev8/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-01 17:23:31.000000 skainet-0.0.0.dev8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-05-01 17:23:16.000000 skainet-0.0.0.dev8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-05-01 17:23:16.000000 skainet-0.0.0.dev8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 17:23:31.000000 skainet-0.0.0.dev8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:23:31.000000 skainet-0.0.0.dev8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:23:31.000000 skainet-0.0.0.dev8/src/skainet/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 17:23:16.000000 skainet-0.0.0.dev8/src/skainet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-05-01 17:23:16.000000 skainet-0.0.0.dev8/src/skainet/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-05-01 17:23:16.000000 skainet-0.0.0.dev8/src/skainet/audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-01 17:23:16.000000 skainet-0.0.0.dev8/src/skainet/config.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-01 17:23:16.000000 skainet-0.0.0.dev8/src/skainet/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-05-01 17:23:16.000000 skainet-0.0.0.dev8/src/skainet/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-05-01 17:23:16.000000 skainet-0.0.0.dev8/src/skainet/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4924 2023-05-01 17:23:16.000000 skainet-0.0.0.dev8/src/skainet/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-05-01 17:23:16.000000 skainet-0.0.0.dev8/src/skainet/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-05-01 17:23:16.000000 skainet-0.0.0.dev8/src/skainet/moderate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11224 2023-05-01 17:23:16.000000 skainet-0.0.0.dev8/src/skainet/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-05-01 17:23:16.000000 skainet-0.0.0.dev8/src/skainet/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:23:31.000000 skainet-0.0.0.dev8/src/skainet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-01 17:23:31.000000 skainet-0.0.0.dev8/src/skainet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-01 17:23:31.000000 skainet-0.0.0.dev8/src/skainet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 17:23:31.000000 skainet-0.0.0.dev8/src/skainet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-01 17:23:31.000000 skainet-0.0.0.dev8/src/skainet.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-01 17:23:31.000000 skainet-0.0.0.dev8/src/skainet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-01 17:23:31.000000 skainet-0.0.0.dev8/src/skainet.egg-info/top_level.txt
```

### Comparing `skainet-0.0.0.dev4/README.md` & `skainet-0.0.0.dev8/README.md`

 * *Files identical despite different names*

### Comparing `skainet-0.0.0.dev4/pyproject.toml` & `skainet-0.0.0.dev8/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [project]
 name = "skainet"
-version = "0.0.0.dev4"
+version = "0.0.0.dev8"
 authors = [
     {name = "Zach Morris", email = "zacharymorr@outlook.com"}
 ]
 requires-python = ">=3.7"
 dependencies = [
     "openai==0.27.4",
     "click==8.1.3",
@@ -18,14 +18,17 @@
 
 [tool.setuptools]
 package-dir = {"" = "src"}
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
+[tool.setuptools.package-data]
+skainet = ["*.ini"]
+
 [tool.isort]
 profile = "black"
 
 [tool.commitizen]
 name = "cz_conventional_commits"
 version = "0.0.0"
 version_files = [
```

### Comparing `skainet-0.0.0.dev4/src/skainet/__main__.py` & `skainet-0.0.0.dev8/src/skainet/__main__.py`

 * *Files identical despite different names*

### Comparing `skainet-0.0.0.dev4/src/skainet/audio.py` & `skainet-0.0.0.dev8/src/skainet/audio.py`

 * *Files identical despite different names*

### Comparing `skainet-0.0.0.dev4/src/skainet/config.py` & `skainet-0.0.0.dev8/src/skainet/config.py`

 * *Files identical despite different names*

### Comparing `skainet-0.0.0.dev4/src/skainet/data.py` & `skainet-0.0.0.dev8/src/skainet/data.py`

 * *Files identical despite different names*

### Comparing `skainet-0.0.0.dev4/src/skainet/file.py` & `skainet-0.0.0.dev8/src/skainet/file.py`

 * *Files identical despite different names*

### Comparing `skainet-0.0.0.dev4/src/skainet/image.py` & `skainet-0.0.0.dev8/src/skainet/image.py`

 * *Files identical despite different names*

### Comparing `skainet-0.0.0.dev4/src/skainet/model.py` & `skainet-0.0.0.dev8/src/skainet/model.py`

 * *Files identical despite different names*

### Comparing `skainet-0.0.0.dev4/src/skainet/moderate.py` & `skainet-0.0.0.dev8/src/skainet/moderate.py`

 * *Files identical despite different names*

### Comparing `skainet-0.0.0.dev4/src/skainet/text.py` & `skainet-0.0.0.dev8/src/skainet/text.py`

 * *Files identical despite different names*

### Comparing `skainet-0.0.0.dev4/src/skainet/utils.py` & `skainet-0.0.0.dev8/src/skainet/utils.py`

 * *Files identical despite different names*

