# Comparing `tmp/malbench-0.3.0.tar.gz` & `tmp/malbench-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "malbench-0.3.0.tar", max compression
+gzip compressed data, was "malbench-0.3.1.tar", max compression
```

## Comparing `malbench-0.3.0.tar` & `malbench-0.3.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      545 2023-04-13 19:49:08.177178 malbench-0.3.0/data/banner.txt
--rw-r--r--   0        0        0      508 2023-04-25 12:39:55.627552 malbench-0.3.0/data/disclaimer.txt
--rw-r--r--   0        0        0        5 2023-04-26 12:10:15.326042 malbench-0.3.0/data/version.txt
--rw-r--r--   0        0        0    35803 2023-04-02 22:37:30.790768 malbench-0.3.0/LICENSE.md
--rw-r--r--   0        0        0        0 2023-04-02 12:57:46.205523 malbench-0.3.0/malbench/__init__.py
--rw-r--r--   0        0        0     2905 2023-04-27 03:15:45.560814 malbench-0.3.0/malbench/__main__.py
--rw-r--r--   0        0        0     4941 2023-04-27 03:46:07.566126 malbench-0.3.0/malbench/args.py
--rw-r--r--   0        0        0     4830 2023-04-26 15:12:59.929156 malbench-0.3.0/malbench/malware.py
--rw-r--r--   0        0        0     8362 2023-04-27 03:29:38.237716 malbench-0.3.0/malbench/message.py
--rw-r--r--   0        0        0      435 2023-04-21 13:20:47.394154 malbench-0.3.0/malbench/version.py
--rw-r--r--   0        0        0      819 2023-04-26 12:10:10.149945 malbench-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     6927 2023-04-27 03:47:54.949752 malbench-0.3.0/README.md
--rw-r--r--   0        0        0     7480 1970-01-01 00:00:00.000000 malbench-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      545 2023-04-13 19:49:08.177178 malbench-0.3.1/data/banner.txt
+-rw-r--r--   0        0        0      508 2023-04-25 12:39:55.627552 malbench-0.3.1/data/disclaimer.txt
+-rw-r--r--   0        0        0        5 2023-05-01 04:29:10.898528 malbench-0.3.1/data/version.txt
+-rw-r--r--   0        0        0    35803 2023-04-02 22:37:30.790768 malbench-0.3.1/LICENSE
+-rw-r--r--   0        0        0        0 2023-04-02 12:57:46.205523 malbench-0.3.1/malbench/__init__.py
+-rw-r--r--   0        0        0     2905 2023-04-27 03:15:45.560814 malbench-0.3.1/malbench/__main__.py
+-rw-r--r--   0        0        0     4941 2023-04-27 03:46:07.566126 malbench-0.3.1/malbench/args.py
+-rw-r--r--   0        0        0     4830 2023-04-26 15:12:59.929156 malbench-0.3.1/malbench/malware.py
+-rw-r--r--   0        0        0     8362 2023-04-27 03:29:38.237716 malbench-0.3.1/malbench/message.py
+-rw-r--r--   0        0        0      435 2023-04-21 13:20:47.394154 malbench-0.3.1/malbench/version.py
+-rw-r--r--   0        0        0      894 2023-05-01 04:32:12.652571 malbench-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     6927 2023-04-27 03:47:54.949752 malbench-0.3.1/README.md
+-rw-r--r--   0        0        0     7658 1970-01-01 00:00:00.000000 malbench-0.3.1/PKG-INFO
```

### Comparing `malbench-0.3.0/data/banner.txt` & `malbench-0.3.1/data/banner.txt`

 * *Files identical despite different names*

### Comparing `malbench-0.3.0/LICENSE.md` & `malbench-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `malbench-0.3.0/malbench/__main__.py` & `malbench-0.3.1/malbench/__main__.py`

 * *Files identical despite different names*

### Comparing `malbench-0.3.0/malbench/args.py` & `malbench-0.3.1/malbench/args.py`

 * *Files identical despite different names*

### Comparing `malbench-0.3.0/malbench/malware.py` & `malbench-0.3.1/malbench/malware.py`

 * *Files identical despite different names*

### Comparing `malbench-0.3.0/malbench/message.py` & `malbench-0.3.1/malbench/message.py`

 * *Files identical despite different names*

### Comparing `malbench-0.3.0/pyproject.toml` & `malbench-0.3.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 [tool.poetry]
 name = "malbench"
-version = "0.3.0"
+version = "0.3.1"
 description = "A tool used for automating the analysis of malware samples against antivirus solutions."
+repository = "https://github.com/youkergav/Malbench"
 authors = ["Gavin Youker <youkergav@gmail.com>"]
 readme = "README.md"
+license = "LICENSE"
 include = ["data/*"]
 exclude = ["data/samples"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 colorama = "^0.4.6"
 toml = "^0.10.2"
```

### Comparing `malbench-0.3.0/README.md` & `malbench-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `malbench-0.3.0/PKG-INFO` & `malbench-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 Metadata-Version: 2.1
 Name: malbench
-Version: 0.3.0
+Version: 0.3.1
 Summary: A tool used for automating the analysis of malware samples against antivirus solutions.
+Home-page: https://github.com/youkergav/Malbench
+License: LICENSE
 Author: Gavin Youker
 Author-email: youkergav@gmail.com
 Requires-Python: >=3.10,<4.0
+Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: colorama (>=0.4.6,<0.5.0)
 Requires-Dist: holidays (>=0.22,<0.23)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Requires-Dist: types-setuptools (>=67.7.0.0,<68.0.0.0)
+Project-URL: Repository, https://github.com/youkergav/Malbench
 Description-Content-Type: text/markdown
 
 # Malbench
 Malbench is a command-line tool for testing and evaluating the effectiveness of malware detection tools (such as antivirus solutions). It does this by running a set of malware samples, and checking if the malware is flagged by the detection tool we are evaluating. Malbench is built to be modular and configurable, so it can be customized to meet the specific needs of different users and environments.
 
 ## About
```

