# Comparing `tmp/pymathematics-2023.4.29.tar.gz` & `tmp/pymathematics-2023.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymathematics-2023.4.29.tar", last modified: Sat Apr 29 08:37:21 2023, max compression
+gzip compressed data, was "pymathematics-2023.5.1.tar", last modified: Mon May  1 18:00:28 2023, max compression
```

## Comparing `pymathematics-2023.4.29.tar` & `pymathematics-2023.5.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        0 2023-04-29 08:37:21.414260 pymathematics-2023.4.29/
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)     1088 2023-04-16 06:03:02.000000 pymathematics-2023.4.29/LICENSE
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      507 2023-04-29 08:37:21.406159 pymathematics-2023.4.29/PKG-INFO
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      166 2023-04-29 08:30:20.000000 pymathematics-2023.4.29/README.md
-drwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        0 2023-04-29 08:37:21.112787 pymathematics-2023.4.29/pymathematics/
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)    26470 2023-04-29 08:31:31.000000 pymathematics-2023.4.29/pymathematics/__init__.py
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      111 2023-04-29 08:30:00.000000 pymathematics-2023.4.29/pymathematics/info.py
-drwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        0 2023-04-29 08:37:21.352156 pymathematics-2023.4.29/pymathematics.egg-info/
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      507 2023-04-29 08:37:17.000000 pymathematics-2023.4.29/pymathematics.egg-info/PKG-INFO
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      258 2023-04-29 08:37:18.000000 pymathematics-2023.4.29/pymathematics.egg-info/SOURCES.txt
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        1 2023-04-29 08:37:17.000000 pymathematics-2023.4.29/pymathematics.egg-info/dependency_links.txt
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        6 2023-04-29 08:37:17.000000 pymathematics-2023.4.29/pymathematics.egg-info/requires.txt
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)       14 2023-04-29 08:37:17.000000 pymathematics-2023.4.29/pymathematics.egg-info/top_level.txt
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)       38 2023-04-29 08:37:21.416282 pymathematics-2023.4.29/setup.cfg
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      696 2023-04-29 08:33:18.000000 pymathematics-2023.4.29/setup.py
+drwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        0 2023-05-01 18:00:28.191467 pymathematics-2023.5.1/
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)     1088 2023-04-16 06:03:02.000000 pymathematics-2023.5.1/LICENSE
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      506 2023-05-01 18:00:28.155466 pymathematics-2023.5.1/PKG-INFO
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      165 2023-05-01 17:56:47.000000 pymathematics-2023.5.1/README.md
+drwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        0 2023-05-01 18:00:27.734466 pymathematics-2023.5.1/pymathematics/
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)    27686 2023-05-01 17:58:49.000000 pymathematics-2023.5.1/pymathematics/__init__.py
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      110 2023-05-01 17:54:20.000000 pymathematics-2023.5.1/pymathematics/info.py
+drwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        0 2023-05-01 18:00:28.084465 pymathematics-2023.5.1/pymathematics.egg-info/
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      506 2023-05-01 18:00:24.000000 pymathematics-2023.5.1/pymathematics.egg-info/PKG-INFO
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      258 2023-05-01 18:00:24.000000 pymathematics-2023.5.1/pymathematics.egg-info/SOURCES.txt
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        1 2023-05-01 18:00:24.000000 pymathematics-2023.5.1/pymathematics.egg-info/dependency_links.txt
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        6 2023-05-01 18:00:24.000000 pymathematics-2023.5.1/pymathematics.egg-info/requires.txt
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)       14 2023-05-01 18:00:24.000000 pymathematics-2023.5.1/pymathematics.egg-info/top_level.txt
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)       38 2023-05-01 18:00:28.195469 pymathematics-2023.5.1/setup.cfg
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      695 2023-05-01 17:56:39.000000 pymathematics-2023.5.1/setup.py
```

### Comparing `pymathematics-2023.4.29/LICENSE` & `pymathematics-2023.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pymathematics-2023.4.29/pymathematics/__init__.py` & `pymathematics-2023.5.1/pymathematics/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -185,14 +185,48 @@
             for y in range(cols2):
                 dot_product = 0
                 for z in range(cols1):
                     dot_product += matrix1[x][z]*matrix2[z][y]
                 result[x][y] = dot_product
         return result
 
+    def multiply(matrix_,const,dimension:int = 1):
+        if 1 <= dimension <= 2:
+            if dimension == 1:
+                for x in range(len(matrix_)):
+                    matrix_[x] = matrix_[x]*const
+            elif dimension == 2:
+                for rows in matrix_:
+                    for x in range(len(rows)):
+                        rows[x] = rows[x]*const
+            else:
+                raise ValueError("capable for only 1 and 2 dimension")
+        return matrix_
+
+    def reciprocal(matrix_,dimension:int = 1):
+        if 1 <= dimension <= 2:
+            if dimension == 1:
+                for x in range(len(matrix_)):
+                    matrix_[x] = 1/matrix_[x]
+            elif dimension == 2:
+                for rows in matrix_:
+                    for x in range(len(rows)):
+                        rows[x] = 1/rows[x]
+            else:
+                raise ValueError("capable for only 1 and 2 dimension")
+        return matrix_
+
+    def remove_column(matrix_,column):
+        for rows in matrix_:
+            rows.remove(rows[column])
+        return matrix_
+    
+    def remove_row(matrix_,column):
+        return matrix_.remove(matrix_[column])
+
 class sets:
     def toset(A:list) -> list:
         new_set = []
         for x in A:
             if x not in new_set:
                 new_set.append(x)
         return new_set
```

### Comparing `pymathematics-2023.4.29/setup.py` & `pymathematics-2023.5.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup,find_packages
 
 setup(
     name = "pymathematics",
-    version = "2023.4.29",
+    version = "2023.5.1",
     description = "package for mathematics",
     long_description = "for more info, check the github repository",
     author = "Sahil Rajwar",
     maintainer = "its_Sahil",
     author_email = "justsahilrajwar2004@gmail.com",
     packages = ["pymathematics"],
     license = "MIT",
```

