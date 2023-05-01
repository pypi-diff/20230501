# Comparing `tmp/gpyt-0.1.0.tar.gz` & `tmp/gpyt-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpyt-0.1.0.tar", max compression
+gzip compressed data, was "gpyt-0.1.1.tar", max compression
```

## Comparing `gpyt-0.1.0.tar` & `gpyt-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0      259 2023-05-01 19:31:37.007304 gpyt-0.1.0/README.md
--rw-r--r--   0        0        0      405 2023-05-01 19:31:19.867304 gpyt-0.1.0/gpyt/__init__.py
--rw-r--r--   0        0        0      920 2023-05-01 19:31:28.087304 gpyt-0.1.0/gpyt/app.py
--rw-r--r--   0        0        0      877 2023-05-01 19:31:20.167304 gpyt-0.1.0/gpyt/assistant.py
--rw-r--r--   0        0        0      332 2023-05-01 19:30:42.187304 gpyt-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      653 1970-01-01 00:00:00.000000 gpyt-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      427 2023-05-01 19:44:40.857304 gpyt-0.1.1/README.md
+-rw-r--r--   0        0        0      974 2023-05-01 19:43:03.287304 gpyt-0.1.1/gpyt/__init__.py
+-rw-r--r--   0        0        0       30 2023-05-01 19:44:00.177304 gpyt-0.1.1/gpyt/__main__.py
+-rw-r--r--   0        0        0      636 2023-05-01 19:40:49.577304 gpyt-0.1.1/gpyt/app.py
+-rw-r--r--   0        0        0      844 2023-05-01 19:37:57.027304 gpyt-0.1.1/gpyt/assistant.py
+-rw-r--r--   0        0        0      332 2023-05-01 19:46:33.867304 gpyt-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      821 1970-01-01 00:00:00.000000 gpyt-0.1.1/PKG-INFO
```

### Comparing `gpyt-0.1.0/gpyt/assistant.py` & `gpyt-0.1.1/gpyt/assistant.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 
 class Assistant:
     def __init__(self, *, api_key: str, model: str, prompt: str, memory: bool = True):
         self.api_key = api_key
         self.model = model
         self.prompt = prompt
         self.memory = memory
-        print(f"{self.memory=}")
         self.messages = [
             {"role": "system", "content": self.prompt},
         ]
 
     def clear_history(self):
         self.messages = [self.messages[0]]
```

### Comparing `gpyt-0.1.0/PKG-INFO` & `gpyt-0.1.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 Metadata-Version: 2.1
 Name: gpyt
-Version: 0.1.0
+Version: 0.1.1
 Summary: GPT on the command line.
 Author: Justin Stitt
 Author-email: jstitt007@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: openai (>=0.27.5,<0.28.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Description-Content-Type: text/markdown
 
-# GPTCLI
+# gpyt
 
 Interact with GPT on the command line.
 
 
 
 ### Desired Features
 * `copy` to copy GPT's response to clipboard
 * color coded responses
 * add gpt jailbreaks
 * `new` to start a new chat (clear all history and console window)
 * store chat logs somewhere.
+* add special flags like -t (terse) or -v (verbose) or -d (detailed) or -i (informal) or -f (for file input)
+* scrolling text (adjustable speed, or disable all together)
```

