# Comparing `tmp/gif_pygame-0.0.6.tar.gz` & `tmp/gif_pygame-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gif_pygame-0.0.6.tar", last modified: Mon May  1 02:34:09 2023, max compression
+gzip compressed data, was "gif_pygame-0.0.7.tar", last modified: Mon May  1 02:38:47 2023, max compression
```

## Comparing `gif_pygame-0.0.6.tar` & `gif_pygame-0.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 02:34:09.204635 gif_pygame-0.0.6/
--rw-rw-rw-   0        0        0     1083 2023-03-27 19:37:47.000000 gif_pygame-0.0.6/LICENSE
--rw-rw-rw-   0        0        0     4436 2023-05-01 02:34:09.203636 gif_pygame-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     3452 2023-03-27 21:27:19.000000 gif_pygame-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-05-01 02:34:09.193122 gif_pygame-0.0.6/gif_pygame/
--rw-rw-rw-   0        0        0       50 2023-03-27 21:16:13.000000 gif_pygame-0.0.6/gif_pygame/__init__.py
--rw-rw-rw-   0        0        0    18990 2023-05-01 02:24:47.000000 gif_pygame-0.0.6/gif_pygame/_pygame_gif.py
-drwxrwxrwx   0        0        0        0 2023-05-01 02:34:09.202635 gif_pygame-0.0.6/gif_pygame.egg-info/
--rw-rw-rw-   0        0        0     4436 2023-05-01 02:34:09.000000 gif_pygame-0.0.6/gif_pygame.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      244 2023-05-01 02:34:09.000000 gif_pygame-0.0.6/gif_pygame.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 02:34:09.000000 gif_pygame-0.0.6/gif_pygame.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-05-01 02:34:09.000000 gif_pygame-0.0.6/gif_pygame.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-01 02:34:09.000000 gif_pygame-0.0.6/gif_pygame.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-01 02:34:09.205636 gif_pygame-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1281 2023-05-01 02:33:51.000000 gif_pygame-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 02:38:47.017755 gif_pygame-0.0.7/
+-rw-rw-rw-   0        0        0     1083 2023-03-27 19:37:47.000000 gif_pygame-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0     4436 2023-05-01 02:38:47.015742 gif_pygame-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     3452 2023-03-27 21:27:19.000000 gif_pygame-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-05-01 02:38:47.003222 gif_pygame-0.0.7/gif_pygame/
+-rw-rw-rw-   0        0        0       50 2023-03-27 21:16:13.000000 gif_pygame-0.0.7/gif_pygame/__init__.py
+-rw-rw-rw-   0        0        0    18959 2023-05-01 02:37:59.000000 gif_pygame-0.0.7/gif_pygame/_pygame_gif.py
+drwxrwxrwx   0        0        0        0 2023-05-01 02:38:47.015742 gif_pygame-0.0.7/gif_pygame.egg-info/
+-rw-rw-rw-   0        0        0     4436 2023-05-01 02:38:46.000000 gif_pygame-0.0.7/gif_pygame.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      244 2023-05-01 02:38:46.000000 gif_pygame-0.0.7/gif_pygame.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 02:38:46.000000 gif_pygame-0.0.7/gif_pygame.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-05-01 02:38:46.000000 gif_pygame-0.0.7/gif_pygame.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-01 02:38:46.000000 gif_pygame-0.0.7/gif_pygame.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-01 02:38:47.017755 gif_pygame-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1281 2023-05-01 02:38:28.000000 gif_pygame-0.0.7/setup.py
```

### Comparing `gif_pygame-0.0.6/LICENSE` & `gif_pygame-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `gif_pygame-0.0.6/PKG-INFO` & `gif_pygame-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gif_pygame
-Version: 0.0.6
+Version: 0.0.7
 Summary: A pygame addon for animated image files
 Author: Zeperox
 Keywords: python,pygame,addon,image,animation,animated images
 Classifier: Development Status :: 6 - Mature
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `gif_pygame-0.0.6/README.md` & `gif_pygame-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `gif_pygame-0.0.6/gif_pygame/_pygame_gif.py` & `gif_pygame-0.0.7/gif_pygame/_pygame_gif.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,15 +85,14 @@
         return selected_frames
 
 
     def get_width(self) -> int:
         """
         Returns the width of the .gif/.apng file
         """
-        print(self.frames[0])
         return self.frames[0][0].get_width()
 
     def get_height(self) -> int:
         """
         Returns the height of the .gif/.apng file
         """
         return self.frames[0][0].get_height()
```

### Comparing `gif_pygame-0.0.6/gif_pygame.egg-info/PKG-INFO` & `gif_pygame-0.0.7/gif_pygame.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gif-pygame
-Version: 0.0.6
+Version: 0.0.7
 Summary: A pygame addon for animated image files
 Author: Zeperox
 Keywords: python,pygame,addon,image,animation,animated images
 Classifier: Development Status :: 6 - Mature
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `gif_pygame-0.0.6/setup.py` & `gif_pygame-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', encoding='utf-8') as readme:
     LONG_DESCRIPTION = readme.read()
 
 setup(
     name="gif_pygame",
-    version="0.0.6",
+    version="0.0.7",
     author="Zeperox",
     description="A pygame addon for animated image files",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     install_requires=["pygame-ce", "pillow"],
     keywords=["python", "pygame", "addon", "image", "animation", "animated images"],
```

