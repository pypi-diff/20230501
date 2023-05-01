# Comparing `tmp/psremoter-1.0.2.tar.gz` & `tmp/psremoter-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psremoter-1.0.2.tar", last modified: Mon May  1 10:59:14 2023, max compression
+gzip compressed data, was "psremoter-1.0.3.tar", last modified: Mon May  1 11:10:23 2023, max compression
```

## Comparing `psremoter-1.0.2.tar` & `psremoter-1.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 10:59:14.164340 psremoter-1.0.2/
--rw-rw-rw-   0        0        0     1345 2023-05-01 10:59:14.163371 psremoter-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      823 2023-05-01 08:55:38.000000 psremoter-1.0.2/README.md
--rw-rw-rw-   0        0        0      879 2023-05-01 10:58:51.000000 psremoter-1.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-01 10:59:14.165337 psremoter-1.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-01 10:59:14.120364 psremoter-1.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-05-01 10:59:14.126360 psremoter-1.0.2/src/psremoter/
--rw-rw-rw-   0        0        0       32 2023-05-01 10:47:51.000000 psremoter-1.0.2/src/psremoter/__init__.py
--rw-rw-rw-   0        0        0     3394 2023-05-01 10:47:51.000000 psremoter-1.0.2/src/psremoter/connector.py
-drwxrwxrwx   0        0        0        0 2023-05-01 10:59:14.159341 psremoter-1.0.2/src/psremoter.egg-info/
--rw-rw-rw-   0        0        0     1345 2023-05-01 10:59:14.000000 psremoter-1.0.2/src/psremoter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      276 2023-05-01 10:59:14.000000 psremoter-1.0.2/src/psremoter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 10:59:14.000000 psremoter-1.0.2/src/psremoter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      106 2023-05-01 10:59:14.000000 psremoter-1.0.2/src/psremoter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-01 10:59:14.000000 psremoter-1.0.2/src/psremoter.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-01 10:59:14.160339 psremoter-1.0.2/tests/
--rw-rw-rw-   0        0        0      545 2023-05-01 10:47:51.000000 psremoter-1.0.2/tests/tests.py
+drwxrwxrwx   0        0        0        0 2023-05-01 11:10:23.711571 psremoter-1.0.3/
+-rw-rw-rw-   0        0        0     1077 2023-05-01 11:09:52.000000 psremoter-1.0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0     1369 2023-05-01 11:10:23.710571 psremoter-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      823 2023-05-01 08:55:38.000000 psremoter-1.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-01 11:10:23.711571 psremoter-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      876 2023-05-01 11:08:29.000000 psremoter-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 11:10:23.670595 psremoter-1.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-05-01 11:10:23.677590 psremoter-1.0.3/src/psremoter/
+-rw-rw-rw-   0        0        0       32 2023-05-01 10:47:51.000000 psremoter-1.0.3/src/psremoter/__init__.py
+-rw-rw-rw-   0        0        0     3394 2023-05-01 10:47:51.000000 psremoter-1.0.3/src/psremoter/connector.py
+drwxrwxrwx   0        0        0        0 2023-05-01 11:10:23.707573 psremoter-1.0.3/src/psremoter.egg-info/
+-rw-rw-rw-   0        0        0     1369 2023-05-01 11:10:23.000000 psremoter-1.0.3/src/psremoter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2023-05-01 11:10:23.000000 psremoter-1.0.3/src/psremoter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 11:10:23.000000 psremoter-1.0.3/src/psremoter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-05-01 11:10:23.000000 psremoter-1.0.3/src/psremoter.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-01 11:10:23.708576 psremoter-1.0.3/tests/
+-rw-rw-rw-   0        0        0      545 2023-05-01 10:47:51.000000 psremoter-1.0.3/tests/tests.py
```

### Comparing `psremoter-1.0.2/PKG-INFO` & `psremoter-1.0.3/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: psremoter
-Version: 1.0.2
+Version: 1.0.3
 Summary: Powershell remote client tool for Python
-Author-email: Daniel Mandelblat <danielmande@gmail.com>
-Project-URL: Homepage, https://github.com/danielMandelblat/psremoter
-Keywords: Powershell,remote,client,commands,Windows
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
+Home-page: https://github.com/danielMandelblat/psremoter
+Author: Daniel Mandelblat
+Author-email: danielmande@gmail.cm
+Project-URL: Bug Tracker, https://github.com/danielMandelblat/psremoter
 Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Provides-Extra: dev
+License-File: LICENSE.txt
 
 # PSRemoteExecuter
 ## _Suitable only for Windows platforms_
 
 This package will help you to execute remote PowerSell script on other Windows platforms in your domain. 
 
 ## Features
```

### Comparing `psremoter-1.0.2/README.md` & `psremoter-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `psremoter-1.0.2/src/psremoter/connector.py` & `psremoter-1.0.3/src/psremoter/connector.py`

 * *Files identical despite different names*

### Comparing `psremoter-1.0.2/src/psremoter.egg-info/PKG-INFO` & `psremoter-1.0.3/src/psremoter.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: psremoter
-Version: 1.0.2
+Version: 1.0.3
 Summary: Powershell remote client tool for Python
-Author-email: Daniel Mandelblat <danielmande@gmail.com>
-Project-URL: Homepage, https://github.com/danielMandelblat/psremoter
-Keywords: Powershell,remote,client,commands,Windows
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
+Home-page: https://github.com/danielMandelblat/psremoter
+Author: Daniel Mandelblat
+Author-email: danielmande@gmail.cm
+Project-URL: Bug Tracker, https://github.com/danielMandelblat/psremoter
 Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Provides-Extra: dev
+License-File: LICENSE.txt
 
 # PSRemoteExecuter
 ## _Suitable only for Windows platforms_
 
 This package will help you to execute remote PowerSell script on other Windows platforms in your domain. 
 
 ## Features
```

### Comparing `psremoter-1.0.2/tests/tests.py` & `psremoter-1.0.3/tests/tests.py`

 * *Files identical despite different names*

