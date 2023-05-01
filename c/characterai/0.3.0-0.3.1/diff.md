# Comparing `tmp/characterai-0.3.0.tar.gz` & `tmp/characterai-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\characterai-0.3.0.tar", last modified: Mon May  1 09:41:55 2023, max compression
+gzip compressed data, was "dist\characterai-0.3.1.tar", last modified: Mon May  1 15:30:08 2023, max compression
```

## Comparing `characterai-0.3.0.tar` & `characterai-0.3.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 09:41:55.613721 characterai-0.3.0/
--rw-rw-rw-   0        0        0     1082 2023-04-28 16:51:34.000000 characterai-0.3.0/LICENSE
--rw-rw-rw-   0        0        0     1960 2023-05-01 09:41:55.612721 characterai-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     1525 2023-05-01 09:40:37.000000 characterai-0.3.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-01 09:41:55.560896 characterai-0.3.0/characterai/
--rw-rw-rw-   0        0        0       90 2023-04-29 10:41:38.000000 characterai-0.3.0/characterai/__init__.py
--rw-rw-rw-   0        0        0     5640 2023-05-01 09:39:20.000000 characterai-0.3.0/characterai/characterai.py
--rw-rw-rw-   0        0        0      126 2023-04-28 20:05:16.000000 characterai-0.3.0/characterai/errors.py
--rw-rw-rw-   0        0        0     5070 2023-05-01 09:33:52.000000 characterai-0.3.0/characterai/pyasynccai.py
-drwxrwxrwx   0        0        0        0 2023-05-01 09:41:55.608720 characterai-0.3.0/characterai.egg-info/
--rw-rw-rw-   0        0        0     1960 2023-05-01 09:41:55.000000 characterai-0.3.0/characterai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      299 2023-05-01 09:41:55.000000 characterai-0.3.0/characterai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 09:41:55.000000 characterai-0.3.0/characterai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-05-01 09:41:55.000000 characterai-0.3.0/characterai.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-01 09:41:55.000000 characterai-0.3.0/characterai.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-01 09:41:55.614722 characterai-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0      615 2023-05-01 09:40:11.000000 characterai-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 15:30:08.236988 characterai-0.3.1/
+-rw-rw-rw-   0        0        0     1082 2023-04-28 16:51:34.000000 characterai-0.3.1/LICENSE
+-rw-rw-rw-   0        0        0      453 2023-05-01 15:30:08.235988 characterai-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1481 2023-05-01 15:25:41.000000 characterai-0.3.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-01 15:30:08.195987 characterai-0.3.1/characterai/
+-rw-rw-rw-   0        0        0       90 2023-04-29 10:41:38.000000 characterai-0.3.1/characterai/__init__.py
+-rw-rw-rw-   0        0        0     5640 2023-05-01 09:39:20.000000 characterai-0.3.1/characterai/characterai.py
+-rw-rw-rw-   0        0        0      126 2023-04-28 20:05:16.000000 characterai-0.3.1/characterai/errors.py
+-rw-rw-rw-   0        0        0     5070 2023-05-01 09:33:52.000000 characterai-0.3.1/characterai/pyasynccai.py
+drwxrwxrwx   0        0        0        0 2023-05-01 15:30:08.231989 characterai-0.3.1/characterai.egg-info/
+-rw-rw-rw-   0        0        0      453 2023-05-01 15:30:07.000000 characterai-0.3.1/characterai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      299 2023-05-01 15:30:08.000000 characterai-0.3.1/characterai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 15:30:07.000000 characterai-0.3.1/characterai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-05-01 15:30:08.000000 characterai-0.3.1/characterai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-01 15:30:08.000000 characterai-0.3.1/characterai.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-01 15:30:08.237989 characterai-0.3.1/setup.cfg
+-rw-rw-rw-   0        0        0      558 2023-05-01 15:29:32.000000 characterai-0.3.1/setup.py
```

### Comparing `characterai-0.3.0/LICENSE` & `characterai-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `characterai-0.3.0/README.md` & `characterai-0.3.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-# 💬 CharacterAI
+# CharacterAI
 
 An unofficial API for Character AI for Python using Playwright
 
-## 💻 Installation
+## Installation
 ```bash
 pip install characterai
 ```
 
-## 🔐 Get TOKEN
+## Get TOKEN
 For using library, you should get token
 1. Log in on character.ai
 2. Go to `Network` tab in DevTools and refresh page
 3. Search `/dj-rest-auth/auth0/`
 4. Copy `key` value
 
-## 🔐 Get CHAR
+## Get CHAR
 This is a character ID, it's very easy to get it
 1. Open any chat
 2. Copy `char=` value from URL
 
-## 📙 Example
+## Example
 #### Chatting
 Simple program for chatting with character
 ```Python
 from characterai import pyCAI
 
 token = 'TOKEN'
 character = 'CHAR'
@@ -31,15 +31,15 @@
 client = pyCAI(token)
 
 while True:
     send = input('You: ')
     print(f'Character: {client.chat.send_message(character, send)}')
 ```
 
-## 📚 Functions
+## Functions
 ### user
 For information about the user, namely about you via a token, the answer is json
 ```python
 user.info()
 user.posts()
 user.followers()
 user.following()
@@ -55,14 +55,14 @@
 ### chat
 To work with the chat, `get_history` answer is json
 ```python
 chat.get_history('CHAR')
 chat.send_message('CHAR', 'YOUR MESSAGE')
 ```
 
-## ⭐️ Features
+## Features
 - The only library for character.ai
 - Asynchronous
 - So easy to use
 
-## ⚠️ Disclaimer
+## Disclaimer
 This library is written by a beginner in python, if you have any problems, write to me in [Telegram](https://t.me/kramcat)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `characterai-0.3.0/characterai/characterai.py` & `characterai-0.3.1/characterai/characterai.py`

 * *Files identical despite different names*

### Comparing `characterai-0.3.0/characterai/pyasynccai.py` & `characterai-0.3.1/characterai/pyasynccai.py`

 * *Files identical despite different names*

### Comparing `characterai-0.3.0/setup.py` & `characterai-0.3.1/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 from setuptools import setup, find_packages
 
-with open('README.md') as readme:
-    long_description = readme.read()
-
 setup(
     name='characterai',
-    version='0.3.0',
+    version='0.3.1',
     author='kramcat',
     description='An unofficial API for character.ai for Python',
-    long_description=long_description,
+    long_description=open('README.md', encoding="utf8"),
     long_description_content_type='text/markdown',
     url='https://github.com/kramcat/characterai',
     packages=find_packages(),
     install_requires=["playwright>=1.32.1"],
     classifiers=[
         'Programming Language :: Python :: 3.9',
         'License :: OSI Approved :: MIT License',
```

