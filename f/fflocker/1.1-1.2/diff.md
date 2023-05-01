# Comparing `tmp/fflocker-1.1.tar.gz` & `tmp/fflocker-1.2.tar.gz`

## Comparing `fflocker-1.1.tar` & `fflocker-1.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fflocker-1.1/fflocker/__init__.py
--rw-r--r--   0        0        0     6707 2020-02-02 00:00:00.000000 fflocker-1.1/fflocker/file_locker.py
--rw-r--r--   0        0        0     8235 2020-02-02 00:00:00.000000 fflocker-1.1/fflocker/folder_locker.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 fflocker-1.1/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 fflocker-1.1/LICENSE
--rw-r--r--   0        0        0     3239 2020-02-02 00:00:00.000000 fflocker-1.1/README.md
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 fflocker-1.1/pyproject.toml
--rw-r--r--   0        0        0     3814 2020-02-02 00:00:00.000000 fflocker-1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fflocker-1.2/fflocker/__init__.py
+-rw-r--r--   0        0        0     6707 2020-02-02 00:00:00.000000 fflocker-1.2/fflocker/file_locker.py
+-rw-r--r--   0        0        0     8235 2020-02-02 00:00:00.000000 fflocker-1.2/fflocker/folder_locker.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 fflocker-1.2/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 fflocker-1.2/LICENSE
+-rw-r--r--   0        0        0     3239 2020-02-02 00:00:00.000000 fflocker-1.2/README.md
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 fflocker-1.2/pyproject.toml
+-rw-r--r--   0        0        0     3812 2020-02-02 00:00:00.000000 fflocker-1.2/PKG-INFO
```

### Comparing `fflocker-1.1/fflocker/file_locker.py` & `fflocker-1.2/fflocker/file_locker.py`

 * *Files identical despite different names*

### Comparing `fflocker-1.1/fflocker/folder_locker.py` & `fflocker-1.2/fflocker/folder_locker.py`

 * *Files identical despite different names*

### Comparing `fflocker-1.1/.gitignore` & `fflocker-1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `fflocker-1.1/LICENSE` & `fflocker-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fflocker-1.1/README.md` & `fflocker-1.2/README.md`

 * *Files identical despite different names*

### Comparing `fflocker-1.1/PKG-INFO` & `fflocker-1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: fflocker
-Version: 1.1
+Version: 1.2
 Summary: Locking files/folders [FF] in GNU/Linux via text-based user interface (TUI).
-Project-URL: Homepage, https://github.com/seVenVo1d/FFLocker
-Project-URL: Bug Tracker, https://github.com/seVenVo1d/FFLocker/issues
+Project-URL: Homepage, https://github.com/camarman/FFLocker
+Project-URL: Bug Tracker, https://github.com/camarman/FFLocker/issues
 Author: Arman Çam
 License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

