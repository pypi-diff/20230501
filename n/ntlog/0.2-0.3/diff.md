# Comparing `tmp/ntlog-0.2.tar.gz` & `tmp/ntlog-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ntlog-0.2.tar", last modified: Mon Apr 10 19:32:45 2023, max compression
+gzip compressed data, was "ntlog-0.3.tar", last modified: Mon May  1 17:46:48 2023, max compression
```

## Comparing `ntlog-0.2.tar` & `ntlog-0.3.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0     3212 2023-04-10 19:29:29.805965 ntlog-0.2/README.rst
--rw-r--r--   0        0        0        0 2023-04-07 19:25:16.421568 ntlog-0.2/ntlog/__init__.py
--rwxr-xr-x   0        0        0     4011 2023-04-10 19:29:29.804965 ntlog-0.2/ntlog/main.py
--rw-r--r--   0        0        0     1113 2023-04-10 19:29:29.805965 ntlog-0.2/pyproject.toml
--rw-r--r--   0        0        0     4187 1970-01-01 00:00:00.000000 ntlog-0.2/PKG-INFO
+-rw-r--r--   0        0        0     6720 2023-05-01 17:46:11.353194 ntlog-0.3/README.rst
+-rw-r--r--   0        0        0       46 2023-05-01 02:29:53.042664 ntlog-0.3/ntlog/__init__.py
+-rw-r--r--   0        0        0     2024 2023-05-01 17:24:58.419825 ntlog-0.3/ntlog/main.py
+-rw-r--r--   0        0        0     8236 2023-05-01 17:04:25.054181 ntlog-0.3/ntlog/ntlog.py
+-rw-r--r--   0        0        0     1113 2023-05-01 17:24:58.419825 ntlog-0.3/pyproject.toml
+-rw-r--r--   0        0        0     7695 1970-01-01 00:00:00.000000 ntlog-0.3/PKG-INFO
```

### Comparing `ntlog-0.2/pyproject.toml` & `ntlog-0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ntlog"
-version = "0.2"
+version = "0.3"
 description = "Append a log file to an running NestedText log"
 readme = "README.rst"
 keywords = ["nestedtext", "logging"]
 authors = [
     {name = "Ken Kundert"},
 ]
 requires-python = ">=3.6"
```

