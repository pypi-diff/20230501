# Comparing `tmp/client_GPT-1.1.1.tar.gz` & `tmp/client_GPT-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "client_GPT-1.1.1.tar", last modified: Thu Apr 27 13:26:52 2023, max compression
+gzip compressed data, was "client_GPT-1.1.2.tar", last modified: Mon May  1 12:51:25 2023, max compression
```

## Comparing `client_GPT-1.1.1.tar` & `client_GPT-1.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 13:26:52.228534 client_GPT-1.1.1/
--rw-rw-rw-   0        0        0      419 2023-04-27 13:26:52.227534 client_GPT-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      330 2023-04-24 09:17:30.000000 client_GPT-1.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-27 13:26:52.221536 client_GPT-1.1.1/client_GPT.egg-info/
--rw-rw-rw-   0        0        0      419 2023-04-27 13:26:52.000000 client_GPT-1.1.1/client_GPT.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      235 2023-04-27 13:26:52.000000 client_GPT-1.1.1/client_GPT.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 13:26:52.000000 client_GPT-1.1.1/client_GPT.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-27 13:26:52.000000 client_GPT-1.1.1/client_GPT.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-27 13:26:52.000000 client_GPT-1.1.1/client_GPT.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-27 13:26:52.225535 client_GPT-1.1.1/client_gpt/
--rw-rw-rw-   0        0        0        0 2023-04-27 13:20:09.000000 client_GPT-1.1.1/client_gpt/__init__.py
--rw-rw-rw-   0        0        0     3891 2023-04-24 10:31:04.000000 client_GPT-1.1.1/client_gpt/client_gpt.py
--rw-rw-rw-   0        0        0       42 2023-04-27 13:26:52.228534 client_GPT-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0      591 2023-04-27 13:26:47.000000 client_GPT-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 12:51:25.326703 client_GPT-1.1.2/
+-rw-rw-rw-   0        0        0      419 2023-05-01 12:51:25.326703 client_GPT-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      425 2023-04-27 14:12:47.000000 client_GPT-1.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-01 12:51:25.308704 client_GPT-1.1.2/client_GPT.egg-info/
+-rw-rw-rw-   0        0        0      419 2023-05-01 12:51:24.000000 client_GPT-1.1.2/client_GPT.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      235 2023-05-01 12:51:24.000000 client_GPT-1.1.2/client_GPT.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 12:51:24.000000 client_GPT-1.1.2/client_GPT.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-01 12:51:24.000000 client_GPT-1.1.2/client_GPT.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-01 12:51:24.000000 client_GPT-1.1.2/client_GPT.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-01 12:51:25.324701 client_GPT-1.1.2/client_gpt/
+-rw-rw-rw-   0        0        0        0 2023-04-27 13:20:09.000000 client_GPT-1.1.2/client_gpt/__init__.py
+-rw-rw-rw-   0        0        0     3925 2023-05-01 12:48:07.000000 client_GPT-1.1.2/client_gpt/client_gpt.py
+-rw-rw-rw-   0        0        0       42 2023-05-01 12:51:25.327700 client_GPT-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      591 2023-05-01 12:50:42.000000 client_GPT-1.1.2/setup.py
```

### Comparing `client_GPT-1.1.1/client_gpt/client_gpt.py` & `client_GPT-1.1.2/client_gpt/client_gpt.py`

 * *Files 13% similar despite different names*

```diff
@@ -14,14 +14,16 @@
         model (str): The ID of the GPT-3 model to use.
         conversation_id (str or None): the unique identifier of the current conversation in the OpenAI. If the value is None, a new conversation ID will be created. If a string is passed, then an existing conversation ID is used.
         session (requests.Session): A session object for making HTTP requests.
     Method:
         ask(prompt, conversation_id=None, previous_convo_id=None): Sends a prompt to the OpenAI API and returns the response.
     """
 
+    chat_api_url = "https://api.openai.com/v1/chat/completions"
+
     def __init__(self, api_key: str, model: str):
         self.api_key = api_key
         self.model = model
         self.conversation_id = None
         self.session = requests.Session()
 
     def ask(
@@ -53,15 +55,15 @@
             previous_convo_id = str(uuid.uuid4())
 
         if conversation_id is not None and len(conversation_id) == 0:
             conversation_id = None
 
         try:
             response = self.session.post(
-                "https://chat.openai.com/backend-api/conversation",
+                self.chat_api_url,
                 headers=headers,
                 data=json.dumps(data),
             )
             if response.status_code == 200:
                 response_text = response.text.replace("data: [DONE]", "")
                 data = re.findall(r"data: (.*)", response_text)[-1]
                 as_json = json.loads(data)
```

### Comparing `client_GPT-1.1.1/setup.py` & `client_GPT-1.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="client_GPT",
-    version="1.1.1",
+    version="1.1.2",
     author="littleknitsstory",
     description="A package for working with GPT language models.",
     url="https://github.com/littleknitsstory/client-gpt",
     packages=setuptools.find_packages(),
     install_requires=[
         "requests",
     ],
```

