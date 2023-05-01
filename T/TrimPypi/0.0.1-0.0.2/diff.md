# Comparing `tmp/TrimPypi-0.0.1.tar.gz` & `tmp/TrimPypi-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TrimPypi-0.0.1.tar", last modified: Mon May  1 03:21:56 2023, max compression
+gzip compressed data, was "TrimPypi-0.0.2.tar", last modified: Mon May  1 03:34:04 2023, max compression
```

## Comparing `TrimPypi-0.0.1.tar` & `TrimPypi-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 03:21:56.711516 TrimPypi-0.0.1/
--rw-rw-rw-   0        0        0     1064 2023-05-01 02:59:55.000000 TrimPypi-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     1093 2023-05-01 03:21:56.710550 TrimPypi-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      166 2023-05-01 03:02:22.000000 TrimPypi-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-01 03:21:56.701812 TrimPypi-0.0.1/TrimPypi/
--rw-rw-rw-   0        0        0       66 2023-05-01 03:21:52.000000 TrimPypi-0.0.1/TrimPypi/__init__.py
--rw-rw-rw-   0        0        0     2796 2023-05-01 03:14:12.000000 TrimPypi-0.0.1/TrimPypi/main.py
-drwxrwxrwx   0        0        0        0 2023-05-01 03:21:56.708520 TrimPypi-0.0.1/TrimPypi.egg-info/
--rw-rw-rw-   0        0        0     1093 2023-05-01 03:21:56.000000 TrimPypi-0.0.1/TrimPypi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      192 2023-05-01 03:21:56.000000 TrimPypi-0.0.1/TrimPypi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 03:21:56.000000 TrimPypi-0.0.1/TrimPypi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-01 03:21:56.000000 TrimPypi-0.0.1/TrimPypi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-01 03:21:56.711516 TrimPypi-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1571 2023-05-01 03:21:55.000000 TrimPypi-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 03:34:04.966803 TrimPypi-0.0.2/
+-rw-rw-rw-   0        0        0     1064 2023-05-01 02:59:55.000000 TrimPypi-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     1093 2023-05-01 03:34:04.965803 TrimPypi-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      166 2023-05-01 03:02:22.000000 TrimPypi-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-01 03:34:04.957021 TrimPypi-0.0.2/TrimPypi/
+-rw-rw-rw-   0        0        0       90 2023-05-01 03:34:00.000000 TrimPypi-0.0.2/TrimPypi/__init__.py
+-rw-rw-rw-   0        0        0     2852 2023-05-01 03:31:21.000000 TrimPypi-0.0.2/TrimPypi/main.py
+drwxrwxrwx   0        0        0        0 2023-05-01 03:34:04.964801 TrimPypi-0.0.2/TrimPypi.egg-info/
+-rw-rw-rw-   0        0        0     1093 2023-05-01 03:34:04.000000 TrimPypi-0.0.2/TrimPypi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      192 2023-05-01 03:34:04.000000 TrimPypi-0.0.2/TrimPypi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 03:34:04.000000 TrimPypi-0.0.2/TrimPypi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-01 03:34:04.000000 TrimPypi-0.0.2/TrimPypi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-01 03:34:04.966803 TrimPypi-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1387 2023-05-01 03:34:00.000000 TrimPypi-0.0.2/setup.py
```

### Comparing `TrimPypi-0.0.1/LICENSE` & `TrimPypi-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `TrimPypi-0.0.1/PKG-INFO` & `TrimPypi-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TrimPypi
-Version: 0.0.1
+Version: 0.0.2
 Summary: Pypi上传工具本地配套文件初始化管理。
 Home-page: https://github.com/TriM-Organization/TrimPypi
 Author: bgArray
 Author-email: TriM-Organization@hotmail.com
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `TrimPypi-0.0.1/TrimPypi/main.py` & `TrimPypi-0.0.2/TrimPypi/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 def set_bat():
-    with open("upload.bat", "w") as w:
+    with open("upload.bat", "w", encoding="utf-8") as w:
         w.write("""python setup.py sdist bdist_wheel
 python -m twine upload dist/*
 python clean_update.py
 """)
 
 
 def set_clean_update():
-    with open("clean_update.py", "w") as w:
+    with open("clean_update.py", "w", encoding="utf-8") as w:
         w.write("""import shutil
 import os
 from rich.console import Console
 from rich.progress import track
 
 console = Console()
 
@@ -30,33 +30,33 @@
 
 if __name__ == "__main__":
     main()
 """)
 
 
 def set_setup():
-    with open("setup.py", "w") as w:
+    with open("setup.py", "w", encoding="utf-8") as w:
         w.write("""# -*- coding: utf-8 -*-
 import setuptools
 import Musicreater
 
 with open("requirements.txt", "r", encoding="utf-8") as fh:
-    dependences = fh.read().strip().split("\n")
+    dependences = fh.read().strip().split("\\n")
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read().replace(
         "./docs/", "https://github.com/TriM-Organization/Musicreater/blob/master/docs/"
     )
 
 setuptools.setup(
     name="Musicreater",
     version=Musicreater.__version__,
     author="Eilles Wan, bgArray",
     author_email="TriM-Organization@hotmail.com",
-    description="一款免费开源的 《我的世界》 mid音乐转换库。\n"
+    description="一款免费开源的 《我的世界》 mid音乐转换库。\\n"
     "A free open-source python library used to convert midi into Minecraft.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/TriM-Organization/Musicreater",
     packages=setuptools.find_packages(),
     classifiers=[
         "Intended Audience :: Developers",
```

### Comparing `TrimPypi-0.0.1/TrimPypi.egg-info/PKG-INFO` & `TrimPypi-0.0.2/TrimPypi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TrimPypi
-Version: 0.0.1
+Version: 0.0.2
 Summary: Pypi上传工具本地配套文件初始化管理。
 Home-page: https://github.com/TriM-Organization/TrimPypi
 Author: bgArray
 Author-email: TriM-Organization@hotmail.com
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `TrimPypi-0.0.1/setup.py` & `TrimPypi-0.0.2/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,31 +1,26 @@
 # -*- coding: utf-8 -*-
 import setuptools
-import Musicreater
-
-with open("requirements.txt", "r", encoding="utf-8") as fh:
-    dependences = fh.read().strip().split("
-")
+import TrimPypi
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read().replace(
-        "./docs/", "https://github.com/TriM-Organization/Musicreater/blob/master/docs/"
+        "./docs/", "https://github.com/TriM-Organization/TrimPypi/blob/master/README.md"
     )
 
 setuptools.setup(
-    name="Musicreater",
-    version=Musicreater.__version__,
-    author="Eilles Wan, bgArray",
+    name="TrimPypi",
+    version=TrimPypi.__version__,
+    author="bgArray",
     author_email="TriM-Organization@hotmail.com",
-    description="Ò»¿îÃâ·Ñ¿ªÔ´µÄ ¡¶ÎÒµÄÊÀ½ç¡· midÒôÀÖ×ª»»¿â¡£
-"
-    "A free open-source python library used to convert midi into Minecraft.",
+    description="Pypi上传工具本地配套文件初始化管理。\n"
+    "Local supporting file initialization management for Pypi upload tool.",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/TriM-Organization/Musicreater",
+    url="https://github.com/TriM-Organization/TrimPypi",
     packages=setuptools.find_packages(),
     classifiers=[
         "Intended Audience :: Developers",
         "Natural Language :: Chinese (Simplified)",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
         "Topic :: Software Development :: Libraries",
@@ -33,10 +28,8 @@
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
     ],
-    # ÐèÒª°²×°µÄÒÀÀµ
-    install_requires=dependences,
 )
```

#### encoding

```diff
@@ -1 +1 @@
-iso-8859-1
+utf-8
```

