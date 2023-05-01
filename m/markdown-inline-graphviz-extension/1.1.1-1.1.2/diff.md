# Comparing `tmp/markdown_inline_graphviz_extension-1.1.1.tar.gz` & `tmp/markdown_inline_graphviz_extension-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "markdown_inline_graphviz_extension-1.1.1.tar", last modified: Wed Jul 27 16:56:48 2022, max compression
+gzip compressed data, was "markdown_inline_graphviz_extension-1.1.2.tar", last modified: Mon May  1 13:18:26 2023, max compression
```

## Comparing `markdown_inline_graphviz_extension-1.1.1.tar` & `markdown_inline_graphviz_extension-1.1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-27 16:56:48.971367 markdown_inline_graphviz_extension-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1058 2022-07-27 16:56:39.000000 markdown_inline_graphviz_extension-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      929 2022-07-27 16:56:48.971367 markdown_inline_graphviz_extension-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1957 2022-07-27 16:56:39.000000 markdown_inline_graphviz_extension-1.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     3976 2022-07-27 16:56:39.000000 markdown_inline_graphviz_extension-1.1.1/markdown_inline_graphviz.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-27 16:56:48.971367 markdown_inline_graphviz_extension-1.1.1/markdown_inline_graphviz_extension.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      929 2022-07-27 16:56:48.000000 markdown_inline_graphviz_extension-1.1.1/markdown_inline_graphviz_extension.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      343 2022-07-27 16:56:48.000000 markdown_inline_graphviz_extension-1.1.1/markdown_inline_graphviz_extension.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-27 16:56:48.000000 markdown_inline_graphviz_extension-1.1.1/markdown_inline_graphviz_extension.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-07-27 16:56:48.000000 markdown_inline_graphviz_extension-1.1.1/markdown_inline_graphviz_extension.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-07-27 16:56:48.000000 markdown_inline_graphviz_extension-1.1.1/markdown_inline_graphviz_extension.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-07-27 16:56:48.971367 markdown_inline_graphviz_extension-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1848 2022-07-27 16:56:39.000000 markdown_inline_graphviz_extension-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 13:18:26.935051 markdown_inline_graphviz_extension-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-01 13:18:08.000000 markdown_inline_graphviz_extension-1.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-05-01 13:18:26.935051 markdown_inline_graphviz_extension-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-05-01 13:18:08.000000 markdown_inline_graphviz_extension-1.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3927 2023-05-01 13:18:08.000000 markdown_inline_graphviz_extension-1.1.2/markdown_inline_graphviz.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 13:18:26.935051 markdown_inline_graphviz_extension-1.1.2/markdown_inline_graphviz_extension.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-05-01 13:18:26.000000 markdown_inline_graphviz_extension-1.1.2/markdown_inline_graphviz_extension.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-01 13:18:26.000000 markdown_inline_graphviz_extension-1.1.2/markdown_inline_graphviz_extension.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 13:18:26.000000 markdown_inline_graphviz_extension-1.1.2/markdown_inline_graphviz_extension.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-01 13:18:26.000000 markdown_inline_graphviz_extension-1.1.2/markdown_inline_graphviz_extension.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-01 13:18:26.000000 markdown_inline_graphviz_extension-1.1.2/markdown_inline_graphviz_extension.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 13:18:26.935051 markdown_inline_graphviz_extension-1.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-05-01 13:18:08.000000 markdown_inline_graphviz_extension-1.1.2/setup.py
```

### Comparing `markdown_inline_graphviz_extension-1.1.1/LICENSE` & `markdown_inline_graphviz_extension-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `markdown_inline_graphviz_extension-1.1.1/PKG-INFO` & `markdown_inline_graphviz_extension-1.1.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: markdown_inline_graphviz_extension
-Version: 1.1.1
+Version: 1.1.2
 Summary: Render inline graphs with Markdown and Graphviz (python3 version)
 Home-page: https://github.com/cesaremorel/markdown-inline-graphviz
 Author: Cesar Morel
 Author-email: cesaremoreln@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Documentation
 Classifier: Topic :: Text Processing
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
+Description-Content-Type: text/markdown
 License-File: LICENSE
 
 This is just a continuation of the great job of Steffen Prince (sprin/markdown-inline-graphviz) in order to get it work with pip3. If you use python 2, please use the original extension instead.
```

### Comparing `markdown_inline_graphviz_extension-1.1.1/README.md` & `markdown_inline_graphviz_extension-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `markdown_inline_graphviz_extension-1.1.1/markdown_inline_graphviz.py` & `markdown_inline_graphviz_extension-1.1.2/markdown_inline_graphviz.py`

 * *Files 5% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         text = "\n".join(lines)
         while 1:
             m = BLOCK_RE_CURLY_BRACKET.search(text) if BLOCK_RE_CURLY_BRACKET.search(text) else BLOCK_RE_GRAVE_ACCENT.search(text)
             if m:
                 command = m.group('command')
                 # Whitelist command, prevent command injection.
                 if command not in SUPPORTED_COMMAMDS:
-                    raise Exception('Command not supported: %s' % command)
+                    break
                 filename = m.group('filename')
                 content = m.group('content')
                 filetype = filename[filename.rfind('.')+1:]
 
                 args = [command, '-T'+filetype]
                 try:
                     proc = subprocess.Popen(
```

### Comparing `markdown_inline_graphviz_extension-1.1.1/markdown_inline_graphviz_extension.egg-info/PKG-INFO` & `markdown_inline_graphviz_extension-1.1.2/markdown_inline_graphviz_extension.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: markdown-inline-graphviz-extension
-Version: 1.1.1
+Version: 1.1.2
 Summary: Render inline graphs with Markdown and Graphviz (python3 version)
 Home-page: https://github.com/cesaremorel/markdown-inline-graphviz
 Author: Cesar Morel
 Author-email: cesaremoreln@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Documentation
 Classifier: Topic :: Text Processing
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
+Description-Content-Type: text/markdown
 License-File: LICENSE
 
 This is just a continuation of the great job of Steffen Prince (sprin/markdown-inline-graphviz) in order to get it work with pip3. If you use python 2, please use the original extension instead.
```

### Comparing `markdown_inline_graphviz_extension-1.1.1/setup.py` & `markdown_inline_graphviz_extension-1.1.2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 import sys
 from setuptools import setup
 
-VERSION = '1.1.1'
+VERSION = '1.1.2'
 
 if sys.argv[-1] == 'publish':
     if os.system("pip freeze | grep wheel"):
         print("wheel not installed.\nUse `pip install wheel`.\nExiting.")
         sys.exit()
     if os.system("pip freeze | grep twine"):
         print("twine not installed.\nUse `pip install twine`.\nExiting.")
@@ -23,14 +23,15 @@
     version=VERSION,
     py_modules=["markdown_inline_graphviz"],
     install_requires=['Markdown>=2.3.1'],
     author="Cesar Morel",
     author_email="cesaremoreln@gmail.com",
     description="Render inline graphs with Markdown and Graphviz (python3 version)",
     long_description="This is just a continuation of the great job of Steffen Prince (sprin/markdown-inline-graphviz) in order to get it work with pip3. If you use python 2, please use the original extension instead.",
+    long_description_content_type="text/markdown",
     license="MIT",
     url="https://github.com/cesaremorel/markdown-inline-graphviz",
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'Topic :: Documentation',
         'Topic :: Text Processing',
```

