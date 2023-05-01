# Comparing `tmp/client_GPT-1.1.6.tar.gz` & `tmp/client_GPT-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "client_GPT-1.1.6.tar", last modified: Mon May  1 16:53:09 2023, max compression
+gzip compressed data, was "client_GPT-1.1.7.tar", last modified: Mon May  1 16:58:02 2023, max compression
```

## Comparing `client_GPT-1.1.6.tar` & `client_GPT-1.1.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 16:53:09.293933 client_GPT-1.1.6/
--rw-rw-rw-   0        0        0      419 2023-05-01 16:53:09.292920 client_GPT-1.1.6/PKG-INFO
--rw-rw-rw-   0        0        0      425 2023-04-27 14:12:47.000000 client_GPT-1.1.6/README.md
-drwxrwxrwx   0        0        0        0 2023-05-01 16:53:09.281921 client_GPT-1.1.6/client_GPT.egg-info/
--rw-rw-rw-   0        0        0      419 2023-05-01 16:53:09.000000 client_GPT-1.1.6/client_GPT.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      235 2023-05-01 16:53:09.000000 client_GPT-1.1.6/client_GPT.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 16:53:09.000000 client_GPT-1.1.6/client_GPT.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-01 16:53:09.000000 client_GPT-1.1.6/client_GPT.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-01 16:53:09.000000 client_GPT-1.1.6/client_GPT.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-01 16:53:09.291920 client_GPT-1.1.6/client_gpt/
--rw-rw-rw-   0        0        0        0 2023-04-27 13:20:09.000000 client_GPT-1.1.6/client_gpt/__init__.py
--rw-rw-rw-   0        0        0     3920 2023-05-01 16:52:47.000000 client_GPT-1.1.6/client_gpt/client_gpt.py
--rw-rw-rw-   0        0        0       42 2023-05-01 16:53:09.294922 client_GPT-1.1.6/setup.cfg
--rw-rw-rw-   0        0        0      591 2023-05-01 16:53:01.000000 client_GPT-1.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 16:58:02.515378 client_GPT-1.1.7/
+-rw-rw-rw-   0        0        0      419 2023-05-01 16:58:02.514380 client_GPT-1.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0      425 2023-04-27 14:12:47.000000 client_GPT-1.1.7/README.md
+drwxrwxrwx   0        0        0        0 2023-05-01 16:58:02.500381 client_GPT-1.1.7/client_GPT.egg-info/
+-rw-rw-rw-   0        0        0      419 2023-05-01 16:58:02.000000 client_GPT-1.1.7/client_GPT.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      235 2023-05-01 16:58:02.000000 client_GPT-1.1.7/client_GPT.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 16:58:02.000000 client_GPT-1.1.7/client_GPT.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-01 16:58:02.000000 client_GPT-1.1.7/client_GPT.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-01 16:58:02.000000 client_GPT-1.1.7/client_GPT.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-01 16:58:02.513379 client_GPT-1.1.7/client_gpt/
+-rw-rw-rw-   0        0        0        0 2023-04-27 13:20:09.000000 client_GPT-1.1.7/client_gpt/__init__.py
+-rw-rw-rw-   0        0        0     4087 2023-05-01 16:57:46.000000 client_GPT-1.1.7/client_gpt/client_gpt.py
+-rw-rw-rw-   0        0        0       42 2023-05-01 16:58:02.516380 client_GPT-1.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      591 2023-05-01 16:57:55.000000 client_GPT-1.1.7/setup.py
```

### Comparing `client_GPT-1.1.6/client_gpt/client_gpt.py` & `client_GPT-1.1.7/client_gpt/client_gpt.py`

 * *Files 5% similar despite different names*

```diff
@@ -61,16 +61,19 @@
             response = self.session.post(
                 self.chat_api_url,
                 headers=headers,
                 data=json.dumps(data),
             )
             if response.status_code == 200:
                 response_text = response.text.replace("data: [DONE]", "")
-                data = re.findall(r"data: (.*)", response_text)
+                data = re.findall(r"data: (.*)", response_text)[-1]
                 as_json = json.loads(data)
+                print(as_json["message"]["content"]["parts"][0],
+                    as_json["message"]["id"],
+                    as_json["conversation_id"],)
                 return (
                     as_json["message"]["content"]["parts"][0],
                     as_json["message"]["id"],
                     as_json["conversation_id"],
                 )
             elif response.status_code == 401:
                 if os.path.exists("auth.json"):
```

### Comparing `client_GPT-1.1.6/setup.py` & `client_GPT-1.1.7/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="client_GPT",
-    version="1.1.6",
+    version="1.1.7",
     author="littleknitsstory",
     description="A package for working with GPT language models.",
     url="https://github.com/littleknitsstory/client-gpt",
     packages=setuptools.find_packages(),
     install_requires=[
         "requests",
     ],
```

