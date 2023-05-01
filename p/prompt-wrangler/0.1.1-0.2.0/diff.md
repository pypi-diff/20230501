# Comparing `tmp/prompt_wrangler-0.1.1.tar.gz` & `tmp/prompt_wrangler-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prompt_wrangler-0.1.1.tar", last modified: Mon May  1 14:25:51 2023, max compression
+gzip compressed data, was "prompt_wrangler-0.2.0.tar", last modified: Mon May  1 14:35:35 2023, max compression
```

## Comparing `prompt_wrangler-0.1.1.tar` & `prompt_wrangler-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 maxshaw    (501) staff       (20)        0 2023-05-01 14:25:51.728212 prompt_wrangler-0.1.1/
--rw-r--r--   0 maxshaw    (501) staff       (20)     1924 2023-05-01 14:25:51.728066 prompt_wrangler-0.1.1/PKG-INFO
--rw-r--r--   0 maxshaw    (501) staff       (20)     1218 2023-05-01 14:17:19.000000 prompt_wrangler-0.1.1/README.md
-drwxr-xr-x   0 maxshaw    (501) staff       (20)        0 2023-05-01 14:25:51.727151 prompt_wrangler-0.1.1/prompt_wrangler/
--rw-r--r--   0 maxshaw    (501) staff       (20)       69 2023-05-01 14:12:42.000000 prompt_wrangler-0.1.1/prompt_wrangler/__init__.py
--rw-r--r--   0 maxshaw    (501) staff       (20)     2366 2023-05-01 14:15:16.000000 prompt_wrangler-0.1.1/prompt_wrangler/client.py
-drwxr-xr-x   0 maxshaw    (501) staff       (20)        0 2023-05-01 14:25:51.727876 prompt_wrangler-0.1.1/prompt_wrangler.egg-info/
--rw-r--r--   0 maxshaw    (501) staff       (20)     1924 2023-05-01 14:25:51.000000 prompt_wrangler-0.1.1/prompt_wrangler.egg-info/PKG-INFO
--rw-r--r--   0 maxshaw    (501) staff       (20)      266 2023-05-01 14:25:51.000000 prompt_wrangler-0.1.1/prompt_wrangler.egg-info/SOURCES.txt
--rw-r--r--   0 maxshaw    (501) staff       (20)        1 2023-05-01 14:25:51.000000 prompt_wrangler-0.1.1/prompt_wrangler.egg-info/dependency_links.txt
--rw-r--r--   0 maxshaw    (501) staff       (20)        9 2023-05-01 14:25:51.000000 prompt_wrangler-0.1.1/prompt_wrangler.egg-info/requires.txt
--rw-r--r--   0 maxshaw    (501) staff       (20)       16 2023-05-01 14:25:51.000000 prompt_wrangler-0.1.1/prompt_wrangler.egg-info/top_level.txt
--rw-r--r--   0 maxshaw    (501) staff       (20)       38 2023-05-01 14:25:51.728272 prompt_wrangler-0.1.1/setup.cfg
--rw-r--r--   0 maxshaw    (501) staff       (20)      959 2023-05-01 14:25:51.000000 prompt_wrangler-0.1.1/setup.py
+drwxr-xr-x   0 maxshaw    (501) staff       (20)        0 2023-05-01 14:35:35.319954 prompt_wrangler-0.2.0/
+-rw-r--r--   0 maxshaw    (501) staff       (20)     1916 2023-05-01 14:35:35.319658 prompt_wrangler-0.2.0/PKG-INFO
+-rw-r--r--   0 maxshaw    (501) staff       (20)     1210 2023-05-01 14:33:51.000000 prompt_wrangler-0.2.0/README.md
+drwxr-xr-x   0 maxshaw    (501) staff       (20)        0 2023-05-01 14:35:35.318723 prompt_wrangler-0.2.0/prompt_wrangler/
+-rw-r--r--   0 maxshaw    (501) staff       (20)       69 2023-05-01 14:12:42.000000 prompt_wrangler-0.2.0/prompt_wrangler/__init__.py
+-rw-r--r--   0 maxshaw    (501) staff       (20)     2362 2023-05-01 14:33:18.000000 prompt_wrangler-0.2.0/prompt_wrangler/client.py
+drwxr-xr-x   0 maxshaw    (501) staff       (20)        0 2023-05-01 14:35:35.319454 prompt_wrangler-0.2.0/prompt_wrangler.egg-info/
+-rw-r--r--   0 maxshaw    (501) staff       (20)     1916 2023-05-01 14:35:35.000000 prompt_wrangler-0.2.0/prompt_wrangler.egg-info/PKG-INFO
+-rw-r--r--   0 maxshaw    (501) staff       (20)      266 2023-05-01 14:35:35.000000 prompt_wrangler-0.2.0/prompt_wrangler.egg-info/SOURCES.txt
+-rw-r--r--   0 maxshaw    (501) staff       (20)        1 2023-05-01 14:35:35.000000 prompt_wrangler-0.2.0/prompt_wrangler.egg-info/dependency_links.txt
+-rw-r--r--   0 maxshaw    (501) staff       (20)        9 2023-05-01 14:35:35.000000 prompt_wrangler-0.2.0/prompt_wrangler.egg-info/requires.txt
+-rw-r--r--   0 maxshaw    (501) staff       (20)       16 2023-05-01 14:35:35.000000 prompt_wrangler-0.2.0/prompt_wrangler.egg-info/top_level.txt
+-rw-r--r--   0 maxshaw    (501) staff       (20)       38 2023-05-01 14:35:35.320022 prompt_wrangler-0.2.0/setup.cfg
+-rw-r--r--   0 maxshaw    (501) staff       (20)     1060 2023-05-01 14:35:34.000000 prompt_wrangler-0.2.0/setup.py
```

### Comparing `prompt_wrangler-0.1.1/PKG-INFO` & `prompt_wrangler-0.2.0/prompt_wrangler.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: prompt_wrangler
-Version: 0.1.1
+Name: prompt-wrangler
+Version: 0.2.0
 Summary: A Python wrapper for the Prompt Wrangler REST API.
 Home-page: https://github.com/exit38/prompt_wrangler
 Author: Max Shaw
 Author-email: max@exit38.org
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -40,19 +40,19 @@
 api_key = "<your_api_key>"
 workspace = "<your_workspace_slug>"
 prompt_wrangler = PromptWrangler(api_key, workspace)
 ```
 
 Replace <your_api_key> with your actual API key.
 
-To add a new prompt, use the `add_prompt` method with the prompt slug:
+To add a new prompt, use the `prompt` method with the prompt slug:
 
 ```python
 prompt_slug = "reason-next-web-command"
-prompt = prompt_wrangler.add_prompt(prompt_slug)
+prompt = prompt_wrangler.prompt(prompt_slug)
 ```
 
 To run the prompt, use the `run` method, optionally passing a dictionary of arguments:
 
 ```python
 args = {'input_text': 'some input'}
 result = prompt.run(args=args)
```

### Comparing `prompt_wrangler-0.1.1/README.md` & `prompt_wrangler-0.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -20,19 +20,19 @@
 api_key = "<your_api_key>"
 workspace = "<your_workspace_slug>"
 prompt_wrangler = PromptWrangler(api_key, workspace)
 ```
 
 Replace <your_api_key> with your actual API key.
 
-To add a new prompt, use the `add_prompt` method with the prompt slug:
+To add a new prompt, use the `prompt` method with the prompt slug:
 
 ```python
 prompt_slug = "reason-next-web-command"
-prompt = prompt_wrangler.add_prompt(prompt_slug)
+prompt = prompt_wrangler.prompt(prompt_slug)
 ```
 
 To run the prompt, use the `run` method, optionally passing a dictionary of arguments:
 
 ```python
 args = {'input_text': 'some input'}
 result = prompt.run(args=args)
```

### Comparing `prompt_wrangler-0.1.1/prompt_wrangler/client.py` & `prompt_wrangler-0.2.0/prompt_wrangler/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         :param api_key: The API key for authentication.
         :param workspace: The workspace identifier.
         """
         self.api_key = api_key
         self.workspace = workspace
         self.base_url = "https://prompt-wrangler.com/api"
 
-    def add_prompt(self, prompt_slug: str) -> "PromptWranglerPrompt":
+    def prompt(self, prompt_slug: str) -> "PromptWranglerPrompt":
         """
         Add a prompt to the PromptWrangler client.
 
         :param prompt_slug: The prompt slug.
         :return: A PromptWranglerPrompt instance.
         """
         return PromptWranglerPrompt(self, prompt_slug)
```

### Comparing `prompt_wrangler-0.1.1/prompt_wrangler.egg-info/PKG-INFO` & `prompt_wrangler-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: prompt-wrangler
-Version: 0.1.1
+Name: prompt_wrangler
+Version: 0.2.0
 Summary: A Python wrapper for the Prompt Wrangler REST API.
 Home-page: https://github.com/exit38/prompt_wrangler
 Author: Max Shaw
 Author-email: max@exit38.org
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -40,19 +40,19 @@
 api_key = "<your_api_key>"
 workspace = "<your_workspace_slug>"
 prompt_wrangler = PromptWrangler(api_key, workspace)
 ```
 
 Replace <your_api_key> with your actual API key.
 
-To add a new prompt, use the `add_prompt` method with the prompt slug:
+To add a new prompt, use the `prompt` method with the prompt slug:
 
 ```python
 prompt_slug = "reason-next-web-command"
-prompt = prompt_wrangler.add_prompt(prompt_slug)
+prompt = prompt_wrangler.prompt(prompt_slug)
 ```
 
 To run the prompt, use the `run` method, optionally passing a dictionary of arguments:
 
 ```python
 args = {'input_text': 'some input'}
 result = prompt.run(args=args)
```

### Comparing `prompt_wrangler-0.1.1/setup.py` & `prompt_wrangler-0.2.0/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="prompt_wrangler",
-    version="0.1.1",
+    version="0.2.0",
     author="Max Shaw",
     author_email="max@exit38.org",
     description="A Python wrapper for the Prompt Wrangler REST API.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/exit38/prompt_wrangler",
     packages=find_packages(),
@@ -21,8 +21,10 @@
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
     ],
     python_requires=">=3.6",
     install_requires=["requests"],
+    package_data={"prompt_wrangler": ["prompt_wrangler/client.pyi"]},
+    include_package_data=True,
 )
```

