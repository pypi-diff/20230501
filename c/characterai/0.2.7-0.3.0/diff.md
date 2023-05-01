# Comparing `tmp/characterai-0.2.7.tar.gz` & `tmp/characterai-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "characterai-0.2.7.tar", last modified: Sat Apr 29 20:07:49 2023, max compression
+gzip compressed data, was "dist\characterai-0.3.0.tar", last modified: Mon May  1 09:41:55 2023, max compression
```

## Comparing `characterai-0.2.7.tar` & `characterai-0.3.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 20:07:49.769737 characterai-0.2.7/
--rw-r--r--   0 root         (0) root         (0)     1082 2023-04-29 18:28:44.000000 characterai-0.2.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1834 2023-04-29 20:07:49.769737 characterai-0.2.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1525 2023-04-29 18:28:44.000000 characterai-0.2.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 20:07:49.769737 characterai-0.2.7/characterai/
--rw-r--r--   0 root         (0) root         (0)       90 2023-04-29 18:28:44.000000 characterai-0.2.7/characterai/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9356 2023-04-29 18:32:10.000000 characterai-0.2.7/characterai/characterai.py
--rw-r--r--   0 root         (0) root         (0)      126 2023-04-29 18:28:44.000000 characterai-0.2.7/characterai/errors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 20:07:49.769737 characterai-0.2.7/characterai.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1834 2023-04-29 20:07:49.000000 characterai-0.2.7/characterai.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      273 2023-04-29 20:07:49.000000 characterai-0.2.7/characterai.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-29 20:07:49.000000 characterai-0.2.7/characterai.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-04-29 20:07:49.000000 characterai-0.2.7/characterai.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-04-29 20:07:49.000000 characterai-0.2.7/characterai.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-29 20:07:49.769737 characterai-0.2.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      602 2023-04-29 20:06:40.000000 characterai-0.2.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 09:41:55.613721 characterai-0.3.0/
+-rw-rw-rw-   0        0        0     1082 2023-04-28 16:51:34.000000 characterai-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0     1960 2023-05-01 09:41:55.612721 characterai-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1525 2023-05-01 09:40:37.000000 characterai-0.3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-01 09:41:55.560896 characterai-0.3.0/characterai/
+-rw-rw-rw-   0        0        0       90 2023-04-29 10:41:38.000000 characterai-0.3.0/characterai/__init__.py
+-rw-rw-rw-   0        0        0     5640 2023-05-01 09:39:20.000000 characterai-0.3.0/characterai/characterai.py
+-rw-rw-rw-   0        0        0      126 2023-04-28 20:05:16.000000 characterai-0.3.0/characterai/errors.py
+-rw-rw-rw-   0        0        0     5070 2023-05-01 09:33:52.000000 characterai-0.3.0/characterai/pyasynccai.py
+drwxrwxrwx   0        0        0        0 2023-05-01 09:41:55.608720 characterai-0.3.0/characterai.egg-info/
+-rw-rw-rw-   0        0        0     1960 2023-05-01 09:41:55.000000 characterai-0.3.0/characterai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      299 2023-05-01 09:41:55.000000 characterai-0.3.0/characterai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 09:41:55.000000 characterai-0.3.0/characterai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-05-01 09:41:55.000000 characterai-0.3.0/characterai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-01 09:41:55.000000 characterai-0.3.0/characterai.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-01 09:41:55.614722 characterai-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0      615 2023-05-01 09:40:11.000000 characterai-0.3.0/setup.py
```

### Comparing `characterai-0.2.7/LICENSE` & `characterai-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `characterai-0.2.7/README.md` & `characterai-0.3.0/README.md`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # 💬 CharacterAI
+
 An unofficial API for Character AI for Python using Playwright
 
 ## 💻 Installation
 ```bash
 pip install characterai
 ```
 
@@ -61,8 +62,7 @@
 ## ⭐️ Features
 - The only library for character.ai
 - Asynchronous
 - So easy to use
 
 ## ⚠️ Disclaimer
 This library is written by a beginner in python, if you have any problems, write to me in [Telegram](https://t.me/kramcat)
-
```

### Comparing `characterai-0.2.7/setup.py` & `characterai-0.3.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-from setuptools import setup
+from setuptools import setup, find_packages
 
 with open('README.md') as readme:
     long_description = readme.read()
 
 setup(
     name='characterai',
-    version='0.2.7',
+    version='0.3.0',
     author='kramcat',
     description='An unofficial API for character.ai for Python',
     long_description=long_description,
     long_description_content_type='text/markdown',
-    url='https://github.com/kramcat/CharacterAI',
-    packages=['characterai'],
-    install_requires=['playwright==1.32.1'],
+    url='https://github.com/kramcat/characterai',
+    packages=find_packages(),
+    install_requires=["playwright>=1.32.1"],
     classifiers=[
         'Programming Language :: Python :: 3.9',
         'License :: OSI Approved :: MIT License',
     ],
-)
+)
```

