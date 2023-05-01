# Comparing `tmp/gtFrame-1.2.2.tar.gz` & `tmp/gtFrame-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gtFrame-1.2.2.tar", last modified: Thu Apr 13 17:52:40 2023, max compression
+gzip compressed data, was "gtFrame-1.2.3.tar", last modified: Mon May  1 18:20:40 2023, max compression
```

## Comparing `gtFrame-1.2.2.tar` & `gtFrame-1.2.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:52:40.043404 gtFrame-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-04-13 17:52:30.000000 gtFrame-1.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-04-13 17:52:40.043404 gtFrame-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-13 17:52:30.000000 gtFrame-1.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:52:40.043404 gtFrame-1.2.2/gtFrame/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-13 17:52:30.000000 gtFrame-1.2.2/gtFrame/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22991 2023-04-13 17:52:30.000000 gtFrame-1.2.2/gtFrame/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)    10282 2023-04-13 17:52:30.000000 gtFrame-1.2.2/gtFrame/direction.py
--rw-r--r--   0 runner    (1001) docker     (123)    14238 2023-04-13 17:52:30.000000 gtFrame-1.2.2/gtFrame/position.py
--rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-04-13 17:52:30.000000 gtFrame-1.2.2/gtFrame/rotation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:52:40.043404 gtFrame-1.2.2/gtFrame.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-04-13 17:52:40.000000 gtFrame-1.2.2/gtFrame.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-04-13 17:52:40.000000 gtFrame-1.2.2/gtFrame.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 17:52:40.000000 gtFrame-1.2.2/gtFrame.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-13 17:52:40.000000 gtFrame-1.2.2/gtFrame.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-13 17:52:40.000000 gtFrame-1.2.2/gtFrame.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-04-13 17:52:30.000000 gtFrame-1.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 17:52:40.043404 gtFrame-1.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 17:52:30.000000 gtFrame-1.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:52:40.043404 gtFrame-1.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    48296 2023-04-13 17:52:30.000000 gtFrame-1.2.2/tests/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)    23157 2023-04-13 17:52:30.000000 gtFrame-1.2.2/tests/test_direction.py
--rw-r--r--   0 runner    (1001) docker     (123)    35544 2023-04-13 17:52:30.000000 gtFrame-1.2.2/tests/test_position.py
--rw-r--r--   0 runner    (1001) docker     (123)     7277 2023-04-13 17:52:30.000000 gtFrame-1.2.2/tests/test_rotation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:20:40.463457 gtFrame-1.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-01 18:20:26.000000 gtFrame-1.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-05-01 18:20:40.463457 gtFrame-1.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-01 18:20:26.000000 gtFrame-1.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:20:40.459457 gtFrame-1.2.3/gtFrame/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-01 18:20:26.000000 gtFrame-1.2.3/gtFrame/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23059 2023-05-01 18:20:26.000000 gtFrame-1.2.3/gtFrame/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10282 2023-05-01 18:20:26.000000 gtFrame-1.2.3/gtFrame/direction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14238 2023-05-01 18:20:26.000000 gtFrame-1.2.3/gtFrame/position.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-05-01 18:20:26.000000 gtFrame-1.2.3/gtFrame/rotation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:20:40.459457 gtFrame-1.2.3/gtFrame.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-05-01 18:20:40.000000 gtFrame-1.2.3/gtFrame.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-01 18:20:40.000000 gtFrame-1.2.3/gtFrame.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 18:20:40.000000 gtFrame-1.2.3/gtFrame.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-01 18:20:40.000000 gtFrame-1.2.3/gtFrame.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-01 18:20:40.000000 gtFrame-1.2.3/gtFrame.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-01 18:20:26.000000 gtFrame-1.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 18:20:40.463457 gtFrame-1.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 18:20:26.000000 gtFrame-1.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:20:40.463457 gtFrame-1.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    49544 2023-05-01 18:20:26.000000 gtFrame-1.2.3/tests/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23157 2023-05-01 18:20:26.000000 gtFrame-1.2.3/tests/test_direction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35544 2023-05-01 18:20:26.000000 gtFrame-1.2.3/tests/test_position.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7277 2023-05-01 18:20:26.000000 gtFrame-1.2.3/tests/test_rotation.py
```

### Comparing `gtFrame-1.2.2/LICENSE` & `gtFrame-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gtFrame-1.2.2/PKG-INFO` & `gtFrame-1.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gtFrame
-Version: 1.2.2
+Version: 1.2.3
 Summary: A simple library for working with frames of reference
 Author-email: "Roko Jukic (bluePlatinum)" <jukic.rok@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Roko Jukic. All rights reserved
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `gtFrame-1.2.2/gtFrame/basic.py` & `gtFrame-1.2.3/gtFrame/basic.py`

 * *Files 2% similar despite different names*

```diff
@@ -198,29 +198,29 @@
         """
 
         # ------------------------
         # this frame to the origin
         self_to_origin = list()
         current_frame = self
 
-        while current_frame != origin2d:
+        while not isinstance(current_frame, RootFrame2d):
 
             # check if desired frame is in the branch
             if current_frame == frame:
                 return self_to_origin
 
             self_to_origin.append((current_frame, "to"))
             current_frame = current_frame.parent()
 
         # -------------------------------
         # destination frame to the origin
         frame_to_origin = list()
         current_frame = frame
 
-        while current_frame != origin2d:
+        while not isinstance(current_frame, RootFrame2d):
 
             # check if self frame is on the branch of frame
             if current_frame == self:
                 return frame_to_origin[::-1]        # invert path to flip ends
 
             frame_to_origin.append((current_frame, "from"))
             current_frame = current_frame.parent()
@@ -523,29 +523,29 @@
         :rtype: list
         """
         # ------------------------
         # this frame to the origin
         self_to_origin = list()
         current_frame = self
 
-        while current_frame != origin3d:
+        while not isinstance(current_frame, RootFrame3d):
 
             # check if desired frame is in the branch
             if current_frame == frame:
                 return self_to_origin
 
             self_to_origin.append((current_frame, "to"))
             current_frame = current_frame.parent()
 
         # -------------------------------
         # destination frame to the origin
         frame_to_origin = list()
         current_frame = frame
 
-        while current_frame != origin3d:
+        while not isinstance(current_frame, RootFrame3d):
 
             # check if self frame is on the branch of frame
             if current_frame == self:
                 return frame_to_origin[::-1]        # invert path to flip ends
 
             frame_to_origin.append((current_frame, "from"))
             current_frame = current_frame.parent()
```

### Comparing `gtFrame-1.2.2/gtFrame/direction.py` & `gtFrame-1.2.3/gtFrame/direction.py`

 * *Files identical despite different names*

### Comparing `gtFrame-1.2.2/gtFrame/position.py` & `gtFrame-1.2.3/gtFrame/position.py`

 * *Files identical despite different names*

### Comparing `gtFrame-1.2.2/gtFrame/rotation.py` & `gtFrame-1.2.3/gtFrame/rotation.py`

 * *Files identical despite different names*

### Comparing `gtFrame-1.2.2/gtFrame.egg-info/PKG-INFO` & `gtFrame-1.2.3/gtFrame.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gtFrame
-Version: 1.2.2
+Version: 1.2.3
 Summary: A simple library for working with frames of reference
 Author-email: "Roko Jukic (bluePlatinum)" <jukic.rok@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Roko Jukic. All rights reserved
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `gtFrame-1.2.2/pyproject.toml` & `gtFrame-1.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['setuptools>=61.0']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = 'gtFrame'
-version = '1.2.2'
+version = '1.2.3'
 authors = [
     { name='Roko Jukic (bluePlatinum)', email='jukic.rok@gmail.com'},
 ]
 description = 'A simple library for working with frames of reference'
 readme = 'README.md'
 license = {file='LICENSE'}
 requires-python = '>=3.7'
```

### Comparing `gtFrame-1.2.2/tests/test_basic.py` & `gtFrame-1.2.3/tests/test_basic.py`

 * *Files 2% similar despite different names*

```diff
@@ -418,14 +418,33 @@
         assert path0 == expected0
         assert path1 == expected1
         assert path2 == expected2
         assert path3 == expected3
         assert path4 == expected4
         assert path5 == expected5
 
+    def test_find_transform_path_separate(self):
+        """
+        Test the :meth:`gtFrame.basic.Frame2d.find_transform_path` method by
+        testing with two separate origin objects.
+        """
+        position = np.zeros(2)
+        rotation = Rotation2d(0)
+
+        origin_a = RootFrame2d()
+        origin_b = RootFrame2d()
+        frame_a = Frame2d(position, rotation, parent_frame=origin_a)
+        frame_b = Frame2d(position, rotation, parent_frame=origin_b)
+
+        expected = [(frame_a, 'to'), (frame_b, 'from')]
+
+        path = frame_a.find_transform_path(frame_b)
+
+        assert path == expected
+
     def test_parent(self, random_frame2d):
         """
         Test the .parent method.
 
         :return: None
         """
         position = np.random.random(2)
@@ -1009,14 +1028,33 @@
         assert path0 == expected0
         assert path1 == expected1
         assert path2 == expected2
         assert path3 == expected3
         assert path4 == expected4
         assert path5 == expected5
 
+    def test_find_transform_path_separate(self):
+        """
+        Test the :meth:`gtFrame.basic.Frame2d.find_transform_path` method by
+        testing with two separate origin objects.
+        """
+        position = np.zeros(3)
+        rotation = Rotation3d.from_rotvec(np.zeros(3))
+
+        origin_a = RootFrame3d()
+        origin_b = RootFrame3d()
+        frame_a = Frame3d(position, rotation, parent_frame=origin_a)
+        frame_b = Frame3d(position, rotation, parent_frame=origin_b)
+
+        expected = [(frame_a, 'to'), (frame_b, 'from')]
+
+        path = frame_a.find_transform_path(frame_b)
+
+        assert path == expected
+
     def test_parent(self, random_frame3d):
         """
         Test the .parent method.
 
         :return: None
         """
         position = np.random.random(3)
```

### Comparing `gtFrame-1.2.2/tests/test_direction.py` & `gtFrame-1.2.3/tests/test_direction.py`

 * *Files identical despite different names*

### Comparing `gtFrame-1.2.2/tests/test_position.py` & `gtFrame-1.2.3/tests/test_position.py`

 * *Files identical despite different names*

### Comparing `gtFrame-1.2.2/tests/test_rotation.py` & `gtFrame-1.2.3/tests/test_rotation.py`

 * *Files identical despite different names*

