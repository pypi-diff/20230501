# Comparing `tmp/airoboros-0.0.1-py3-none-any.whl.zip` & `tmp/airoboros-0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 13486 bytes, number of entries: 10
+Zip file size: 13549 bytes, number of entries: 10
 -rw-r--r--  2.0 unx        0 b- defN 23-May-01 08:36 airoboros/__init__.py
 -rw-r--r--  2.0 unx      466 b- defN 23-May-01 09:54 airoboros/entrypoint.py
--rw-r--r--  2.0 unx      297 b- defN 23-May-01 08:36 airoboros/exceptions.py
--rw-r--r--  2.0 unx    25388 b- defN 23-May-01 09:45 airoboros/self_instruct.py
--rw-r--r--  2.0 unx    11357 b- defN 23-May-01 10:10 airoboros-0.0.1.dist-info/LICENSE
--rw-r--r--  2.0 unx      763 b- defN 23-May-01 10:10 airoboros-0.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-01 10:10 airoboros-0.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       55 b- defN 23-May-01 10:10 airoboros-0.0.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       10 b- defN 23-May-01 10:10 airoboros-0.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      810 b- defN 23-May-01 10:10 airoboros-0.0.1.dist-info/RECORD
-10 files, 39238 bytes uncompressed, 12096 bytes compressed:  69.2%
+-rw-r--r--  2.0 unx      338 b- defN 23-May-01 19:03 airoboros/exceptions.py
+-rw-r--r--  2.0 unx    25713 b- defN 23-May-01 19:24 airoboros/self_instruct.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-May-01 19:25 airoboros-0.0.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx      763 b- defN 23-May-01 19:25 airoboros-0.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-01 19:25 airoboros-0.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       55 b- defN 23-May-01 19:25 airoboros-0.0.2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       10 b- defN 23-May-01 19:25 airoboros-0.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      810 b- defN 23-May-01 19:25 airoboros-0.0.2.dist-info/RECORD
+10 files, 39604 bytes uncompressed, 12159 bytes compressed:  69.3%
```

## zipnote {}

```diff
@@ -6,26 +6,26 @@
 
 Filename: airoboros/exceptions.py
 Comment: 
 
 Filename: airoboros/self_instruct.py
 Comment: 
 
-Filename: airoboros-0.0.1.dist-info/LICENSE
+Filename: airoboros-0.0.2.dist-info/LICENSE
 Comment: 
 
-Filename: airoboros-0.0.1.dist-info/METADATA
+Filename: airoboros-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: airoboros-0.0.1.dist-info/WHEEL
+Filename: airoboros-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: airoboros-0.0.1.dist-info/entry_points.txt
+Filename: airoboros-0.0.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: airoboros-0.0.1.dist-info/top_level.txt
+Filename: airoboros-0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: airoboros-0.0.1.dist-info/RECORD
+Filename: airoboros-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## airoboros/exceptions.py

```diff
@@ -6,7 +6,9 @@
     ...
 class TokensExhaustedError(RuntimeError):
     ...
 class ContextLengthExceededError(RuntimeError):
     ...
 class ServerOverloadedError(RuntimeError):
     ...
+class ServerError(RuntimeError):
+    ...
```

## airoboros/self_instruct.py

```diff
@@ -16,33 +16,34 @@
 from typing import List, Dict, Any
 from rouge_score import rouge_scorer
 from .exceptions import (
     RateLimitError,
     TooManyRequestsError,
     TokensExhaustedError,
     ServerOverloadedError,
+    ServerError,
     ContextLengthExceededError,
     BadResponseError,
 )
 
 # Defaults and constants.
 BATCH_SIZE = 13
 DEFAULT_PROMPT = f"""You are asked to generate a set of {BATCH_SIZE} diverse prompts.  These prompts will be given to a GPT model and we will evaluate the GPT model for completing the prompts.
 
 Here are the requirements:
  * Try not to repeat the verb for each __instruction__ to maximize diversity.
- * Try to avoid constroversial and politically charged subjects.
- * The __instruction__ should include a variety of types of prompts, such as open-ended generation, brainstorming, classification, closed question-answering, summarization, editing, information extraction, etc.k
+ * Try to avoid controversial and politically charged subjects.
+ * The __instruction__ should include a variety of types of prompts, such as open-ended generation, brainstorming, classification, closed question-answering, summarization, editing, information extraction, etc.
  * The __instruction__ should be something a large language model can complete with a text response, for example do not create a task asking to create visual/audio output, setting an alarm, scheduling something on the calendar, etc. because the language model cannot perform those tasks.
  * The __instruction__ should be in English.
  * The __instruction__ should be between 1 and 3 sentences long.
  * For prompts that require extracting information from __passage__, e.g. question-answering, summarization, information extraction, etc., include a passage of text with 2-8 sentences in __passage__ providing all relevant data, including more information than necessary to generate __response__. __passage__ must not be simple placeholders or links to external resources.  Be sure to include all words, phrases, dates, or lists of items in __passage__ if those are part of __response__.
  * Not all prompts require __passage__. For example, when a task asks about some general information, e.g. "what is the highest peak in the world?", it is not necssary to provide a specific __passage__. In this case, we simply put "__no_context__" in the __passage__ field.
  * The __response__ should be an appropriate response to the __instruction__ and __passage__
- * Be sure to include {BATCH_SIZE} propts in the response.
+ * Be sure to include {BATCH_SIZE} prompts in the response.
 REPLACE_TOPICS
 
 List of {BATCH_SIZE} prompts:
 """
 SKIP_WORDS = ["image", "graph", "picture", "file", "map", "draw", "plot", "go to"]
 SKIP_SEARCH_RE = re.compile(r"\b{'|'.join(SKIP_WORDS)}s?\b", re.I)
 CODE_GEN_RE = re.compile(
@@ -478,15 +479,22 @@
             )
             logger.info(
                 f"Generated new task [has context: {context != ''}]: {instruction_text}"
             )
         return tasks
 
     @backoff.on_exception(
-        backoff.expo, (RateLimitError, TooManyRequestsError, ServerOverloadedError)
+        backoff.expo,
+        (
+            asyncio.TimeoutError,
+            ServerError,
+            RateLimitError,
+            TooManyRequestsError,
+            ServerOverloadedError,
+        ),
     )
     async def _post(self, path: str, payload: Dict[str, Any]) -> Dict[str, Any]:
         """Perform a post request to OpenAI API.
 
         :param path: URL path to send request to.
         :type path: str
 
@@ -497,26 +505,31 @@
         :rtype: Dict[str, Any]
         """
         headers = {"Authorization": f"Bearer {self.openai_api_key}"}
         if self.organization_id:
             headers["OpenAI-Organization"] = self.organization_id
         async with aiohttp.ClientSession() as session:
             result = await session.post(
-                f"{OPENAI_API_BASE_URL}{path}", headers=headers, json=payload
+                f"{OPENAI_API_BASE_URL}{path}",
+                headers=headers,
+                json=payload,
+                timeout=120.0,
             )
             if result.status != 200:
                 text = await result.text()
                 if "too many requests" in text.lower():
                     raise TooManyRequestsError(text)
                 if "rate limit reached" in text.lower():
                     raise RateLimitError(text)
                 elif "context_length_exceeded" in text.lower():
                     raise ContextLengthExceededError(text)
                 elif "server_error" in text and "overloaded" in text.lower():
                     raise ServerOverloadedError(text)
+                elif "bad gateway" in text.lower() or "server_error" in text.lower():
+                    raise ServerError(text)
                 else:
                     raise BadResponseError(text)
             result = await result.json()
         logger.debug(f"POST {path} with {json.dumps(payload)}: {json.dumps(result)}")
         self.used_tokens += result["usage"]["total_tokens"]
         if self.max_usage_tokens and self.used_tokens > self.max_usage_tokens:
             raise TokensExhaustedError(f"Max token usage exceeded: {self.used_tokens}")
```

## Comparing `airoboros-0.0.1.dist-info/LICENSE` & `airoboros-0.0.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `airoboros-0.0.1.dist-info/METADATA` & `airoboros-0.0.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airoboros
-Version: 0.0.1
+Version: 0.0.2
 Summary: Re-implementation of the self-instruct paper, with updated prompts, models, etc.
 Home-page: https://github.com/jondurbin/airoboros
 Author: Jon Durbin
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

