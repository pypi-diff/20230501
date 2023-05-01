# Comparing `tmp/salamencrypt-1.0.1.tar.gz` & `tmp/salamencrypt-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "salamencrypt-1.0.1.tar", last modified: Mon May  1 17:48:57 2023, max compression
+gzip compressed data, was "salamencrypt-1.0.2.tar", last modified: Mon May  1 17:57:48 2023, max compression
```

## Comparing `salamencrypt-1.0.1.tar` & `salamencrypt-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-01 17:48:57.619559 salamencrypt-1.0.1/
--rw-rw----   0 root         (0) everybody  (9997)     1068 2022-08-05 16:34:15.000000 salamencrypt-1.0.1/LICENSE
--rw-rw----   0 root         (0) everybody  (9997)     2491 2023-05-01 17:48:57.579559 salamencrypt-1.0.1/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)     1998 2023-05-01 14:50:46.000000 salamencrypt-1.0.1/README.md
--rw-rw----   0 root         (0) everybody  (9997)       38 2023-05-01 17:48:57.619559 salamencrypt-1.0.1/setup.cfg
--rw-rw----   0 root         (0) everybody  (9997)     1108 2023-05-01 17:46:33.000000 salamencrypt-1.0.1/setup.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-01 17:48:56.099559 salamencrypt-1.0.1/src/
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-01 17:48:56.519559 salamencrypt-1.0.1/src/salamencrypt/
--rw-rw----   0 root         (0) everybody  (9997)       29 2023-05-01 14:13:39.000000 salamencrypt-1.0.1/src/salamencrypt/__init__.py
--rw-rw----   0 root         (0) everybody  (9997)      368 2023-05-01 17:43:47.000000 salamencrypt-1.0.1/src/salamencrypt/salamencrypt.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-01 17:48:57.529559 salamencrypt-1.0.1/src/salamencrypt.egg-info/
--rw-rw----   0 root         (0) everybody  (9997)     2491 2023-05-01 17:48:55.000000 salamencrypt-1.0.1/src/salamencrypt.egg-info/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)      248 2023-05-01 17:48:56.000000 salamencrypt-1.0.1/src/salamencrypt.egg-info/SOURCES.txt
--rw-rw----   0 root         (0) everybody  (9997)        1 2023-05-01 17:48:56.000000 salamencrypt-1.0.1/src/salamencrypt.egg-info/dependency_links.txt
--rw-rw----   0 root         (0) everybody  (9997)       13 2023-05-01 17:48:56.000000 salamencrypt-1.0.1/src/salamencrypt.egg-info/top_level.txt
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-01 17:57:48.817776 salamencrypt-1.0.2/
+-rw-rw----   0 root         (0) everybody  (9997)     1068 2022-08-05 16:34:15.000000 salamencrypt-1.0.2/LICENSE
+-rw-rw----   0 root         (0) everybody  (9997)     2491 2023-05-01 17:57:48.797776 salamencrypt-1.0.2/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)     1998 2023-05-01 14:50:46.000000 salamencrypt-1.0.2/README.md
+-rw-rw----   0 root         (0) everybody  (9997)       38 2023-05-01 17:57:48.817776 salamencrypt-1.0.2/setup.cfg
+-rw-rw----   0 root         (0) everybody  (9997)     1108 2023-05-01 17:56:03.000000 salamencrypt-1.0.2/setup.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-01 17:57:48.417776 salamencrypt-1.0.2/src/
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-01 17:57:48.637776 salamencrypt-1.0.2/src/salamencrypt/
+-rw-rw----   0 root         (0) everybody  (9997)       29 2023-05-01 14:13:39.000000 salamencrypt-1.0.2/src/salamencrypt/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)      512 2023-05-01 17:55:42.000000 salamencrypt-1.0.2/src/salamencrypt/salamencrypt.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-01 17:57:48.767776 salamencrypt-1.0.2/src/salamencrypt.egg-info/
+-rw-rw----   0 root         (0) everybody  (9997)     2491 2023-05-01 17:57:48.000000 salamencrypt-1.0.2/src/salamencrypt.egg-info/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)      248 2023-05-01 17:57:48.000000 salamencrypt-1.0.2/src/salamencrypt.egg-info/SOURCES.txt
+-rw-rw----   0 root         (0) everybody  (9997)        1 2023-05-01 17:57:48.000000 salamencrypt-1.0.2/src/salamencrypt.egg-info/dependency_links.txt
+-rw-rw----   0 root         (0) everybody  (9997)       13 2023-05-01 17:57:48.000000 salamencrypt-1.0.2/src/salamencrypt.egg-info/top_level.txt
```

### Comparing `salamencrypt-1.0.1/LICENSE` & `salamencrypt-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `salamencrypt-1.0.1/PKG-INFO` & `salamencrypt-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: salamencrypt
-Version: 1.0.1
+Version: 1.0.2
 Summary: • Encrypt & Run Code Tool Python .
 Home-page: https://t.me/T5B55
 Author: salammzere3
 Author-email: salamhunter@gmail.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 2
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: salamencrypt Version: 1.0.1 Summary: â¢ Encrypt &
+Metadata-Version: 2.1 Name: salamencrypt Version: 1.0.2 Summary: â¢ Encrypt &
 Run Code Tool Python . Home-page: https://t.me/T5B55 Author: salammzere3
 Author-email: salamhunter@gmail.com Project-URL: Bug Tracker, https://
 github.com/pypa/sampleproject/issues Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 2 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3 Description-Content-Type: text/markdown License-File:
 LICENSE
```

### Comparing `salamencrypt-1.0.1/README.md` & `salamencrypt-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `salamencrypt-1.0.1/setup.py` & `salamencrypt-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 f.write('requests\nuser_agent\njson\nsecrets\nnames\nhashlib\nurllib\nuuid\nre\nmechanize\ninstaloader\ntime\ndatetime\nbs4\nOneClick')
 
 fr = open("requirements.txt",'r')
 requires = fr.read().split('\n')
     
 setuptools.setup(
     name="salamencrypt",
-    version="1.0.1",
+    version="1.0.2",
     author="salammzere3",
     author_email="salamhunter@gmail.com",
     description="• Encrypt & Run Code Tool Python .",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://t.me/T5B55",
     project_urls={
```

### Comparing `salamencrypt-1.0.1/src/salamencrypt.egg-info/PKG-INFO` & `salamencrypt-1.0.2/src/salamencrypt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: salamencrypt
-Version: 1.0.1
+Version: 1.0.2
 Summary: • Encrypt & Run Code Tool Python .
 Home-page: https://t.me/T5B55
 Author: salammzere3
 Author-email: salamhunter@gmail.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 2
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: salamencrypt Version: 1.0.1 Summary: â¢ Encrypt &
+Metadata-Version: 2.1 Name: salamencrypt Version: 1.0.2 Summary: â¢ Encrypt &
 Run Code Tool Python . Home-page: https://t.me/T5B55 Author: salammzere3
 Author-email: salamhunter@gmail.com Project-URL: Bug Tracker, https://
 github.com/pypa/sampleproject/issues Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 2 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3 Description-Content-Type: text/markdown License-File:
 LICENSE
```

