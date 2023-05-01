# Comparing `tmp/thunno2-2.1.7.tar.gz` & `tmp/thunno2-2.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thunno2-2.1.7.tar", last modified: Mon May  1 12:43:07 2023, max compression
+gzip compressed data, was "thunno2-2.1.8.tar", last modified: Mon May  1 12:44:16 2023, max compression
```

## Comparing `thunno2-2.1.7.tar` & `thunno2-2.1.8.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-05-01 12:43:07.433351 thunno2-2.1.7/
--rw-r--r--   0 nayak      (501) staff       (20)      959 2023-05-01 12:43:07.433240 thunno2-2.1.7/PKG-INFO
--rw-r--r--   0 nayak      (501) staff       (20)       38 2023-05-01 12:43:07.433410 thunno2-2.1.7/setup.cfg
--rw-r--r--   0 nayak      (501) staff       (20)     1314 2023-04-16 17:25:02.000000 thunno2-2.1.7/setup.py
-drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-05-01 12:43:07.432575 thunno2-2.1.7/thunno2/
--rw-r--r--   0 nayak      (501) staff       (20)      200 2023-05-01 10:45:28.000000 thunno2-2.1.7/thunno2/__init__.py
--rw-r--r--   0 nayak      (501) staff       (20)      760 2023-04-30 09:02:54.000000 thunno2-2.1.7/thunno2/autoexplanation.py
--rw-r--r--   0 nayak      (501) staff       (20)     1393 2023-04-16 17:25:02.000000 thunno2-2.1.7/thunno2/codepage.py
--rw-r--r--   0 nayak      (501) staff       (20)    51654 2023-05-01 10:45:28.000000 thunno2-2.1.7/thunno2/commands.py
--rw-r--r--   0 nayak      (501) staff       (20)     2950 2023-04-16 17:25:02.000000 thunno2-2.1.7/thunno2/constants.py
--rw-r--r--   0 nayak      (501) staff       (20)   245360 2023-04-16 17:25:02.000000 thunno2-2.1.7/thunno2/dictionary.py
--rw-r--r--   0 nayak      (501) staff       (20)     7174 2023-04-27 10:00:16.000000 thunno2-2.1.7/thunno2/flags.py
--rw-r--r--   0 nayak      (501) staff       (20)    51729 2023-05-01 10:45:28.000000 thunno2-2.1.7/thunno2/helpers.py
--rw-r--r--   0 nayak      (501) staff       (20)    27697 2023-05-01 08:58:11.000000 thunno2-2.1.7/thunno2/interpreter.py
--rw-r--r--   0 nayak      (501) staff       (20)    23408 2023-04-27 13:07:04.000000 thunno2-2.1.7/thunno2/lexer.py
--rw-r--r--   0 nayak      (501) staff       (20)     1998 2023-05-01 08:52:47.000000 thunno2-2.1.7/thunno2/run.py
--rw-r--r--   0 nayak      (501) staff       (20)    72542 2023-04-30 14:45:33.000000 thunno2-2.1.7/thunno2/tests.py
--rw-r--r--   0 nayak      (501) staff       (20)     4019 2023-04-29 16:25:56.000000 thunno2-2.1.7/thunno2/tokens.py
--rw-r--r--   0 nayak      (501) staff       (20)       97 2023-05-01 12:42:55.000000 thunno2-2.1.7/thunno2/version.py
-drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-05-01 12:43:07.433093 thunno2-2.1.7/thunno2.egg-info/
--rw-r--r--   0 nayak      (501) staff       (20)      959 2023-05-01 12:43:07.000000 thunno2-2.1.7/thunno2.egg-info/PKG-INFO
--rw-r--r--   0 nayak      (501) staff       (20)      441 2023-05-01 12:43:07.000000 thunno2-2.1.7/thunno2.egg-info/SOURCES.txt
--rw-r--r--   0 nayak      (501) staff       (20)        1 2023-05-01 12:43:07.000000 thunno2-2.1.7/thunno2.egg-info/dependency_links.txt
--rw-r--r--   0 nayak      (501) staff       (20)       54 2023-05-01 12:43:07.000000 thunno2-2.1.7/thunno2.egg-info/entry_points.txt
--rw-r--r--   0 nayak      (501) staff       (20)        8 2023-05-01 12:43:07.000000 thunno2-2.1.7/thunno2.egg-info/top_level.txt
+drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-05-01 12:44:16.085301 thunno2-2.1.8/
+-rw-r--r--   0 nayak      (501) staff       (20)      959 2023-05-01 12:44:16.085177 thunno2-2.1.8/PKG-INFO
+-rw-r--r--   0 nayak      (501) staff       (20)       38 2023-05-01 12:44:16.085340 thunno2-2.1.8/setup.cfg
+-rw-r--r--   0 nayak      (501) staff       (20)     1314 2023-04-16 17:25:02.000000 thunno2-2.1.8/setup.py
+drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-05-01 12:44:16.084342 thunno2-2.1.8/thunno2/
+-rw-r--r--   0 nayak      (501) staff       (20)       22 2023-05-01 12:43:53.000000 thunno2-2.1.8/thunno2/__init__.py
+-rw-r--r--   0 nayak      (501) staff       (20)      760 2023-04-30 09:02:54.000000 thunno2-2.1.8/thunno2/autoexplanation.py
+-rw-r--r--   0 nayak      (501) staff       (20)     1393 2023-04-16 17:25:02.000000 thunno2-2.1.8/thunno2/codepage.py
+-rw-r--r--   0 nayak      (501) staff       (20)    51654 2023-05-01 10:45:28.000000 thunno2-2.1.8/thunno2/commands.py
+-rw-r--r--   0 nayak      (501) staff       (20)     2950 2023-04-16 17:25:02.000000 thunno2-2.1.8/thunno2/constants.py
+-rw-r--r--   0 nayak      (501) staff       (20)   245360 2023-04-16 17:25:02.000000 thunno2-2.1.8/thunno2/dictionary.py
+-rw-r--r--   0 nayak      (501) staff       (20)     7174 2023-04-27 10:00:16.000000 thunno2-2.1.8/thunno2/flags.py
+-rw-r--r--   0 nayak      (501) staff       (20)    51729 2023-05-01 10:45:28.000000 thunno2-2.1.8/thunno2/helpers.py
+-rw-r--r--   0 nayak      (501) staff       (20)    27697 2023-05-01 08:58:11.000000 thunno2-2.1.8/thunno2/interpreter.py
+-rw-r--r--   0 nayak      (501) staff       (20)    23408 2023-04-27 13:07:04.000000 thunno2-2.1.8/thunno2/lexer.py
+-rw-r--r--   0 nayak      (501) staff       (20)     1998 2023-05-01 08:52:47.000000 thunno2-2.1.8/thunno2/run.py
+-rw-r--r--   0 nayak      (501) staff       (20)    72542 2023-04-30 14:45:33.000000 thunno2-2.1.8/thunno2/tests.py
+-rw-r--r--   0 nayak      (501) staff       (20)     4019 2023-04-29 16:25:56.000000 thunno2-2.1.8/thunno2/tokens.py
+-rw-r--r--   0 nayak      (501) staff       (20)       97 2023-05-01 12:43:42.000000 thunno2-2.1.8/thunno2/version.py
+drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-05-01 12:44:16.085009 thunno2-2.1.8/thunno2.egg-info/
+-rw-r--r--   0 nayak      (501) staff       (20)      959 2023-05-01 12:44:16.000000 thunno2-2.1.8/thunno2.egg-info/PKG-INFO
+-rw-r--r--   0 nayak      (501) staff       (20)      441 2023-05-01 12:44:16.000000 thunno2-2.1.8/thunno2.egg-info/SOURCES.txt
+-rw-r--r--   0 nayak      (501) staff       (20)        1 2023-05-01 12:44:16.000000 thunno2-2.1.8/thunno2.egg-info/dependency_links.txt
+-rw-r--r--   0 nayak      (501) staff       (20)       54 2023-05-01 12:44:16.000000 thunno2-2.1.8/thunno2.egg-info/entry_points.txt
+-rw-r--r--   0 nayak      (501) staff       (20)        8 2023-05-01 12:44:16.000000 thunno2-2.1.8/thunno2.egg-info/top_level.txt
```

### Comparing `thunno2-2.1.7/PKG-INFO` & `thunno2-2.1.8/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: thunno2
-Version: 2.1.7
+Version: 2.1.8
 Summary: A golfing language
 Home-page: https://github.com/Thunno/Thunno2
 Author: Rujul Nayak
 Author-email: rujulnayak@outlook.com
 License: MIT
-Download-URL: https://github.com/Thunno/Thunno2/archive/refs/tags/v2.1.7.tar.gz
+Download-URL: https://github.com/Thunno/Thunno2/archive/refs/tags/v2.1.8.tar.gz
 Keywords: golfing,code-golf,language
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `thunno2-2.1.7/setup.py` & `thunno2-2.1.8/setup.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.1.7/thunno2/autoexplanation.py` & `thunno2-2.1.8/thunno2/autoexplanation.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.1.7/thunno2/codepage.py` & `thunno2-2.1.8/thunno2/codepage.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.1.7/thunno2/commands.py` & `thunno2-2.1.8/thunno2/commands.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.1.7/thunno2/constants.py` & `thunno2-2.1.8/thunno2/constants.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.1.7/thunno2/dictionary.py` & `thunno2-2.1.8/thunno2/dictionary.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.1.7/thunno2/flags.py` & `thunno2-2.1.8/thunno2/flags.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.1.7/thunno2/helpers.py` & `thunno2-2.1.8/thunno2/helpers.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.1.7/thunno2/interpreter.py` & `thunno2-2.1.8/thunno2/interpreter.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.1.7/thunno2/lexer.py` & `thunno2-2.1.8/thunno2/lexer.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.1.7/thunno2/run.py` & `thunno2-2.1.8/thunno2/run.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.1.7/thunno2/tests.py` & `thunno2-2.1.8/thunno2/tests.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.1.7/thunno2/tokens.py` & `thunno2-2.1.8/thunno2/tokens.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.1.7/thunno2.egg-info/PKG-INFO` & `thunno2-2.1.8/thunno2.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: thunno2
-Version: 2.1.7
+Version: 2.1.8
 Summary: A golfing language
 Home-page: https://github.com/Thunno/Thunno2
 Author: Rujul Nayak
 Author-email: rujulnayak@outlook.com
 License: MIT
-Download-URL: https://github.com/Thunno/Thunno2/archive/refs/tags/v2.1.7.tar.gz
+Download-URL: https://github.com/Thunno/Thunno2/archive/refs/tags/v2.1.8.tar.gz
 Keywords: golfing,code-golf,language
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

