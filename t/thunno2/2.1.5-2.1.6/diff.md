# Comparing `tmp/thunno2-2.1.5.tar.gz` & `tmp/thunno2-2.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thunno2-2.1.5.tar", last modified: Mon May  1 08:32:38 2023, max compression
+gzip compressed data, was "thunno2-2.1.6.tar", last modified: Mon May  1 08:38:12 2023, max compression
```

## Comparing `thunno2-2.1.5.tar` & `thunno2-2.1.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-05-01 08:32:38.086150 thunno2-2.1.5/
--rw-r--r--   0 nayak      (501) staff       (20)      959 2023-05-01 08:32:38.086034 thunno2-2.1.5/PKG-INFO
--rw-r--r--   0 nayak      (501) staff       (20)       38 2023-05-01 08:32:38.086188 thunno2-2.1.5/setup.cfg
--rw-r--r--   0 nayak      (501) staff       (20)     1314 2023-04-16 17:25:02.000000 thunno2-2.1.5/setup.py
-drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-05-01 08:32:38.085365 thunno2-2.1.5/thunno2/
--rw-r--r--   0 nayak      (501) staff       (20)       22 2023-04-03 16:07:07.000000 thunno2-2.1.5/thunno2/__init__.py
--rw-r--r--   0 nayak      (501) staff       (20)      760 2023-04-30 09:02:54.000000 thunno2-2.1.5/thunno2/autoexplanation.py
--rw-r--r--   0 nayak      (501) staff       (20)     1393 2023-04-16 17:25:02.000000 thunno2-2.1.5/thunno2/codepage.py
--rw-r--r--   0 nayak      (501) staff       (20)    51654 2023-04-29 19:16:49.000000 thunno2-2.1.5/thunno2/commands.py
--rw-r--r--   0 nayak      (501) staff       (20)     2950 2023-04-16 17:25:02.000000 thunno2-2.1.5/thunno2/constants.py
--rw-r--r--   0 nayak      (501) staff       (20)   245360 2023-04-16 17:25:02.000000 thunno2-2.1.5/thunno2/dictionary.py
--rw-r--r--   0 nayak      (501) staff       (20)     7174 2023-04-27 10:00:16.000000 thunno2-2.1.5/thunno2/flags.py
--rw-r--r--   0 nayak      (501) staff       (20)    51729 2023-05-01 08:31:39.000000 thunno2-2.1.5/thunno2/helpers.py
--rw-r--r--   0 nayak      (501) staff       (20)    27697 2023-04-30 14:45:33.000000 thunno2-2.1.5/thunno2/interpreter.py
--rw-r--r--   0 nayak      (501) staff       (20)    23408 2023-04-27 13:07:04.000000 thunno2-2.1.5/thunno2/lexer.py
--rw-r--r--   0 nayak      (501) staff       (20)     1998 2023-04-30 09:02:54.000000 thunno2-2.1.5/thunno2/run.py
--rw-r--r--   0 nayak      (501) staff       (20)    72542 2023-04-30 14:45:33.000000 thunno2-2.1.5/thunno2/tests.py
--rw-r--r--   0 nayak      (501) staff       (20)     4019 2023-04-29 16:25:56.000000 thunno2-2.1.5/thunno2/tokens.py
--rw-r--r--   0 nayak      (501) staff       (20)       97 2023-05-01 08:32:19.000000 thunno2-2.1.5/thunno2/version.py
-drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-05-01 08:32:38.085883 thunno2-2.1.5/thunno2.egg-info/
--rw-r--r--   0 nayak      (501) staff       (20)      959 2023-05-01 08:32:37.000000 thunno2-2.1.5/thunno2.egg-info/PKG-INFO
--rw-r--r--   0 nayak      (501) staff       (20)      441 2023-05-01 08:32:37.000000 thunno2-2.1.5/thunno2.egg-info/SOURCES.txt
--rw-r--r--   0 nayak      (501) staff       (20)        1 2023-05-01 08:32:37.000000 thunno2-2.1.5/thunno2.egg-info/dependency_links.txt
--rw-r--r--   0 nayak      (501) staff       (20)       54 2023-05-01 08:32:37.000000 thunno2-2.1.5/thunno2.egg-info/entry_points.txt
--rw-r--r--   0 nayak      (501) staff       (20)        8 2023-05-01 08:32:37.000000 thunno2-2.1.5/thunno2.egg-info/top_level.txt
+drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-05-01 08:38:12.872437 thunno2-2.1.6/
+-rw-r--r--   0 nayak      (501) staff       (20)      959 2023-05-01 08:38:12.872324 thunno2-2.1.6/PKG-INFO
+-rw-r--r--   0 nayak      (501) staff       (20)       38 2023-05-01 08:38:12.872471 thunno2-2.1.6/setup.cfg
+-rw-r--r--   0 nayak      (501) staff       (20)     1314 2023-04-16 17:25:02.000000 thunno2-2.1.6/setup.py
+drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-05-01 08:38:12.871621 thunno2-2.1.6/thunno2/
+-rw-r--r--   0 nayak      (501) staff       (20)       22 2023-04-03 16:07:07.000000 thunno2-2.1.6/thunno2/__init__.py
+-rw-r--r--   0 nayak      (501) staff       (20)      760 2023-04-30 09:02:54.000000 thunno2-2.1.6/thunno2/autoexplanation.py
+-rw-r--r--   0 nayak      (501) staff       (20)     1393 2023-04-16 17:25:02.000000 thunno2-2.1.6/thunno2/codepage.py
+-rw-r--r--   0 nayak      (501) staff       (20)    51654 2023-04-29 19:16:49.000000 thunno2-2.1.6/thunno2/commands.py
+-rw-r--r--   0 nayak      (501) staff       (20)     2950 2023-04-16 17:25:02.000000 thunno2-2.1.6/thunno2/constants.py
+-rw-r--r--   0 nayak      (501) staff       (20)   245360 2023-04-16 17:25:02.000000 thunno2-2.1.6/thunno2/dictionary.py
+-rw-r--r--   0 nayak      (501) staff       (20)     7174 2023-04-27 10:00:16.000000 thunno2-2.1.6/thunno2/flags.py
+-rw-r--r--   0 nayak      (501) staff       (20)    51729 2023-05-01 08:31:39.000000 thunno2-2.1.6/thunno2/helpers.py
+-rw-r--r--   0 nayak      (501) staff       (20)    27697 2023-05-01 08:37:46.000000 thunno2-2.1.6/thunno2/interpreter.py
+-rw-r--r--   0 nayak      (501) staff       (20)    23408 2023-04-27 13:07:04.000000 thunno2-2.1.6/thunno2/lexer.py
+-rw-r--r--   0 nayak      (501) staff       (20)     1998 2023-04-30 09:02:54.000000 thunno2-2.1.6/thunno2/run.py
+-rw-r--r--   0 nayak      (501) staff       (20)    72542 2023-04-30 14:45:33.000000 thunno2-2.1.6/thunno2/tests.py
+-rw-r--r--   0 nayak      (501) staff       (20)     4019 2023-04-29 16:25:56.000000 thunno2-2.1.6/thunno2/tokens.py
+-rw-r--r--   0 nayak      (501) staff       (20)       97 2023-05-01 08:38:05.000000 thunno2-2.1.6/thunno2/version.py
+drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-05-01 08:38:12.872173 thunno2-2.1.6/thunno2.egg-info/
+-rw-r--r--   0 nayak      (501) staff       (20)      959 2023-05-01 08:38:12.000000 thunno2-2.1.6/thunno2.egg-info/PKG-INFO
+-rw-r--r--   0 nayak      (501) staff       (20)      441 2023-05-01 08:38:12.000000 thunno2-2.1.6/thunno2.egg-info/SOURCES.txt
+-rw-r--r--   0 nayak      (501) staff       (20)        1 2023-05-01 08:38:12.000000 thunno2-2.1.6/thunno2.egg-info/dependency_links.txt
+-rw-r--r--   0 nayak      (501) staff       (20)       54 2023-05-01 08:38:12.000000 thunno2-2.1.6/thunno2.egg-info/entry_points.txt
+-rw-r--r--   0 nayak      (501) staff       (20)        8 2023-05-01 08:38:12.000000 thunno2-2.1.6/thunno2.egg-info/top_level.txt
```

### Comparing `thunno2-2.1.5/PKG-INFO` & `thunno2-2.1.6/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: thunno2
-Version: 2.1.5
+Version: 2.1.6
 Summary: A golfing language
 Home-page: https://github.com/Thunno/Thunno2
 Author: Rujul Nayak
 Author-email: rujulnayak@outlook.com
 License: MIT
-Download-URL: https://github.com/Thunno/Thunno2/archive/refs/tags/v2.1.5.tar.gz
+Download-URL: https://github.com/Thunno/Thunno2/archive/refs/tags/v2.1.6.tar.gz
 Keywords: golfing,code-golf,language
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `thunno2-2.1.5/setup.py` & `thunno2-2.1.6/setup.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.1.5/thunno2/autoexplanation.py` & `thunno2-2.1.6/thunno2/autoexplanation.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.1.5/thunno2/codepage.py` & `thunno2-2.1.6/thunno2/codepage.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.1.5/thunno2/commands.py` & `thunno2-2.1.6/thunno2/commands.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.1.5/thunno2/constants.py` & `thunno2-2.1.6/thunno2/constants.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.1.5/thunno2/dictionary.py` & `thunno2-2.1.6/thunno2/dictionary.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.1.5/thunno2/flags.py` & `thunno2-2.1.6/thunno2/flags.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.1.5/thunno2/helpers.py` & `thunno2-2.1.6/thunno2/helpers.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.1.5/thunno2/interpreter.py` & `thunno2-2.1.6/thunno2/interpreter.py`

 * *Files 0% similar despite different names*

```diff
@@ -220,15 +220,15 @@
                 + dictionary.dictionary_decompress_string(info[2:]).title()
             )
         elif desc == "compressed number" or desc == "small compressed number":
             base255_number = decompress(info, "»")
             ctx.stack.push(base255_number)
         elif desc == "compressed list":
             base255_number = decompress(info, "¿")
-            decompressed_string = to_custom_base_string(",.0123456789-", base255_number)
+            decompressed_string = to_custom_base_string("0123456789-.,", base255_number)
             try:
                 if decompressed_string[:1] == ",":
                     decompressed_string = "0" + decompressed_string
                 if decompressed_string[-1:] == ",":
                     decompressed_string += "0"
                 if decompressed_string[:1] == ".":
                     decompressed_string = ".5" + decompressed_string[1:]
```

### Comparing `thunno2-2.1.5/thunno2/lexer.py` & `thunno2-2.1.6/thunno2/lexer.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.1.5/thunno2/run.py` & `thunno2-2.1.6/thunno2/run.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.1.5/thunno2/tests.py` & `thunno2-2.1.6/thunno2/tests.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.1.5/thunno2/tokens.py` & `thunno2-2.1.6/thunno2/tokens.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.1.5/thunno2.egg-info/PKG-INFO` & `thunno2-2.1.6/thunno2.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: thunno2
-Version: 2.1.5
+Version: 2.1.6
 Summary: A golfing language
 Home-page: https://github.com/Thunno/Thunno2
 Author: Rujul Nayak
 Author-email: rujulnayak@outlook.com
 License: MIT
-Download-URL: https://github.com/Thunno/Thunno2/archive/refs/tags/v2.1.5.tar.gz
+Download-URL: https://github.com/Thunno/Thunno2/archive/refs/tags/v2.1.6.tar.gz
 Keywords: golfing,code-golf,language
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

