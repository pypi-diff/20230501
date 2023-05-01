# Comparing `tmp/easierfile-2.0.0.tar.gz` & `tmp/easierfile-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easierfile-2.0.0.tar", max compression
+gzip compressed data, was "easierfile-2.1.0.tar", max compression
```

## Comparing `easierfile-2.0.0.tar` & `easierfile-2.1.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       62 2023-04-21 13:34:36.835394 easierfile-2.0.0/easierfile/__init__.py
--rw-r--r--   0        0        0     4521 2023-04-22 03:44:40.952818 easierfile-2.0.0/easierfile/file.py
--rw-r--r--   0        0        0     1092 2023-04-11 00:52:37.919987 easierfile-2.0.0/LICENSE
--rw-r--r--   0        0        0      563 2023-04-21 13:40:18.443965 easierfile-2.0.0/pyproject.toml
--rw-r--r--   0        0        0      942 2023-04-20 04:53:26.793798 easierfile-2.0.0/README.md
--rw-r--r--   0        0        0     1769 1970-01-01 00:00:00.000000 easierfile-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0       62 2023-04-21 13:34:36.835394 easierfile-2.1.0/easierfile/__init__.py
+-rw-r--r--   0        0        0     4903 2023-05-01 13:07:38.204733 easierfile-2.1.0/easierfile/file.py
+-rw-r--r--   0        0        0     1092 2023-04-11 00:52:37.919987 easierfile-2.1.0/LICENSE
+-rw-r--r--   0        0        0      588 2023-05-01 12:41:45.401879 easierfile-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1676 2023-05-01 13:21:24.795756 easierfile-2.1.0/README.md
+-rw-r--r--   0        0        0     2498 1970-01-01 00:00:00.000000 easierfile-2.1.0/PKG-INFO
```

### Comparing `easierfile-2.0.0/easierfile/file.py` & `easierfile-2.1.0/easierfile/file.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         fcntl.flock(file.fileno(), fcntl.LOCK_EX | fcntl.LOCK_NB)
 
     def _unlock_file(file):
         fcntl.flock(file.fileno(), fcntl.LOCK_UN)
 
 
 import os
-
+from dynoptimdict import DynamicDataDict as Dict
 
 class File:
     def __init__(self, file_path, is_auto_create=True, is_occupy=True):
         # Get static file information.
         self.__m_info = {}
         self.__m_info["path"] = os.path.abspath(file_path)
         self.__m_info["dir_path"] = os.path.dirname(self.__m_info["path"])
@@ -50,31 +50,31 @@
         if self.__m_is_lock:
             try:
                 self.__lock(False)
             except FileNotFoundError:  # Indicates that the file lock does not exist and no further exception handling is required.
                 pass
 
     def __lock(self, is_lock):
-        if os.path.isfile(self.__m_info["path"]):
+        if self.status["exist"]:
             if is_lock:
                 self.__m_file = open(self.__m_info["path"], "w")
                 _lock_file(self.__m_file)
                 self.__m_is_lock = is_lock
             else:
                 _unlock_file(self.__m_file)
                 self.__m_file.close()
-                self.__m_is_lock = not is_lock
+                self.__m_is_lock = is_lock
         else:
             if is_lock:
                 raise FileNotFoundError("File was about to be occupied, but not found: " + self.__m_info["path"])
             else:
                 raise FileNotFoundError("File was about to be unoccupied, but not found: " + self.__m_info["path"])
 
     def create(self):
-        if not os.path.isfile(self.__m_info["path"]):
+        if not self.status["exist"]:
             if not os.path.exists(self.__m_info["dir_path"]):  # Create the file directory if it doesn't exist, so that code<open()> doesn't throw the exception.
                 os.mkdir(self.__m_info["dir_path"])
             try:
                 file_temp = open(self.__m_info["path"], "x")
             except FileExistsError:  # Avoid exception caused by creating corresponding file in other ways during program execution intervals.
                 pass
             else:
@@ -83,39 +83,53 @@
                 self.__lock(True)
         else:
             raise FileExistsError("File exists: " + self.__m_info["path"])
 
     def delete(self):
         if self.__m_is_lock:
             self.__lock(False)
-        if os.path.isfile(self.__m_info["path"]):
+        if self.status["exist"]:
             os.remove(self.__m_info["path"])
 
     def rewrite(self,content):
-        if os.path.isfile(self.__m_info["path"]):
+        if self.status["exist"]:
             file_temp = open(self.__m_info["path"], "w")
             file_temp.write(content)
             file_temp.close()
         else:
             raise FileNotFoundError("File not found: " + self.__m_info["path"])
 
     def append(self,content):
-        if os.path.isfile(self.__m_info["path"]):
+        if self.status["exist"]:
             file_temp = open(self.__m_info["path"], "a")
             file_temp.write(content)
             file_temp.close()
         else:
             raise FileNotFoundError("File not found: " + self.__m_info["path"])
 
     @property
     def content(self):
-        if os.path.isfile(self.__m_info["path"]):
+        if self.status["exist"]:
             file_temp = open(self.__m_info["path"], "r")
             content = file_temp.read()
             file_temp.close()
             return content
         else:
             raise FileNotFoundError("File not found: " + self.__m_info["path"])
 
     @property
     def info(self):
         return self.__m_info
+
+    @property
+    def status(self):
+        def get_status_file_lock():
+            return self.__m_is_lock
+
+        def get_status_exist():
+            return os.path.isfile(self.__m_info["path"])
+
+        status = Dict()
+        # Pass function pointers for obtaining dynamic data into object:Dict<status>.
+        status["file_lock"] = get_status_file_lock
+        status["exist"] = get_status_exist
+        return status
```

### Comparing `easierfile-2.0.0/LICENSE` & `easierfile-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `easierfile-2.0.0/pyproject.toml` & `easierfile-2.1.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 [tool.poetry]
 name = "easierfile"
-version = "2.0.0"
+version = "2.1.0"
 description = "An easier-to-use Python package that object-oriented encapsulates Python traditional built-in file operations."
 license = "MIT"
 authors = ["leoweyr <leoweyr@foxmail.com>"]
 readme = "README.md"
 repository = "https://github.com/leoweyr/Python-Easierfile"
 classifiers = [
     "Development Status :: 4 - Beta"
 ]
 packages = [{include = "easierfile"}]
 
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.8"
+dynoptimdict = "^1.0.0"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

