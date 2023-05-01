# Comparing `tmp/malbench-0.3.2.tar.gz` & `tmp/malbench-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "malbench-0.3.2.tar", max compression
+gzip compressed data, was "malbench-0.3.3.tar", max compression
```

## Comparing `malbench-0.3.2.tar` & `malbench-0.3.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      545 2023-04-13 19:49:08.177178 malbench-0.3.2/data/banner.txt
--rw-r--r--   0        0        0      508 2023-04-25 12:39:55.627552 malbench-0.3.2/data/disclaimer.txt
--rw-r--r--   0        0        0        5 2023-05-01 04:55:31.656629 malbench-0.3.2/data/version.txt
--rw-r--r--   0        0        0    35803 2023-04-02 22:37:30.790768 malbench-0.3.2/LICENSE
--rw-r--r--   0        0        0        0 2023-04-02 12:57:46.205523 malbench-0.3.2/malbench/__init__.py
--rw-r--r--   0        0        0     2905 2023-04-27 03:15:45.560814 malbench-0.3.2/malbench/__main__.py
--rw-r--r--   0        0        0     4941 2023-04-27 03:46:07.566126 malbench-0.3.2/malbench/args.py
--rw-r--r--   0        0        0     4830 2023-04-26 15:12:59.929156 malbench-0.3.2/malbench/malware.py
--rw-r--r--   0        0        0     8362 2023-04-27 03:29:38.237716 malbench-0.3.2/malbench/message.py
--rw-r--r--   0        0        0      435 2023-04-21 13:20:47.394154 malbench-0.3.2/malbench/version.py
--rw-r--r--   0        0        0      894 2023-05-01 04:55:40.662999 malbench-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     7144 2023-05-01 04:55:05.817341 malbench-0.3.2/README.md
--rw-r--r--   0        0        0     7870 1970-01-01 00:00:00.000000 malbench-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0      545 2023-04-13 19:49:08.177178 malbench-0.3.3/data/banner.txt
+-rw-r--r--   0        0        0      508 2023-04-25 12:39:55.627552 malbench-0.3.3/data/disclaimer.txt
+-rw-r--r--   0        0        0        5 2023-05-01 12:47:17.593190 malbench-0.3.3/data/version.txt
+-rw-r--r--   0        0        0    35803 2023-04-02 22:37:30.790768 malbench-0.3.3/LICENSE
+-rw-r--r--   0        0        0        0 2023-04-02 12:57:46.205523 malbench-0.3.3/malbench/__init__.py
+-rw-r--r--   0        0        0     2905 2023-04-27 03:15:45.560814 malbench-0.3.3/malbench/__main__.py
+-rw-r--r--   0        0        0     4941 2023-04-27 03:46:07.566126 malbench-0.3.3/malbench/args.py
+-rw-r--r--   0        0        0     4830 2023-04-26 15:12:59.929156 malbench-0.3.3/malbench/malware.py
+-rw-r--r--   0        0        0     8362 2023-04-27 03:29:38.237716 malbench-0.3.3/malbench/message.py
+-rw-r--r--   0        0        0      435 2023-04-21 13:20:47.394154 malbench-0.3.3/malbench/version.py
+-rw-r--r--   0        0        0      892 2023-05-01 12:47:25.525781 malbench-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     7144 2023-05-01 04:55:05.817341 malbench-0.3.3/README.md
+-rw-r--r--   0        0        0     7896 1970-01-01 00:00:00.000000 malbench-0.3.3/PKG-INFO
```

### Comparing `malbench-0.3.2/data/banner.txt` & `malbench-0.3.3/data/banner.txt`

 * *Files identical despite different names*

### Comparing `malbench-0.3.2/LICENSE` & `malbench-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `malbench-0.3.2/malbench/__main__.py` & `malbench-0.3.3/malbench/__main__.py`

 * *Files identical despite different names*

### Comparing `malbench-0.3.2/malbench/args.py` & `malbench-0.3.3/malbench/args.py`

 * *Files identical despite different names*

### Comparing `malbench-0.3.2/malbench/malware.py` & `malbench-0.3.3/malbench/malware.py`

 * *Files identical despite different names*

### Comparing `malbench-0.3.2/malbench/message.py` & `malbench-0.3.3/malbench/message.py`

 * *Files identical despite different names*

### Comparing `malbench-0.3.2/pyproject.toml` & `malbench-0.3.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [tool.poetry]
 name = "malbench"
-version = "0.3.2"
-description = "A tool used for automating the analysis of malware samples against antivirus solutions."
+version = "0.3.3"
+description = "A tool used to benchmark antivirus solutions against real-world malware samples."
 repository = "https://github.com/youkergav/Malbench"
 authors = ["Gavin Youker <youkergav@gmail.com>"]
 readme = "README.md"
-license = "LICENSE"
+license = "GPL-3.0-only"
 include = ["data/*"]
 exclude = ["data/samples"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 colorama = "^0.4.6"
 toml = "^0.10.2"
```

### Comparing `malbench-0.3.2/README.md` & `malbench-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `malbench-0.3.2/PKG-INFO` & `malbench-0.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: malbench
-Version: 0.3.2
-Summary: A tool used for automating the analysis of malware samples against antivirus solutions.
+Version: 0.3.3
+Summary: A tool used to benchmark antivirus solutions against real-world malware samples.
 Home-page: https://github.com/youkergav/Malbench
-License: LICENSE
+License: GPL-3.0-only
 Author: Gavin Youker
 Author-email: youkergav@gmail.com
 Requires-Python: >=3.10,<4.0
-Classifier: License :: Other/Proprietary License
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: colorama (>=0.4.6,<0.5.0)
 Requires-Dist: holidays (>=0.22,<0.23)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
```

