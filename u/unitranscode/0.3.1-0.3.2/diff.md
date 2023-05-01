# Comparing `tmp/unitranscode-0.3.1.tar.gz` & `tmp/unitranscode-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unitranscode-0.3.1.tar", last modified: Mon May  1 05:08:32 2023, max compression
+gzip compressed data, was "unitranscode-0.3.2.tar", last modified: Mon May  1 05:16:24 2023, max compression
```

## Comparing `unitranscode-0.3.1.tar` & `unitranscode-0.3.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 matthew   (1000) matthew   (1000)        0 2023-05-01 05:08:32.766454 unitranscode-0.3.1/
--rw-rw-r--   0 matthew   (1000) matthew   (1000)     1062 2023-01-01 01:11:48.000000 unitranscode-0.3.1/LICENSE
--rw-rw-r--   0 matthew   (1000) matthew   (1000)      603 2023-05-01 05:08:32.766454 unitranscode-0.3.1/PKG-INFO
--rw-rw-r--   0 matthew   (1000) matthew   (1000)     1399 2023-01-01 03:15:58.000000 unitranscode-0.3.1/README.md
--rw-rw-r--   0 matthew   (1000) matthew   (1000)       38 2023-05-01 05:08:32.766454 unitranscode-0.3.1/setup.cfg
--rw-rw-r--   0 matthew   (1000) matthew   (1000)      717 2023-05-01 05:08:08.000000 unitranscode-0.3.1/setup.py
-drwxrwxr-x   0 matthew   (1000) matthew   (1000)        0 2023-05-01 05:08:32.742454 unitranscode-0.3.1/tests/
--rw-rw-r--   0 matthew   (1000) matthew   (1000)     1138 2023-04-28 03:34:33.000000 unitranscode-0.3.1/tests/test_transcoder.py
-drwxrwxr-x   0 matthew   (1000) matthew   (1000)        0 2023-05-01 05:08:32.742454 unitranscode-0.3.1/unitranscode/
--rw-rw-r--   0 matthew   (1000) matthew   (1000)      411 2023-01-01 01:28:59.000000 unitranscode-0.3.1/unitranscode/__init__.py
--rw-rw-r--   0 matthew   (1000) matthew   (1000)     3661 2023-04-28 03:37:11.000000 unitranscode-0.3.1/unitranscode/custom_types.py
--rw-rw-r--   0 matthew   (1000) matthew   (1000)    25244 2023-05-01 05:05:38.000000 unitranscode-0.3.1/unitranscode/transcoder.py
--rw-rw-r--   0 matthew   (1000) matthew   (1000)      137 2023-01-01 01:28:30.000000 unitranscode-0.3.1/unitranscode/utils.py
-drwxrwxr-x   0 matthew   (1000) matthew   (1000)        0 2023-05-01 05:08:32.742454 unitranscode-0.3.1/unitranscode.egg-info/
--rw-rw-r--   0 matthew   (1000) matthew   (1000)      603 2023-05-01 05:08:32.000000 unitranscode-0.3.1/unitranscode.egg-info/PKG-INFO
--rw-rw-r--   0 matthew   (1000) matthew   (1000)      333 2023-05-01 05:08:32.000000 unitranscode-0.3.1/unitranscode.egg-info/SOURCES.txt
--rw-rw-r--   0 matthew   (1000) matthew   (1000)        1 2023-05-01 05:08:32.000000 unitranscode-0.3.1/unitranscode.egg-info/dependency_links.txt
--rw-rw-r--   0 matthew   (1000) matthew   (1000)        7 2023-05-01 05:08:32.000000 unitranscode-0.3.1/unitranscode.egg-info/requires.txt
--rw-rw-r--   0 matthew   (1000) matthew   (1000)       13 2023-05-01 05:08:32.000000 unitranscode-0.3.1/unitranscode.egg-info/top_level.txt
+drwxrwxr-x   0 matthew   (1000) matthew   (1000)        0 2023-05-01 05:16:24.884529 unitranscode-0.3.2/
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)     1062 2023-01-01 01:11:48.000000 unitranscode-0.3.2/LICENSE
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)      558 2023-05-01 05:16:24.884529 unitranscode-0.3.2/PKG-INFO
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)     1399 2023-01-01 03:15:58.000000 unitranscode-0.3.2/README.md
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)       38 2023-05-01 05:16:24.884529 unitranscode-0.3.2/setup.cfg
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)      717 2023-05-01 05:15:41.000000 unitranscode-0.3.2/setup.py
+drwxrwxr-x   0 matthew   (1000) matthew   (1000)        0 2023-05-01 05:16:24.852530 unitranscode-0.3.2/tests/
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)     1138 2023-04-28 03:34:33.000000 unitranscode-0.3.2/tests/test_transcoder.py
+drwxrwxr-x   0 matthew   (1000) matthew   (1000)        0 2023-05-01 05:16:24.884529 unitranscode-0.3.2/unitranscode/
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)      411 2023-01-01 01:28:59.000000 unitranscode-0.3.2/unitranscode/__init__.py
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)     3661 2023-04-28 03:37:11.000000 unitranscode-0.3.2/unitranscode/custom_types.py
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)    25254 2023-05-01 05:15:19.000000 unitranscode-0.3.2/unitranscode/transcoder.py
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)      137 2023-05-01 05:12:02.000000 unitranscode-0.3.2/unitranscode/utils.py
+drwxrwxr-x   0 matthew   (1000) matthew   (1000)        0 2023-05-01 05:16:24.884529 unitranscode-0.3.2/unitranscode.egg-info/
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)      558 2023-05-01 05:16:24.000000 unitranscode-0.3.2/unitranscode.egg-info/PKG-INFO
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)      333 2023-05-01 05:16:24.000000 unitranscode-0.3.2/unitranscode.egg-info/SOURCES.txt
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)        1 2023-05-01 05:16:24.000000 unitranscode-0.3.2/unitranscode.egg-info/dependency_links.txt
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)        7 2023-05-01 05:16:24.000000 unitranscode-0.3.2/unitranscode.egg-info/requires.txt
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)       13 2023-05-01 05:16:24.000000 unitranscode-0.3.2/unitranscode.egg-info/top_level.txt
```

### Comparing `unitranscode-0.3.1/LICENSE` & `unitranscode-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `unitranscode-0.3.1/PKG-INFO` & `unitranscode-0.3.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,15 @@
 Metadata-Version: 2.1
 Name: unitranscode
-Version: 0.3.1
+Version: 0.3.2
 Summary: Universal transcoding library
 Home-page: https://github.com/MatthewScholefield/unitranscode
 Author: Matthew D. Scholefield
 Author-email: matthew331199@gmail.com
-License: UNKNOWN
 Keywords: unitranscode
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 License-File: LICENSE
-
-UNKNOWN
-
```

### Comparing `unitranscode-0.3.1/README.md` & `unitranscode-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `unitranscode-0.3.1/setup.py` & `unitranscode-0.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 
 setup(
     name='unitranscode',
-    version='0.3.1',
+    version='0.3.2',
     description='Universal transcoding library',
     url='https://github.com/MatthewScholefield/unitranscode',
     author='Matthew D. Scholefield',
     author_email='matthew331199@gmail.com',
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
```

### Comparing `unitranscode-0.3.1/tests/test_transcoder.py` & `unitranscode-0.3.2/tests/test_transcoder.py`

 * *Files identical despite different names*

### Comparing `unitranscode-0.3.1/unitranscode/custom_types.py` & `unitranscode-0.3.2/unitranscode/custom_types.py`

 * *Files identical despite different names*

### Comparing `unitranscode-0.3.1/unitranscode/transcoder.py` & `unitranscode-0.3.2/unitranscode/transcoder.py`

 * *Files 0% similar despite different names*

```diff
@@ -694,15 +694,15 @@
         args.append(out_file_fmt)
         self.ffmpeg(
             *args,
             duration_s=self.info(in_file).duration_s,
             on_progress=on_progress,
             op=op,
         )
-        pre, suff = out_file_fmt.split('%d')
+        pre, suff = out_file_fmt.encode().split(b'%d')
         out_filenames_raw = sorted(
             re.findall(
                 rb"^\s*\[[^]]*]\s*Opening '(.*)' for writing\s*$",
                 (
                     op.stderr_bytes.replace(b'\r', b'\n')
                     + b'\n'
                     + op.stdout_bytes.replace(b'\r', b'\n')
```

### Comparing `unitranscode-0.3.1/unitranscode.egg-info/PKG-INFO` & `unitranscode-0.3.2/unitranscode.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,15 @@
 Metadata-Version: 2.1
 Name: unitranscode
-Version: 0.3.1
+Version: 0.3.2
 Summary: Universal transcoding library
 Home-page: https://github.com/MatthewScholefield/unitranscode
 Author: Matthew D. Scholefield
 Author-email: matthew331199@gmail.com
-License: UNKNOWN
 Keywords: unitranscode
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 License-File: LICENSE
-
-UNKNOWN
-
```

