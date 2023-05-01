# Comparing `tmp/fstflowchat-0.0.3.tar.gz` & `tmp/fstflowchat-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fstflowchat-0.0.3.tar", last modified: Mon Apr 24 01:51:25 2023, max compression
+gzip compressed data, was "fstflowchat-0.0.4.tar", last modified: Mon May  1 02:51:33 2023, max compression
```

## Comparing `fstflowchat-0.0.3.tar` & `fstflowchat-0.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 kaze7539   (503) staff       (20)        0 2023-04-24 01:51:25.436050 fstflowchat-0.0.3/
--rw-r--r--   0 kaze7539   (503) staff       (20)     1071 2023-04-19 21:48:08.000000 fstflowchat-0.0.3/LICENSE
--rw-r--r--   0 kaze7539   (503) staff       (20)       28 2023-04-24 01:28:18.000000 fstflowchat-0.0.3/MANIFEST.in
--rw-r--r--   0 kaze7539   (503) staff       (20)     2614 2023-04-24 01:51:25.435694 fstflowchat-0.0.3/PKG-INFO
--rw-r--r--   0 kaze7539   (503) staff       (20)     1473 2023-04-24 00:59:35.000000 fstflowchat-0.0.3/README.md
--rw-r--r--   0 kaze7539   (503) staff       (20)       38 2023-04-24 01:51:25.436110 fstflowchat-0.0.3/setup.cfg
--rwxr-xr-x   0 kaze7539   (503) staff       (20)     8191 2023-04-24 01:43:27.000000 fstflowchat-0.0.3/setup.py
-drwxr-xr-x   0 kaze7539   (503) staff       (20)        0 2023-04-24 01:51:25.418104 fstflowchat-0.0.3/src/
-drwxr-xr-x   0 kaze7539   (503) staff       (20)        0 2023-04-24 01:51:25.427195 fstflowchat-0.0.3/src/fstflowchat/
--rw-r--r--   0 kaze7539   (503) staff       (20)        0 2023-04-24 01:05:43.000000 fstflowchat-0.0.3/src/fstflowchat/__init__.py
--rw-r--r--   0 kaze7539   (503) staff       (20)     7200 2023-04-24 01:50:56.000000 fstflowchat-0.0.3/src/fstflowchat/example.py
--rw-r--r--   0 kaze7539   (503) staff       (20)      795 2023-04-23 23:37:09.000000 fstflowchat-0.0.3/src/fstflowchat/quiz.dot
-drwxr-xr-x   0 kaze7539   (503) staff       (20)        0 2023-04-24 01:51:25.435243 fstflowchat-0.0.3/src/fstflowchat.egg-info/
--rw-r--r--   0 kaze7539   (503) staff       (20)     2614 2023-04-24 01:51:25.000000 fstflowchat-0.0.3/src/fstflowchat.egg-info/PKG-INFO
--rw-r--r--   0 kaze7539   (503) staff       (20)      354 2023-04-24 01:51:25.000000 fstflowchat-0.0.3/src/fstflowchat.egg-info/SOURCES.txt
--rw-r--r--   0 kaze7539   (503) staff       (20)        1 2023-04-24 01:51:25.000000 fstflowchat-0.0.3/src/fstflowchat.egg-info/dependency_links.txt
--rw-r--r--   0 kaze7539   (503) staff       (20)       65 2023-04-24 01:51:25.000000 fstflowchat-0.0.3/src/fstflowchat.egg-info/entry_points.txt
--rw-r--r--   0 kaze7539   (503) staff       (20)       11 2023-04-24 01:51:25.000000 fstflowchat-0.0.3/src/fstflowchat.egg-info/requires.txt
--rw-r--r--   0 kaze7539   (503) staff       (20)       12 2023-04-24 01:51:25.000000 fstflowchat-0.0.3/src/fstflowchat.egg-info/top_level.txt
+drwxr-xr-x   0 kaze7539   (503) staff       (20)        0 2023-05-01 02:51:33.153457 fstflowchat-0.0.4/
+-rw-r--r--   0 kaze7539   (503) staff       (20)     1071 2023-04-19 21:48:08.000000 fstflowchat-0.0.4/LICENSE
+-rw-r--r--   0 kaze7539   (503) staff       (20)       28 2023-04-24 01:28:18.000000 fstflowchat-0.0.4/MANIFEST.in
+-rw-r--r--   0 kaze7539   (503) staff       (20)     2614 2023-05-01 02:51:33.152054 fstflowchat-0.0.4/PKG-INFO
+-rw-r--r--   0 kaze7539   (503) staff       (20)     1473 2023-04-24 00:59:35.000000 fstflowchat-0.0.4/README.md
+-rw-r--r--   0 kaze7539   (503) staff       (20)       38 2023-05-01 02:51:33.153541 fstflowchat-0.0.4/setup.cfg
+-rwxr-xr-x   0 kaze7539   (503) staff       (20)     8191 2023-05-01 02:51:17.000000 fstflowchat-0.0.4/setup.py
+drwxr-xr-x   0 kaze7539   (503) staff       (20)        0 2023-05-01 02:51:33.131041 fstflowchat-0.0.4/src/
+drwxr-xr-x   0 kaze7539   (503) staff       (20)        0 2023-05-01 02:51:33.137597 fstflowchat-0.0.4/src/fstflowchat/
+-rw-r--r--   0 kaze7539   (503) staff       (20)     4007 2023-05-01 02:29:33.000000 fstflowchat-0.0.4/src/fstflowchat/__init__.py
+-rw-r--r--   0 kaze7539   (503) staff       (20)     7200 2023-04-24 01:50:56.000000 fstflowchat-0.0.4/src/fstflowchat/example.py
+-rw-r--r--   0 kaze7539   (503) staff       (20)      795 2023-04-23 23:37:09.000000 fstflowchat-0.0.4/src/fstflowchat/quiz.dot
+drwxr-xr-x   0 kaze7539   (503) staff       (20)        0 2023-05-01 02:51:33.149797 fstflowchat-0.0.4/src/fstflowchat.egg-info/
+-rw-r--r--   0 kaze7539   (503) staff       (20)     2614 2023-05-01 02:51:33.000000 fstflowchat-0.0.4/src/fstflowchat.egg-info/PKG-INFO
+-rw-r--r--   0 kaze7539   (503) staff       (20)      354 2023-05-01 02:51:33.000000 fstflowchat-0.0.4/src/fstflowchat.egg-info/SOURCES.txt
+-rw-r--r--   0 kaze7539   (503) staff       (20)        1 2023-05-01 02:51:33.000000 fstflowchat-0.0.4/src/fstflowchat.egg-info/dependency_links.txt
+-rw-r--r--   0 kaze7539   (503) staff       (20)       65 2023-05-01 02:51:33.000000 fstflowchat-0.0.4/src/fstflowchat.egg-info/entry_points.txt
+-rw-r--r--   0 kaze7539   (503) staff       (20)       11 2023-05-01 02:51:33.000000 fstflowchat-0.0.4/src/fstflowchat.egg-info/requires.txt
+-rw-r--r--   0 kaze7539   (503) staff       (20)       12 2023-05-01 02:51:33.000000 fstflowchat-0.0.4/src/fstflowchat.egg-info/top_level.txt
```

### Comparing `fstflowchat-0.0.3/LICENSE` & `fstflowchat-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `fstflowchat-0.0.3/PKG-INFO` & `fstflowchat-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fstflowchat
-Version: 0.0.3
+Version: 0.0.4
 Summary: a small, pedagogical, fst-based dialog toolkit.
 Home-page: https://fstflowchat.readthedocs.io/en/latest/
 Author: Abe Kazemzadeh
 Project-URL: Bug Reports, https://github.com/abecode/fstflowchat/issues
 Project-URL: Funding, https://donate.pypi.org
 Project-URL: Say Thanks!, http://saythanks.io/to/example
 Project-URL: Source, https://github.com/abecode/fstflowchat/issues
```

### Comparing `fstflowchat-0.0.3/README.md` & `fstflowchat-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `fstflowchat-0.0.3/setup.py` & `fstflowchat-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/guides/single-sourcing-package-version/
-    version="0.0.3",  # Required
+    version="0.0.4",  # Required
     
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description="a small, pedagogical, fst-based dialog toolkit.",  # Optional
     
     # This is an optional longer description of your project that represents
```

### Comparing `fstflowchat-0.0.3/src/fstflowchat/example.py` & `fstflowchat-0.0.4/src/fstflowchat/example.py`

 * *Files identical despite different names*

### Comparing `fstflowchat-0.0.3/src/fstflowchat/quiz.dot` & `fstflowchat-0.0.4/src/fstflowchat/quiz.dot`

 * *Files identical despite different names*

### Comparing `fstflowchat-0.0.3/src/fstflowchat.egg-info/PKG-INFO` & `fstflowchat-0.0.4/src/fstflowchat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fstflowchat
-Version: 0.0.3
+Version: 0.0.4
 Summary: a small, pedagogical, fst-based dialog toolkit.
 Home-page: https://fstflowchat.readthedocs.io/en/latest/
 Author: Abe Kazemzadeh
 Project-URL: Bug Reports, https://github.com/abecode/fstflowchat/issues
 Project-URL: Funding, https://donate.pypi.org
 Project-URL: Say Thanks!, http://saythanks.io/to/example
 Project-URL: Source, https://github.com/abecode/fstflowchat/issues
```

