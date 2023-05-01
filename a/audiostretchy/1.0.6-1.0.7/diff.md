# Comparing `tmp/audiostretchy-1.0.6.tar.gz` & `tmp/audiostretchy-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audiostretchy-1.0.6.tar", last modified: Mon May  1 00:36:59 2023, max compression
+gzip compressed data, was "audiostretchy-1.0.7.tar", last modified: Mon May  1 00:42:55 2023, max compression
```

## Comparing `audiostretchy-1.0.6.tar` & `audiostretchy-1.0.7.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:36:59.728857 audiostretchy-1.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-01 00:36:48.000000 audiostretchy-1.0.6/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:36:59.724857 audiostretchy-1.0.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:36:59.728857 audiostretchy-1.0.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-01 00:36:48.000000 audiostretchy-1.0.6/.github/workflows/compile-linux.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-01 00:36:48.000000 audiostretchy-1.0.6/.github/workflows/compile-mac.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-05-01 00:36:48.000000 audiostretchy-1.0.6/.github/workflows/compile-windows.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-05-01 00:36:48.000000 audiostretchy-1.0.6/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-01 00:36:48.000000 audiostretchy-1.0.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-01 00:36:48.000000 audiostretchy-1.0.6/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-01 00:36:48.000000 audiostretchy-1.0.6/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-05-01 00:36:48.000000 audiostretchy-1.0.6/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-01 00:36:48.000000 audiostretchy-1.0.6/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-01 00:36:48.000000 audiostretchy-1.0.6/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-05-01 00:36:48.000000 audiostretchy-1.0.6/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-05-01 00:36:59.728857 audiostretchy-1.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4521 2023-05-01 00:36:48.000000 audiostretchy-1.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:36:59.728857 audiostretchy-1.0.6/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-01 00:36:48.000000 audiostretchy-1.0.6/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:36:59.728857 audiostretchy-1.0.6/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-01 00:36:48.000000 audiostretchy-1.0.6/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-01 00:36:48.000000 audiostretchy-1.0.6/docs/authors.md
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-01 00:36:48.000000 audiostretchy-1.0.6/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (123)    10046 2023-05-01 00:36:48.000000 audiostretchy-1.0.6/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-01 00:36:48.000000 audiostretchy-1.0.6/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-01 00:36:48.000000 audiostretchy-1.0.6/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-01 00:36:48.000000 audiostretchy-1.0.6/docs/license.md
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-01 00:36:48.000000 audiostretchy-1.0.6/docs/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-01 00:36:48.000000 audiostretchy-1.0.6/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-01 00:36:48.000000 audiostretchy-1.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-05-01 00:36:59.732858 audiostretchy-1.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-01 00:36:48.000000 audiostretchy-1.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:36:59.724857 audiostretchy-1.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:36:59.728857 audiostretchy-1.0.6/src/audiostretchy/
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-01 00:36:48.000000 audiostretchy-1.0.6/src/audiostretchy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-01 00:36:48.000000 audiostretchy-1.0.6/src/audiostretchy/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:36:59.728857 audiostretchy-1.0.6/src/audiostretchy/interface/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:36:59.728857 audiostretchy-1.0.6/src/audiostretchy/interface/linux/
--rwxr-xr-x   0 runner    (1001) docker     (123)    22664 2023-05-01 00:36:48.000000 audiostretchy-1.0.6/src/audiostretchy/interface/linux/_stretch.so
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:36:59.728857 audiostretchy-1.0.6/src/audiostretchy/interface/mac/
--rwxr-xr-x   0 runner    (1001) docker     (123)    99483 2023-05-01 00:36:48.000000 audiostretchy-1.0.6/src/audiostretchy/interface/mac/_stretch.dylib
--rw-r--r--   0 runner    (1001) docker     (123)     6383 2023-05-01 00:36:48.000000 audiostretchy-1.0.6/src/audiostretchy/interface/stretch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:36:59.728857 audiostretchy-1.0.6/src/audiostretchy/interface/win/
--rw-r--r--   0 runner    (1001) docker     (123)   104960 2023-05-01 00:36:48.000000 audiostretchy-1.0.6/src/audiostretchy/interface/win/_stretch.dll
--rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-05-01 00:36:48.000000 audiostretchy-1.0.6/src/audiostretchy/stretch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:36:59.728857 audiostretchy-1.0.6/src/audiostretchy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-05-01 00:36:59.000000 audiostretchy-1.0.6/src/audiostretchy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-01 00:36:59.000000 audiostretchy-1.0.6/src/audiostretchy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 00:36:59.000000 audiostretchy-1.0.6/src/audiostretchy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-01 00:36:59.000000 audiostretchy-1.0.6/src/audiostretchy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 00:36:59.000000 audiostretchy-1.0.6/src/audiostretchy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-01 00:36:59.000000 audiostretchy-1.0.6/src/audiostretchy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-01 00:36:59.000000 audiostretchy-1.0.6/src/audiostretchy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:36:59.728857 audiostretchy-1.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-01 00:36:48.000000 audiostretchy-1.0.6/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:42:55.856718 audiostretchy-1.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-01 00:42:32.000000 audiostretchy-1.0.7/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:42:55.852718 audiostretchy-1.0.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:42:55.852718 audiostretchy-1.0.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-01 00:42:32.000000 audiostretchy-1.0.7/.github/workflows/compile-linux.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-01 00:42:32.000000 audiostretchy-1.0.7/.github/workflows/compile-mac.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-05-01 00:42:32.000000 audiostretchy-1.0.7/.github/workflows/compile-windows.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-05-01 00:42:32.000000 audiostretchy-1.0.7/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-01 00:42:32.000000 audiostretchy-1.0.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-01 00:42:32.000000 audiostretchy-1.0.7/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-01 00:42:32.000000 audiostretchy-1.0.7/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-05-01 00:42:32.000000 audiostretchy-1.0.7/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-01 00:42:32.000000 audiostretchy-1.0.7/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-01 00:42:32.000000 audiostretchy-1.0.7/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-05-01 00:42:32.000000 audiostretchy-1.0.7/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5115 2023-05-01 00:42:55.856718 audiostretchy-1.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4521 2023-05-01 00:42:32.000000 audiostretchy-1.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:42:55.856718 audiostretchy-1.0.7/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-01 00:42:32.000000 audiostretchy-1.0.7/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:42:55.856718 audiostretchy-1.0.7/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-01 00:42:32.000000 audiostretchy-1.0.7/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-01 00:42:32.000000 audiostretchy-1.0.7/docs/authors.md
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-01 00:42:32.000000 audiostretchy-1.0.7/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10046 2023-05-01 00:42:32.000000 audiostretchy-1.0.7/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-01 00:42:32.000000 audiostretchy-1.0.7/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-01 00:42:32.000000 audiostretchy-1.0.7/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-01 00:42:32.000000 audiostretchy-1.0.7/docs/license.md
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-01 00:42:32.000000 audiostretchy-1.0.7/docs/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-01 00:42:32.000000 audiostretchy-1.0.7/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-01 00:42:32.000000 audiostretchy-1.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-05-01 00:42:55.856718 audiostretchy-1.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-01 00:42:32.000000 audiostretchy-1.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:42:55.852718 audiostretchy-1.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:42:55.856718 audiostretchy-1.0.7/src/audiostretchy/
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-01 00:42:32.000000 audiostretchy-1.0.7/src/audiostretchy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-01 00:42:32.000000 audiostretchy-1.0.7/src/audiostretchy/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:42:55.856718 audiostretchy-1.0.7/src/audiostretchy/interface/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:42:55.856718 audiostretchy-1.0.7/src/audiostretchy/interface/linux/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22664 2023-05-01 00:42:32.000000 audiostretchy-1.0.7/src/audiostretchy/interface/linux/_stretch.so
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:42:55.856718 audiostretchy-1.0.7/src/audiostretchy/interface/mac/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    99483 2023-05-01 00:42:32.000000 audiostretchy-1.0.7/src/audiostretchy/interface/mac/_stretch.dylib
+-rw-r--r--   0 runner    (1001) docker     (123)     6383 2023-05-01 00:42:32.000000 audiostretchy-1.0.7/src/audiostretchy/interface/stretch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:42:55.856718 audiostretchy-1.0.7/src/audiostretchy/interface/win/
+-rw-r--r--   0 runner    (1001) docker     (123)   104960 2023-05-01 00:42:32.000000 audiostretchy-1.0.7/src/audiostretchy/interface/win/_stretch.dll
+-rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-05-01 00:42:32.000000 audiostretchy-1.0.7/src/audiostretchy/stretch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:42:55.856718 audiostretchy-1.0.7/src/audiostretchy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5115 2023-05-01 00:42:55.000000 audiostretchy-1.0.7/src/audiostretchy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-01 00:42:55.000000 audiostretchy-1.0.7/src/audiostretchy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 00:42:55.000000 audiostretchy-1.0.7/src/audiostretchy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-01 00:42:55.000000 audiostretchy-1.0.7/src/audiostretchy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 00:42:55.000000 audiostretchy-1.0.7/src/audiostretchy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-01 00:42:55.000000 audiostretchy-1.0.7/src/audiostretchy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-01 00:42:55.000000 audiostretchy-1.0.7/src/audiostretchy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:42:55.856718 audiostretchy-1.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-01 00:42:32.000000 audiostretchy-1.0.7/tests/conftest.py
```

### Comparing `audiostretchy-1.0.6/.coveragerc` & `audiostretchy-1.0.7/.coveragerc`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.0.6/.github/workflows/compile-linux.yaml` & `audiostretchy-1.0.7/.github/workflows/compile-linux.yaml`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.0.6/.github/workflows/compile-mac.yaml` & `audiostretchy-1.0.7/.github/workflows/compile-mac.yaml`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.0.6/.github/workflows/compile-windows.yaml` & `audiostretchy-1.0.7/.github/workflows/compile-windows.yaml`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.0.6/.github/workflows/publish.yaml` & `audiostretchy-1.0.7/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.0.6/.gitignore` & `audiostretchy-1.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.0.6/.pre-commit-config.yaml` & `audiostretchy-1.0.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.0.6/.readthedocs.yml` & `audiostretchy-1.0.7/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.0.6/LICENSE.txt` & `audiostretchy-1.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.0.6/PKG-INFO` & `audiostretchy-1.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
 Name: audiostretchy
-Version: 1.0.6
-Summary: Add a short description here!
+Version: 1.0.7
+Summary: Wrapper around the audio-stretch C library to time-stretch WAV files without changing their pitch
 Home-page: https://github.com/twardoch/audiostretchy
-Author: twardoch
-Author-email: adam@twardoch.com
+Author: Adam Twardoch
+Author-email: adam+github@twardoch.com
 License: BSD-3-Clause
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Provides-Extra: testing
 License-File: LICENSE.txt
 
 # AudioStretchy
 
 AudioStretchy is a Python library that allows you to time-stretch audio signals without changing their pitch. It is a wrapper around the [audio-stretch](https://github.com/dbry/audio-stretch) library by David Bryant, which implements a sophisticated time-stretching algorithm for high-quality results. 
 
-Version: 1.0.5
+Version: 1.0.7
 
 ## Features
 
 - Time stretching of audio files without changing their pitch
 - Supports WAV files
 - Adjustable stretching ratio from 0.25 to 4.0
 - Cross-platform: Windows, macOS, and Linux
```

### Comparing `audiostretchy-1.0.6/README.md` & `audiostretchy-1.0.7/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # AudioStretchy
 
 AudioStretchy is a Python library that allows you to time-stretch audio signals without changing their pitch. It is a wrapper around the [audio-stretch](https://github.com/dbry/audio-stretch) library by David Bryant, which implements a sophisticated time-stretching algorithm for high-quality results. 
 
-Version: 1.0.5
+Version: 1.0.7
 
 ## Features
 
 - Time stretching of audio files without changing their pitch
 - Supports WAV files
 - Adjustable stretching ratio from 0.25 to 4.0
 - Cross-platform: Windows, macOS, and Linux
```

### Comparing `audiostretchy-1.0.6/docs/Makefile` & `audiostretchy-1.0.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.0.6/docs/conf.py` & `audiostretchy-1.0.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.0.6/docs/index.md` & `audiostretchy-1.0.7/docs/index.md`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.0.6/setup.cfg` & `audiostretchy-1.0.7/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [metadata]
 name = audiostretchy
-description = Add a short description here!
-author = twardoch
-author_email = adam@twardoch.com
+description = Wrapper around the audio-stretch C library to time-stretch WAV files without changing their pitch
+author = Adam Twardoch
+author_email = adam+github@twardoch.com
 license = BSD-3-Clause
 license_files = LICENSE.txt
 long_description = file: README.md
 long_description_content_type = text/markdown; charset=UTF-8; variant=GFM
 url = https://github.com/twardoch/audiostretchy
 project_urls = 
 	Documentation = https://pyscaffold.org/
@@ -17,14 +17,15 @@
 
 [options]
 zip_safe = False
 packages = find_namespace:
 include_package_data = True
 package_dir = 
 	=src
+python_requires = >=3.8
 install_requires = 
 	importlib-metadata; python_version<"3.8"
 	fire>=0.5.0
 	numpy>=1.23.0
 
 [options.packages.find]
 where = src
```

### Comparing `audiostretchy-1.0.6/setup.py` & `audiostretchy-1.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.0.6/src/audiostretchy/__init__.py` & `audiostretchy-1.0.7/src/audiostretchy/__init__.py`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.0.6/src/audiostretchy/interface/linux/_stretch.so` & `audiostretchy-1.0.7/src/audiostretchy/interface/linux/_stretch.so`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.0.6/src/audiostretchy/interface/mac/_stretch.dylib` & `audiostretchy-1.0.7/src/audiostretchy/interface/mac/_stretch.dylib`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.0.6/src/audiostretchy/interface/stretch.py` & `audiostretchy-1.0.7/src/audiostretchy/interface/stretch.py`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.0.6/src/audiostretchy/interface/win/_stretch.dll` & `audiostretchy-1.0.7/src/audiostretchy/interface/win/_stretch.dll`

 * *Files 0% similar despite different names*

#### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x00000001800014d4
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Mon May  1 00:29:30 2023
+Time/Date		Mon May  1 00:34:11 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	34
 SizeOfCode		000000000000da00
 SizeOfInitializedData	000000000000ce00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000000014d4
@@ -30758,16 +30758,15 @@
    18001691d:	add    %al,(%rax)
    18001691f:	add    %dh,-0xe(%rax)
    180016922:	add    %al,0x1(%rax)
    180016928:	js     0x18001691c
    18001692a:	add    %al,0x1(%rax)
    180016930:	add    %al,(%rax)
    180016932:	add    %al,(%rax)
-   180016934:	(bad)
-   180016935:	(bad)
+   180016934:	add    (%rcx),%ecx
    180016936:	rex.WRXB
    180016937:	add    %al,%fs:(%rax)
    18001693a:	add    %al,(%rax)
    18001693c:	or     $0xb8000000,%eax
    180016941:	add    (%rax),%al
    180016943:	add    %ch,%al
    180016945:	insb   (%dx),%es:(%rdi)
```

### Comparing `audiostretchy-1.0.6/src/audiostretchy/stretch.py` & `audiostretchy-1.0.7/src/audiostretchy/stretch.py`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.0.6/src/audiostretchy.egg-info/PKG-INFO` & `audiostretchy-1.0.7/src/audiostretchy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
 Name: audiostretchy
-Version: 1.0.6
-Summary: Add a short description here!
+Version: 1.0.7
+Summary: Wrapper around the audio-stretch C library to time-stretch WAV files without changing their pitch
 Home-page: https://github.com/twardoch/audiostretchy
-Author: twardoch
-Author-email: adam@twardoch.com
+Author: Adam Twardoch
+Author-email: adam+github@twardoch.com
 License: BSD-3-Clause
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Provides-Extra: testing
 License-File: LICENSE.txt
 
 # AudioStretchy
 
 AudioStretchy is a Python library that allows you to time-stretch audio signals without changing their pitch. It is a wrapper around the [audio-stretch](https://github.com/dbry/audio-stretch) library by David Bryant, which implements a sophisticated time-stretching algorithm for high-quality results. 
 
-Version: 1.0.5
+Version: 1.0.7
 
 ## Features
 
 - Time stretching of audio files without changing their pitch
 - Supports WAV files
 - Adjustable stretching ratio from 0.25 to 4.0
 - Cross-platform: Windows, macOS, and Linux
```

### Comparing `audiostretchy-1.0.6/src/audiostretchy.egg-info/SOURCES.txt` & `audiostretchy-1.0.7/src/audiostretchy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

