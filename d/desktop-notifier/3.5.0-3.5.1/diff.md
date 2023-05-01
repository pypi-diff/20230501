# Comparing `tmp/desktop-notifier-3.5.0.tar.gz` & `tmp/desktop-notifier-3.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "desktop-notifier-3.5.0.tar", last modified: Mon May  1 18:29:37 2023, max compression
+gzip compressed data, was "desktop-notifier-3.5.1.tar", last modified: Mon May  1 19:36:45 2023, max compression
```

## Comparing `desktop-notifier-3.5.0.tar` & `desktop-notifier-3.5.1.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:29:37.212569 desktop-notifier-3.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-01 18:29:19.000000 desktop-notifier-3.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8333 2023-05-01 18:29:37.212569 desktop-notifier-3.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7383 2023-05-01 18:29:19.000000 desktop-notifier-3.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-05-01 18:29:19.000000 desktop-notifier-3.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 18:29:37.212569 desktop-notifier-3.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:29:37.208568 desktop-notifier-3.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:29:37.212569 desktop-notifier-3.5.0/src/desktop_notifier/
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-01 18:29:19.000000 desktop-notifier-3.5.0/src/desktop_notifier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10614 2023-05-01 18:29:19.000000 desktop-notifier-3.5.0/src/desktop_notifier/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7660 2023-05-01 18:29:19.000000 desktop-notifier-3.5.0/src/desktop_notifier/dbus.py
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-05-01 18:29:19.000000 desktop-notifier-3.5.0/src/desktop_notifier/dummy.py
--rw-r--r--   0 runner    (1001) docker     (123)    14980 2023-05-01 18:29:19.000000 desktop-notifier-3.5.0/src/desktop_notifier/macos.py
--rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-05-01 18:29:19.000000 desktop-notifier-3.5.0/src/desktop_notifier/macos_legacy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-05-01 18:29:19.000000 desktop-notifier-3.5.0/src/desktop_notifier/macos_support.py
--rw-r--r--   0 runner    (1001) docker     (123)    12931 2023-05-01 18:29:19.000000 desktop-notifier-3.5.0/src/desktop_notifier/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:29:37.212569 desktop-notifier-3.5.0/src/desktop_notifier/resources/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-01 18:29:19.000000 desktop-notifier-3.5.0/src/desktop_notifier/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9356 2023-05-01 18:29:19.000000 desktop-notifier-3.5.0/src/desktop_notifier/winrt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:29:37.212569 desktop-notifier-3.5.0/src/desktop_notifier.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8333 2023-05-01 18:29:37.000000 desktop-notifier-3.5.0/src/desktop_notifier.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-01 18:29:37.000000 desktop-notifier-3.5.0/src/desktop_notifier.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 18:29:37.000000 desktop-notifier-3.5.0/src/desktop_notifier.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-01 18:29:37.000000 desktop-notifier-3.5.0/src/desktop_notifier.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-01 18:29:37.000000 desktop-notifier-3.5.0/src/desktop_notifier.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:36:45.545543 desktop-notifier-3.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-01 19:36:31.000000 desktop-notifier-3.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8333 2023-05-01 19:36:45.545543 desktop-notifier-3.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7383 2023-05-01 19:36:31.000000 desktop-notifier-3.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-05-01 19:36:31.000000 desktop-notifier-3.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 19:36:45.545543 desktop-notifier-3.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:36:45.545543 desktop-notifier-3.5.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:36:45.545543 desktop-notifier-3.5.1/src/desktop_notifier/
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-01 19:36:31.000000 desktop-notifier-3.5.1/src/desktop_notifier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10614 2023-05-01 19:36:31.000000 desktop-notifier-3.5.1/src/desktop_notifier/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7660 2023-05-01 19:36:31.000000 desktop-notifier-3.5.1/src/desktop_notifier/dbus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-05-01 19:36:31.000000 desktop-notifier-3.5.1/src/desktop_notifier/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14980 2023-05-01 19:36:31.000000 desktop-notifier-3.5.1/src/desktop_notifier/macos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-05-01 19:36:31.000000 desktop-notifier-3.5.1/src/desktop_notifier/macos_legacy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-05-01 19:36:31.000000 desktop-notifier-3.5.1/src/desktop_notifier/macos_support.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12931 2023-05-01 19:36:31.000000 desktop-notifier-3.5.1/src/desktop_notifier/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:36:45.545543 desktop-notifier-3.5.1/src/desktop_notifier/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-01 19:36:31.000000 desktop-notifier-3.5.1/src/desktop_notifier/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-05-01 19:36:31.000000 desktop-notifier-3.5.1/src/desktop_notifier/resources/python.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9356 2023-05-01 19:36:31.000000 desktop-notifier-3.5.1/src/desktop_notifier/winrt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:36:45.545543 desktop-notifier-3.5.1/src/desktop_notifier.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8333 2023-05-01 19:36:45.000000 desktop-notifier-3.5.1/src/desktop_notifier.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-01 19:36:45.000000 desktop-notifier-3.5.1/src/desktop_notifier.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 19:36:45.000000 desktop-notifier-3.5.1/src/desktop_notifier.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-01 19:36:45.000000 desktop-notifier-3.5.1/src/desktop_notifier.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-01 19:36:45.000000 desktop-notifier-3.5.1/src/desktop_notifier.egg-info/top_level.txt
```

### Comparing `desktop-notifier-3.5.0/LICENSE` & `desktop-notifier-3.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `desktop-notifier-3.5.0/PKG-INFO` & `desktop-notifier-3.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: desktop-notifier
-Version: 3.5.0
+Version: 3.5.1
 Summary: Python library for cross-platform desktop notifications
 Author-email: Sam Schott <sam.schott@outlook.com>
 License: MIT
 Project-URL: Homepage, https://github.com/samschott/desktop-notifier
 Keywords: desktop-notifier
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `desktop-notifier-3.5.0/README.md` & `desktop-notifier-3.5.1/README.md`

 * *Files identical despite different names*

### Comparing `desktop-notifier-3.5.0/pyproject.toml` & `desktop-notifier-3.5.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.2", "build"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "desktop-notifier"
-version = "3.5.0"
+version = "3.5.1"
 authors = [{name = "Sam Schott", email = "sam.schott@outlook.com"}]
 license = {text = "MIT"}
 description = "Python library for cross-platform desktop notifications"
 keywords = ["desktop-notifier"]
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Intended Audience :: Developers",
@@ -52,14 +52,17 @@
 docs = [
     "sphinx",
     "sphinx-autoapi",
     "sphinx-mdinclude",
     "sphinx_rtd_theme",
 ]
 
+[tool.setuptools.package-data]
+desktop_notifier = ["**/*.png"]
+
 [tool.flake8]
 ignore = "E203,E501,W503,H306"
 per-file-ignores = """
 __init__.py: F401"""
 statistics = "True"
 
 [tool.mypy]
```

### Comparing `desktop-notifier-3.5.0/src/desktop_notifier/base.py` & `desktop-notifier-3.5.1/src/desktop_notifier/base.py`

 * *Files identical despite different names*

### Comparing `desktop-notifier-3.5.0/src/desktop_notifier/dbus.py` & `desktop-notifier-3.5.1/src/desktop_notifier/dbus.py`

 * *Files identical despite different names*

### Comparing `desktop-notifier-3.5.0/src/desktop_notifier/dummy.py` & `desktop-notifier-3.5.1/src/desktop_notifier/dummy.py`

 * *Files identical despite different names*

### Comparing `desktop-notifier-3.5.0/src/desktop_notifier/macos.py` & `desktop-notifier-3.5.1/src/desktop_notifier/macos.py`

 * *Files identical despite different names*

### Comparing `desktop-notifier-3.5.0/src/desktop_notifier/macos_legacy.py` & `desktop-notifier-3.5.1/src/desktop_notifier/macos_legacy.py`

 * *Files identical despite different names*

### Comparing `desktop-notifier-3.5.0/src/desktop_notifier/macos_support.py` & `desktop-notifier-3.5.1/src/desktop_notifier/macos_support.py`

 * *Files identical despite different names*

### Comparing `desktop-notifier-3.5.0/src/desktop_notifier/main.py` & `desktop-notifier-3.5.1/src/desktop_notifier/main.py`

 * *Files identical despite different names*

### Comparing `desktop-notifier-3.5.0/src/desktop_notifier/winrt.py` & `desktop-notifier-3.5.1/src/desktop_notifier/winrt.py`

 * *Files identical despite different names*

### Comparing `desktop-notifier-3.5.0/src/desktop_notifier.egg-info/PKG-INFO` & `desktop-notifier-3.5.1/src/desktop_notifier.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: desktop-notifier
-Version: 3.5.0
+Version: 3.5.1
 Summary: Python library for cross-platform desktop notifications
 Author-email: Sam Schott <sam.schott@outlook.com>
 License: MIT
 Project-URL: Homepage, https://github.com/samschott/desktop-notifier
 Keywords: desktop-notifier
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `desktop-notifier-3.5.0/src/desktop_notifier.egg-info/SOURCES.txt` & `desktop-notifier-3.5.1/src/desktop_notifier.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -11,8 +11,9 @@
 src/desktop_notifier/main.py
 src/desktop_notifier/winrt.py
 src/desktop_notifier.egg-info/PKG-INFO
 src/desktop_notifier.egg-info/SOURCES.txt
 src/desktop_notifier.egg-info/dependency_links.txt
 src/desktop_notifier.egg-info/requires.txt
 src/desktop_notifier.egg-info/top_level.txt
-src/desktop_notifier/resources/__init__.py
+src/desktop_notifier/resources/__init__.py
+src/desktop_notifier/resources/python.png
```

