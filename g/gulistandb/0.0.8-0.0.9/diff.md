# Comparing `tmp/gulistandb-0.0.8.tar.gz` & `tmp/gulistandb-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gulistandb-0.0.8.tar", last modified: Thu Apr 27 11:50:44 2023, max compression
+gzip compressed data, was "gulistandb-0.0.9.tar", last modified: Mon May  1 14:05:33 2023, max compression
```

## Comparing `gulistandb-0.0.8.tar` & `gulistandb-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 11:50:44.287523 gulistandb-0.0.8/
--rw-rw-rw-   0        0        0     1093 2023-04-24 06:50:57.000000 gulistandb-0.0.8/License
--rw-rw-rw-   0        0        0    10082 2023-04-27 11:50:44.277529 gulistandb-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0    18722 2023-04-27 10:52:57.000000 gulistandb-0.0.8/README.md
--rw-rw-rw-   0        0        0       42 2023-04-27 11:50:44.288522 gulistandb-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1040 2023-04-27 11:50:35.000000 gulistandb-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-27 11:50:44.160601 gulistandb-0.0.8/src/
--rw-rw-rw-   0        0        0        0 2023-04-22 14:38:14.000000 gulistandb-0.0.8/src/__init__.py
--rw-rw-rw-   0        0        0     1066 2023-04-27 04:58:22.000000 gulistandb-0.0.8/src/editor.py
-drwxrwxrwx   0        0        0        0 2023-04-27 11:50:44.269534 gulistandb-0.0.8/src/gulistandb.egg-info/
--rw-rw-rw-   0        0        0    10082 2023-04-27 11:50:43.000000 gulistandb-0.0.8/src/gulistandb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      292 2023-04-27 11:50:43.000000 gulistandb-0.0.8/src/gulistandb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 11:50:43.000000 gulistandb-0.0.8/src/gulistandb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-04-27 11:50:43.000000 gulistandb-0.0.8/src/gulistandb.egg-info/requires.txt
--rw-rw-rw-   0        0        0       42 2023-04-27 11:50:43.000000 gulistandb-0.0.8/src/gulistandb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     6409 2023-04-27 11:49:40.000000 gulistandb-0.0.8/src/gulistandb.py
--rw-rw-rw-   0        0        0     1361 2023-04-26 11:39:19.000000 gulistandb-0.0.8/src/reader.py
--rw-rw-rw-   0        0        0     1766 2023-04-27 04:59:45.000000 gulistandb-0.0.8/src/writter.py
+drwxrwxrwx   0        0        0        0 2023-05-01 14:05:33.450667 gulistandb-0.0.9/
+-rw-rw-rw-   0        0        0     1093 2023-04-24 06:50:57.000000 gulistandb-0.0.9/License
+-rw-rw-rw-   0        0        0    10082 2023-05-01 14:05:33.439671 gulistandb-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0    18722 2023-04-27 10:52:57.000000 gulistandb-0.0.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-01 14:05:33.452666 gulistandb-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1040 2023-05-01 14:05:11.000000 gulistandb-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 14:05:33.338737 gulistandb-0.0.9/src/
+-rw-rw-rw-   0        0        0        0 2023-04-22 14:38:14.000000 gulistandb-0.0.9/src/__init__.py
+-rw-rw-rw-   0        0        0     1066 2023-04-27 04:58:22.000000 gulistandb-0.0.9/src/editor.py
+drwxrwxrwx   0        0        0        0 2023-05-01 14:05:33.434674 gulistandb-0.0.9/src/gulistandb.egg-info/
+-rw-rw-rw-   0        0        0    10082 2023-05-01 14:05:32.000000 gulistandb-0.0.9/src/gulistandb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      292 2023-05-01 14:05:33.000000 gulistandb-0.0.9/src/gulistandb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 14:05:32.000000 gulistandb-0.0.9/src/gulistandb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-05-01 14:05:32.000000 gulistandb-0.0.9/src/gulistandb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       42 2023-05-01 14:05:32.000000 gulistandb-0.0.9/src/gulistandb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     6423 2023-05-01 14:03:44.000000 gulistandb-0.0.9/src/gulistandb.py
+-rw-rw-rw-   0        0        0     1361 2023-04-26 11:39:19.000000 gulistandb-0.0.9/src/reader.py
+-rw-rw-rw-   0        0        0     1766 2023-04-28 07:16:42.000000 gulistandb-0.0.9/src/writter.py
```

### Comparing `gulistandb-0.0.8/License` & `gulistandb-0.0.9/License`

 * *Files identical despite different names*

### Comparing `gulistandb-0.0.8/PKG-INFO` & `gulistandb-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: gulistandb
-Version: 0.0.8
+Version: 0.0.9
 Summary: This is a user-friendly local database package designed for beginners. You don't need to know any query language - simply import the package and use its methods according to the documentation. The data will be automatically saved in a CSV file in a 'data' folder within your current working directory. This package is perfect for small-scale projects or for those who are just getting started with beginner python project
-Home-page: https://github.com/AzazAhmedLipu79/GuliStan_DB
+Home-page: https://github.com/AzazAhmedLipu79/gulistanDB/
 Author: Azaz Ahmed Lipu
 Author-email: lipuahmedazaz79@gmail.com
 License: MIT
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: License
```

### Comparing `gulistandb-0.0.8/README.md` & `gulistandb-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `gulistandb-0.0.8/setup.py` & `gulistandb-0.0.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,24 +2,24 @@
 
 
 with open('README.md', 'r', encoding='utf-16') as f:
     long_description = f.read()
 
 setup(
     name='gulistandb',
-    version='0.0.8',
+    version='0.0.9',
     install_requires=[
         'pandas',
         # add more dependencies as needed
     ],
     package_dir={'': 'src'},
 
     # metadata
     author='Azaz Ahmed Lipu',
     author_email='lipuahmedazaz79@gmail.com',
     description="This is a user-friendly local database package designed for beginners. You don't need to know any query language - simply import the package and use its methods according to the documentation. The data will be automatically saved in a CSV file in a 'data' folder within your current working directory. This package is perfect for small-scale projects or for those who are just getting started with beginner python project",
     license='MIT',
     long_description=long_description,
     long_description_content_type='text/markdown',
-    url='https://github.com/AzazAhmedLipu79/GuliStan_DB',
+    url='https://github.com/AzazAhmedLipu79/gulistanDB/',
     python_requires='>=3'
 )
```

### Comparing `gulistandb-0.0.8/src/editor.py` & `gulistandb-0.0.9/src/editor.py`

 * *Files identical despite different names*

### Comparing `gulistandb-0.0.8/src/gulistandb.egg-info/PKG-INFO` & `gulistandb-0.0.9/src/gulistandb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: gulistandb
-Version: 0.0.8
+Version: 0.0.9
 Summary: This is a user-friendly local database package designed for beginners. You don't need to know any query language - simply import the package and use its methods according to the documentation. The data will be automatically saved in a CSV file in a 'data' folder within your current working directory. This package is perfect for small-scale projects or for those who are just getting started with beginner python project
-Home-page: https://github.com/AzazAhmedLipu79/GuliStan_DB
+Home-page: https://github.com/AzazAhmedLipu79/gulistanDB/
 Author: Azaz Ahmed Lipu
 Author-email: lipuahmedazaz79@gmail.com
 License: MIT
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: License
```

### Comparing `gulistandb-0.0.8/src/gulistandb.py` & `gulistandb-0.0.9/src/gulistandb.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,22 +37,22 @@
 
         self.folder_path = os.path.join(
             os.getcwd(), "Data")
         self.file_path = f'{os.path.join(os.getcwd(), "Data")}/{self.TableName}.{self.fileType}'
 
         print(
             f"GulistanDB:\t\033[1;32mTable initialized successfully!\n{self.file_path}\033[0m")
-        if self.mode == True:
-            self.__commit()
-            return None
-        print("ReInitilized")
+        # if self.mode == True:
+        #     self.__commit()
+        #     return None
+        # print("ReInitilized")
 
-    def commit_mode(self, mode=False):
-        self.mode = mode
-        print(self.mode)
+    # def commit_mode(self, mode=False):
+    #     self.mode = mode
+    #     print(self.mode)
 
     def __commit(self):
         self.file_path = f'{os.path.join(os.getcwd(), "Data")}/{self.TableName}.{self.fileType}'
         try:
             if not os.path.exists(self.folder_path):
                 os.makedirs(self.folder_path)
             fileInit(self.fileType, self.file_path, self.column)
```

### Comparing `gulistandb-0.0.8/src/reader.py` & `gulistandb-0.0.9/src/reader.py`

 * *Files identical despite different names*

### Comparing `gulistandb-0.0.8/src/writter.py` & `gulistandb-0.0.9/src/writter.py`

 * *Files identical despite different names*

