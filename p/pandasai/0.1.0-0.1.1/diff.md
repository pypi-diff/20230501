# Comparing `tmp/pandasai-0.1.0.tar.gz` & `tmp/pandasai-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandasai-0.1.0.tar", max compression
+gzip compressed data, was "pandasai-0.1.1.tar", max compression
```

## Comparing `pandasai-0.1.0.tar` & `pandasai-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0     1055 2023-04-24 05:55:05.323190 pandasai-0.1.0/LICENSE
--rw-r--r--   0        0        0     2923 2023-04-29 12:25:55.311311 pandasai-0.1.0/README.md
--rw-r--r--   0        0        0     3326 2023-04-29 12:22:08.974103 pandasai-0.1.0/pandasai/__init__.py
--rw-r--r--   0        0        0        0 2023-04-24 11:19:15.318272 pandasai-0.1.0/pandasai/llm/__init__.py
--rw-r--r--   0        0        0     1065 2023-04-24 13:43:47.784698 pandasai-0.1.0/pandasai/llm/alpaca.py
--rw-r--r--   0        0        0     1938 2023-04-29 12:22:08.974865 pandasai-0.1.0/pandasai/llm/base.py
--rw-r--r--   0        0        0      324 2023-04-29 12:22:08.975266 pandasai-0.1.0/pandasai/llm/fake.py
--rw-r--r--   0        0        0      965 2023-04-29 12:22:08.975718 pandasai-0.1.0/pandasai/llm/open_assistant.py
--rw-r--r--   0        0        0     2908 2023-04-29 12:22:08.976312 pandasai-0.1.0/pandasai/llm/openai.py
--rw-r--r--   0        0        0      579 2023-04-29 13:04:33.234577 pandasai-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3607 1970-01-01 00:00:00.000000 pandasai-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1055 2023-04-24 05:55:05.323190 pandasai-0.1.1/LICENSE
+-rw-r--r--   0        0        0     4082 2023-05-01 00:23:57.698037 pandasai-0.1.1/README.md
+-rw-r--r--   0        0        0     4132 2023-04-30 23:39:11.591122 pandasai-0.1.1/pandasai/__init__.py
+-rw-r--r--   0        0        0      512 2023-04-30 10:30:15.012968 pandasai-0.1.1/pandasai/exceptions.py
+-rw-r--r--   0        0        0        0 2023-04-30 09:49:31.456755 pandasai-0.1.1/pandasai/llm/__init__.py
+-rw-r--r--   0        0        0     1466 2023-04-30 23:41:22.772250 pandasai-0.1.1/pandasai/llm/alpaca.py
+-rw-r--r--   0        0        0     2196 2023-04-30 23:43:44.275375 pandasai-0.1.1/pandasai/llm/base.py
+-rw-r--r--   0        0        0      439 2023-04-30 23:42:14.083716 pandasai-0.1.1/pandasai/llm/fake.py
+-rw-r--r--   0        0        0     1167 2023-04-30 10:29:36.204761 pandasai-0.1.1/pandasai/llm/open_assistant.py
+-rw-r--r--   0        0        0     3296 2023-04-30 23:41:08.717617 pandasai-0.1.1/pandasai/llm/openai.py
+-rw-r--r--   0        0        0      635 2023-05-01 00:24:04.023587 pandasai-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4807 1970-01-01 00:00:00.000000 pandasai-0.1.1/PKG-INFO
```

### Comparing `pandasai-0.1.0/LICENSE` & `pandasai-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pandasai-0.1.0/pandasai/__init__.py` & `pandasai-0.1.1/pandasai/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,82 +1,107 @@
-import pandas as pd
-from .llm.base import LLM
+""" PandasAI is a wrapper around a LLM to make dataframes convesational """
 import io
 import sys
+import pandas as pd
+from .llm.base import LLM
+from .exceptions import LLMNotFoundError
 
 
 class PandasAI:
     """PandasAI is a wrapper around a LLM to make dataframes convesational"""
 
     _task_instruction: str = """
 There is a dataframe in pandas (python).
 The name of the dataframe is `df`.
-This is the result of `print(df.head())`:
+This is the result of `print(df.head({rows_to_display}))`:
 {df_head}.
 
 Return the python code (do not import anything) to get the answer to the following question:
 """
     _response_instruction: str = """
 Question: {question}
 Answer: {answer}
 
 Rewrite the answer to the question in a conversational way.
 """
     _llm: LLM
     _verbose: bool = False
     _is_conversational_answer: bool = True
+    _enforce_privacy: bool = False
     last_code_generated: str = None
     code_output: str = None
 
-    def __init__(self, llm=None, conversational=True, verbose=False):
+    def __init__(
+        self, llm=None, conversational=True, verbose=False, enforce_privacy=False
+    ):
         if llm is None:
-            raise Exception(
+            raise LLMNotFoundError(
                 "An LLM should be provided to instantiate a PandasAI instance"
             )
         self._llm = llm
         self._is_conversational_answer = conversational
         self._verbose = verbose
+        self._enforce_privacy = enforce_privacy
 
     def conversational_answer(self, question: str, code: str, answer: str) -> str:
         """Return the conversational answer"""
+        if self._enforce_privacy:
+            # we don't want to send potentially sensitive data to the LLM server
+            # if the user has set enforce_privacy to True
+            return answer
+
         instruction = self._response_instruction.format(
             question=question, code=code, answer=answer
         )
         return self._llm.call(instruction, answer)
 
     def run(
-        self, df: pd.DataFrame, prompt: str, is_conversational_answer: bool = None
+        self,
+        data_frame: pd.DataFrame,
+        prompt: str,
+        is_conversational_answer: bool = None,
     ) -> str:
         """Run the LLM with the given prompt"""
-        self.log(f"Running PandasAI with {self._llm._type} LLM...")
+        self.log(f"Running PandasAI with {self._llm.type} LLM...")
+
+        rows_to_display = 5
+        if self._enforce_privacy:
+            rows_to_display = 0
 
         code = self._llm.generate_code(
-            self._task_instruction.format(df_head=df.head()), prompt
+            self._task_instruction.format(
+                df_head=data_frame.head(rows_to_display),
+                rows_to_display=rows_to_display,
+            ),
+            prompt,
         )
         self.last_code_generated = code
         self.log(
             f"""
 Code generated:
 ```
 {code}
 ```"""
         )
 
-        answer = self.run_code(code, df)
+        answer = self.run_code(code, data_frame)
         self.code_output = answer
         self.log(f"Answer: {answer}")
 
         if is_conversational_answer is None:
             is_conversational_answer = self._is_conversational_answer
         if is_conversational_answer:
             answer = self.conversational_answer(prompt, code, answer)
             self.log(f"Conversational answer: {answer}")
         return answer
 
-    def run_code(self, code: str, df: pd.DataFrame):
+    def run_code(
+        self, code: str, df: pd.DataFrame  # pylint: disable=W0613 disable=C0103
+    ) -> str:
+        # pylint: disable=W0122 disable=W0123 disable=W0702:bare-except
         """Run the code in the current context and return the result"""
 
         # Redirect standard output to a StringIO buffer
         output = io.StringIO()
         sys.stdout = output
 
         # Execute the code
@@ -88,19 +113,18 @@
 
         # Evaluate the last line and return its value or the captured output
         lines = code.strip().split("\n")
         last_line = lines[-1].strip()
         if last_line.startswith("print(") and last_line.endswith(")"):
             # Last line is already printing
             return eval(last_line[6:-1])
-        else:
-            # Evaluate last line and return its value or the captured output
-            try:
-                result = eval(last_line)
-                return result
-            except:
-                return captured_output
+        # Evaluate last line and return its value or the captured output
+        try:
+            result = eval(last_line)
+            return result
+        except:
+            return captured_output
 
     def log(self, message: str):
         """Log a message"""
         if self._verbose:
             print(message)
```

### Comparing `pandasai-0.1.0/pandasai/llm/base.py` & `pandasai-0.1.1/pandasai/llm/base.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,28 @@
+""" Base class to implement a new LLM. """
+
 import re
 import ast
 import astor
+from ..exceptions import (
+    APIKeyNotFoundError,
+    NoCodeFoundError,
+    MethodNotImplementedError,
+)
 
 
 class LLM:
+    """Base class to implement a new LLM."""
+
+    last_prompt: str = None
+
     @property
-    def _type(self) -> str:
+    def type(self) -> str:
         """Return type of llm."""
-        raise Exception("Type has not been implemented")
+        raise APIKeyNotFoundError("Type has not been implemented")
 
     def _remove_imports(self, code: str) -> str:
         tree = ast.parse(code)
         new_body = []
 
         for node in tree.body:
             if not isinstance(node, (ast.Import, ast.ImportFrom)):
@@ -46,20 +57,20 @@
         """Extract the code from the response"""
 
         code = response
         if len(response.split(separator)) > 1:
             code = response.split(separator)[1]
         code = self._polish_code(code)
         if not self._is_python_code(code):
-            raise Exception("No code found in the response")
+            raise NoCodeFoundError("No code found in the response")
 
         return code
 
-    def call(self, instruction: str, input: str) -> str:
+    def call(self, instruction: str, value: str) -> str:
         """Execute the llm with the given prompt"""
 
-        raise Exception("Call method has not been implemented")
+        raise MethodNotImplementedError("Call method has not been implemented")
 
     def generate_code(self, instruction: str, prompt: str) -> str:
         """Generate the code based on the instruction and the prompt"""
 
         return self._extract_code(self.call(instruction, prompt))
```

### Comparing `pandasai-0.1.0/pandasai/llm/open_assistant.py` & `pandasai-0.1.1/pandasai/llm/open_assistant.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,44 @@
-import requests
+""" Open Assistant LLM """
+
 import os
+import requests
 from dotenv import load_dotenv
 from .base import LLM
+from ..exceptions import APIKeyNotFoundError
 
 load_dotenv()
 
 
 class OpenAssistant(LLM):
+    """Open Assistant LLM"""
+
     api_token: str
+    _api_url: str = (
+        "https://api-inference.huggingface.co/models/"
+        "OpenAssistant/oasst-sft-1-pythia-12b"
+    )
 
     def __init__(self, api_token: str = None):
         self.api_token = api_token or os.getenv("HUGGINGFACE_API_KEY")
         if self.api_token is None:
-            raise Exception("HuggingFace Hub API key is required")
+            raise APIKeyNotFoundError("HuggingFace Hub API key is required")
 
     def query(self, payload):
-        API_URL = "https://api-inference.huggingface.co/models/OpenAssistant/oasst-sft-1-pythia-12b"
-        headers = {"Authorization": "Bearer {}".format(self.api_token)}
+        """Query the API"""
+
+        headers = {"Authorization": f"Bearer {self.api_token}"}
 
-        response = requests.post(API_URL, headers=headers, json=payload)
+        response = requests.post(
+            self._api_url, headers=headers, json=payload, timeout=60
+        )
         return response.json()
 
-    def call(self, instruction: str, input: str) -> str:
+    def call(self, instruction: str, value: str) -> str:
         output = self.query(
-            {"inputs": "<|prompter|>" + instruction + input + "<|endoftext|>"}
+            {"inputs": "<|prompter|>" + instruction + value + "<|endoftext|>"}
         )
         return output[0]["generated_text"]
 
     @property
-    def _type(self) -> str:
+    def type(self) -> str:
         return "open-assistant"
```

### Comparing `pandasai-0.1.0/pyproject.toml` & `pandasai-0.1.1/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 [tool.poetry]
 name = "pandasai"
-version = "0.1.0"
+version = "0.1.1"
 description = "Pandas AI is a Python library that integrates generative artificial intelligence capabilities into Pandas, making dataframes conversational."
 authors = ["Gabriele Venturi"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "pandasai"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 python-dotenv = "^1.0.0"
 pandas = "^2.0.1"
 astor = "^0.8.1"
+openai = "^0.27.5"
 
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 pre-commit = "^3.2.2"
+pylint = "^2.17.3"
+pytest = "^7.3.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

