# Comparing `tmp/client_GPT-1.1.3.tar.gz` & `tmp/client_GPT-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "client_GPT-1.1.3.tar", last modified: Mon May  1 12:57:09 2023, max compression
+gzip compressed data, was "client_GPT-1.1.4.tar", last modified: Mon May  1 15:33:55 2023, max compression
```

## Comparing `client_GPT-1.1.3.tar` & `client_GPT-1.1.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 12:57:09.970694 client_GPT-1.1.3/
--rw-rw-rw-   0        0        0      419 2023-05-01 12:57:09.969706 client_GPT-1.1.3/PKG-INFO
--rw-rw-rw-   0        0        0      425 2023-04-27 14:12:47.000000 client_GPT-1.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-01 12:57:09.961713 client_GPT-1.1.3/client_GPT.egg-info/
--rw-rw-rw-   0        0        0      419 2023-05-01 12:57:09.000000 client_GPT-1.1.3/client_GPT.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      235 2023-05-01 12:57:09.000000 client_GPT-1.1.3/client_GPT.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 12:57:09.000000 client_GPT-1.1.3/client_GPT.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-01 12:57:09.000000 client_GPT-1.1.3/client_GPT.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-01 12:57:09.000000 client_GPT-1.1.3/client_GPT.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-01 12:57:09.965693 client_GPT-1.1.3/client_gpt/
--rw-rw-rw-   0        0        0        0 2023-04-27 13:20:09.000000 client_GPT-1.1.3/client_gpt/__init__.py
--rw-rw-rw-   0        0        0     3925 2023-05-01 12:48:07.000000 client_GPT-1.1.3/client_gpt/client_gpt.py
--rw-rw-rw-   0        0        0       42 2023-05-01 12:57:09.971709 client_GPT-1.1.3/setup.cfg
--rw-rw-rw-   0        0        0      591 2023-05-01 12:56:47.000000 client_GPT-1.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 15:33:54.999318 client_GPT-1.1.4/
+-rw-rw-rw-   0        0        0      419 2023-05-01 15:33:54.998322 client_GPT-1.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0      425 2023-04-27 14:12:47.000000 client_GPT-1.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-01 15:33:54.979321 client_GPT-1.1.4/client_GPT.egg-info/
+-rw-rw-rw-   0        0        0      419 2023-05-01 15:33:54.000000 client_GPT-1.1.4/client_GPT.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      235 2023-05-01 15:33:54.000000 client_GPT-1.1.4/client_GPT.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 15:33:54.000000 client_GPT-1.1.4/client_GPT.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-01 15:33:54.000000 client_GPT-1.1.4/client_GPT.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-01 15:33:54.000000 client_GPT-1.1.4/client_GPT.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-01 15:33:54.996321 client_GPT-1.1.4/client_gpt/
+-rw-rw-rw-   0        0        0        0 2023-04-27 13:20:09.000000 client_GPT-1.1.4/client_gpt/__init__.py
+-rw-rw-rw-   0        0        0     3946 2023-05-01 15:33:38.000000 client_GPT-1.1.4/client_gpt/client_gpt.py
+-rw-rw-rw-   0        0        0       42 2023-05-01 15:33:54.999318 client_GPT-1.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      591 2023-05-01 15:33:48.000000 client_GPT-1.1.4/setup.py
```

### Comparing `client_GPT-1.1.3/client_gpt/client_gpt.py` & `client_GPT-1.1.4/client_gpt/client_gpt.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,16 +13,16 @@
         api_key (str): Your OpenAI API key.
         model (str): The ID of the GPT-3 model to use.
         conversation_id (str or None): the unique identifier of the current conversation in the OpenAI. If the value is None, a new conversation ID will be created. If a string is passed, then an existing conversation ID is used.
         session (requests.Session): A session object for making HTTP requests.
     Method:
         ask(prompt, conversation_id=None, previous_convo_id=None): Sends a prompt to the OpenAI API and returns the response.
     """
-
-    chat_api_url = "https://api.openai.com/v1/chat/completions"
+    
+    chat_api_url = "https://api.openai.com/v1/engines/davinci-codex/completions"
 
     def __init__(self, api_key: str, model: str):
         self.api_key = api_key
         self.model = model
         self.conversation_id = None
         self.session = requests.Session()
```

### Comparing `client_GPT-1.1.3/setup.py` & `client_GPT-1.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="client_GPT",
-    version="1.1.3",
+    version="1.1.4",
     author="littleknitsstory",
     description="A package for working with GPT language models.",
     url="https://github.com/littleknitsstory/client-gpt",
     packages=setuptools.find_packages(),
     install_requires=[
         "requests",
     ],
```

