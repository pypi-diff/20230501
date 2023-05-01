# Comparing `tmp/gif_pygame-0.0.5.tar.gz` & `tmp/gif_pygame-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gif_pygame-0.0.5.tar", last modified: Tue Mar 28 14:51:15 2023, max compression
+gzip compressed data, was "gif_pygame-0.0.6.tar", last modified: Mon May  1 02:34:09 2023, max compression
```

## Comparing `gif_pygame-0.0.5.tar` & `gif_pygame-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-03-28 14:51:15.419000 gif_pygame-0.0.5/
--rw-rw-rw-   0        0        0     1083 2023-03-27 19:37:47.000000 gif_pygame-0.0.5/LICENSE
--rw-rw-rw-   0        0        0     4436 2023-03-28 14:51:15.415004 gif_pygame-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     3452 2023-03-27 21:27:19.000000 gif_pygame-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-03-28 14:51:15.399975 gif_pygame-0.0.5/gif_pygame/
--rw-rw-rw-   0        0        0       50 2023-03-27 21:16:13.000000 gif_pygame-0.0.5/gif_pygame/__init__.py
--rw-rw-rw-   0        0        0    18971 2023-03-28 14:50:58.000000 gif_pygame-0.0.5/gif_pygame/_pygame_gif.py
-drwxrwxrwx   0        0        0        0 2023-03-28 14:51:15.415004 gif_pygame-0.0.5/gif_pygame.egg-info/
--rw-rw-rw-   0        0        0     4436 2023-03-28 14:51:15.000000 gif_pygame-0.0.5/gif_pygame.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      244 2023-03-28 14:51:15.000000 gif_pygame-0.0.5/gif_pygame.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-28 14:51:15.000000 gif_pygame-0.0.5/gif_pygame.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-03-28 14:51:15.000000 gif_pygame-0.0.5/gif_pygame.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-03-28 14:51:15.000000 gif_pygame-0.0.5/gif_pygame.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-28 14:51:15.419000 gif_pygame-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1281 2023-03-28 14:51:07.000000 gif_pygame-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 02:34:09.204635 gif_pygame-0.0.6/
+-rw-rw-rw-   0        0        0     1083 2023-03-27 19:37:47.000000 gif_pygame-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0     4436 2023-05-01 02:34:09.203636 gif_pygame-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     3452 2023-03-27 21:27:19.000000 gif_pygame-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-05-01 02:34:09.193122 gif_pygame-0.0.6/gif_pygame/
+-rw-rw-rw-   0        0        0       50 2023-03-27 21:16:13.000000 gif_pygame-0.0.6/gif_pygame/__init__.py
+-rw-rw-rw-   0        0        0    18990 2023-05-01 02:24:47.000000 gif_pygame-0.0.6/gif_pygame/_pygame_gif.py
+drwxrwxrwx   0        0        0        0 2023-05-01 02:34:09.202635 gif_pygame-0.0.6/gif_pygame.egg-info/
+-rw-rw-rw-   0        0        0     4436 2023-05-01 02:34:09.000000 gif_pygame-0.0.6/gif_pygame.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      244 2023-05-01 02:34:09.000000 gif_pygame-0.0.6/gif_pygame.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 02:34:09.000000 gif_pygame-0.0.6/gif_pygame.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-05-01 02:34:09.000000 gif_pygame-0.0.6/gif_pygame.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-01 02:34:09.000000 gif_pygame-0.0.6/gif_pygame.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-01 02:34:09.205636 gif_pygame-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1281 2023-05-01 02:33:51.000000 gif_pygame-0.0.6/setup.py
```

### Comparing `gif_pygame-0.0.5/LICENSE` & `gif_pygame-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `gif_pygame-0.0.5/PKG-INFO` & `gif_pygame-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gif_pygame
-Version: 0.0.5
+Version: 0.0.6
 Summary: A pygame addon for animated image files
 Author: Zeperox
 Keywords: python,pygame,addon,image,animation,animated images
 Classifier: Development Status :: 6 - Mature
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `gif_pygame-0.0.5/README.md` & `gif_pygame-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `gif_pygame-0.0.5/gif_pygame/_pygame_gif.py` & `gif_pygame-0.0.6/gif_pygame/_pygame_gif.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,19 +44,19 @@
         self.gif = Image.open(filepath)
 
         self.frames = []
         for frame in range(self.gif.n_frames):
             self.gif.seek(frame)
             if frame == 0:
                 if "duration" in self.gif.info:
-                    self.frames.append((pygame.image.load(filepath), self.gif.info["duration"]*.001))
+                    self.frames.append([pygame.image.load(filepath), self.gif.info["duration"]*.001])
                 else:
-                    self.frames.append((pygame.image.load(filepath), 1))
+                    self.frames.append([pygame.image.load(filepath), 1])
             else:
-                self.frames.append((pygame.image.fromstring(self.gif.tobytes(), self.gif.size, self.gif.mode), self.gif.info["duration"]*.001))
+                self.frames.append([pygame.image.fromstring(self.gif.tobytes(), self.gif.size, self.gif.mode), self.gif.info["duration"]*.001])
         
         self.gif.close()
         self.frame = 0
         self.frame_time = 0
         self.paused_time = 0
         self.paused = False
 
@@ -85,14 +85,15 @@
         return selected_frames
 
 
     def get_width(self) -> int:
         """
         Returns the width of the .gif/.apng file
         """
+        print(self.frames[0])
         return self.frames[0][0].get_width()
 
     def get_height(self) -> int:
         """
         Returns the height of the .gif/.apng file
         """
         return self.frames[0][0].get_height()
@@ -145,21 +146,21 @@
         for index, surface in enumerate(surfaces):
             try:
                 self.frames[surface[1]]
             except:
                 failed_frames.append((index, surface[1]))
                 continue
 
-            if surface not in successful_frames:
+            if surface in successful_frames:
                 duplicated_frames.append((index, surface[1]))
                 continue
 
             else:
                 successful_frames.append(surface)
-                self.frames[surface[1]][0] = surface[1]
+                self.frames[surface[1]][0] = surface[0]
 
         if len(successful_frames) == 0:
             raise IndexError("None of the given frames are in the frames list")
         else:
             if len(failed_frames):
                 failed_str = "There were some failed frames, they were:\n"
                 for failed_frame in failed_frames:
@@ -205,21 +206,21 @@
         for index, duration in enumerate(durations):
             try:
                 self.frames[duration[1]]
             except:
                 failed_frames.append((index, duration[1]))
                 continue
 
-            if duration not in successful_frames:
+            if duration in successful_frames:
                 duplicated_frames.append((index, duration[1]))
                 continue
 
             else:
                 successful_frames.append(duration)
-                self.frames[duration[1]][1] = duration[1]
+                self.frames[duration[1]][1] = duration[0]
 
         if len(successful_frames) == 0:
             raise IndexError("None of the given frames are in the frames list")
         else:
             if len(failed_frames):
                 failed_str = "There were some failed frames, they were:\n"
                 for failed_frame in failed_frames:
@@ -265,15 +266,15 @@
         for index, data in enumerate(datas):
             try:
                 self.frames[data[2]]
             except:
                 failed_frames.append((index, data[2]))
                 continue
 
-            if data not in successful_frames:
+            if data in successful_frames:
                 duplicated_frames.append((index, data[2]))
                 continue
 
             else:
                 successful_frames.append(data)
                 self.frames[data[2]][0] = data[0]
                 self.frames[data[2]][1] = data[1]
```

### Comparing `gif_pygame-0.0.5/gif_pygame.egg-info/PKG-INFO` & `gif_pygame-0.0.6/gif_pygame.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gif-pygame
-Version: 0.0.5
+Version: 0.0.6
 Summary: A pygame addon for animated image files
 Author: Zeperox
 Keywords: python,pygame,addon,image,animation,animated images
 Classifier: Development Status :: 6 - Mature
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `gif_pygame-0.0.5/setup.py` & `gif_pygame-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', encoding='utf-8') as readme:
     LONG_DESCRIPTION = readme.read()
 
 setup(
     name="gif_pygame",
-    version="0.0.5",
+    version="0.0.6",
     author="Zeperox",
     description="A pygame addon for animated image files",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     install_requires=["pygame-ce", "pillow"],
     keywords=["python", "pygame", "addon", "image", "animation", "animated images"],
```

