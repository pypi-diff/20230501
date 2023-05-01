# Comparing `tmp/revChatGPT-5.0.0.tar.gz` & `tmp/revChatGPT-5.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "revChatGPT-5.0.0.tar", last modified: Sun Apr 23 13:19:43 2023, max compression
+gzip compressed data, was "revChatGPT-5.0.1.tar", last modified: Mon May  1 08:35:05 2023, max compression
```

## Comparing `revChatGPT-5.0.0.tar` & `revChatGPT-5.0.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 13:19:43.738466 revChatGPT-5.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-04-23 13:19:07.000000 revChatGPT-5.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7905 2023-04-23 13:19:43.738466 revChatGPT-5.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6762 2023-04-23 13:19:43.000000 revChatGPT-5.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-23 13:19:43.738466 revChatGPT-5.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-04-23 13:19:07.000000 revChatGPT-5.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 13:19:43.734466 revChatGPT-5.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 13:19:43.738466 revChatGPT-5.0.0/src/revChatGPT/
--rw-r--r--   0 runner    (1001) docker     (123)    49256 2023-04-23 13:19:07.000000 revChatGPT-5.0.0/src/revChatGPT/V1.py
--rw-r--r--   0 runner    (1001) docker     (123)    23208 2023-04-23 13:19:07.000000 revChatGPT-5.0.0/src/revChatGPT/V3.py
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-04-23 13:19:07.000000 revChatGPT-5.0.0/src/revChatGPT/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-04-23 13:19:07.000000 revChatGPT-5.0.0/src/revChatGPT/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 13:19:43.738466 revChatGPT-5.0.0/src/revChatGPT/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-04-23 13:19:07.000000 revChatGPT-5.0.0/src/revChatGPT/config/enable_internet.json
--rw-r--r--   0 runner    (1001) docker     (123)     8584 2023-04-23 13:19:07.000000 revChatGPT-5.0.0/src/revChatGPT/recipient.py
--rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-04-23 13:19:07.000000 revChatGPT-5.0.0/src/revChatGPT/typings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-04-23 13:19:07.000000 revChatGPT-5.0.0/src/revChatGPT/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 13:19:43.738466 revChatGPT-5.0.0/src/revChatGPT.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7905 2023-04-23 13:19:43.000000 revChatGPT-5.0.0/src/revChatGPT.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-04-23 13:19:43.000000 revChatGPT-5.0.0/src/revChatGPT.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 13:19:43.000000 revChatGPT-5.0.0/src/revChatGPT.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-23 13:19:43.000000 revChatGPT-5.0.0/src/revChatGPT.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-23 13:19:43.000000 revChatGPT-5.0.0/src/revChatGPT.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 13:19:43.738466 revChatGPT-5.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-04-23 13:19:07.000000 revChatGPT-5.0.0/tests/test_recipient.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:35:05.526491 revChatGPT-5.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-05-01 08:34:36.000000 revChatGPT-5.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7849 2023-05-01 08:35:05.526491 revChatGPT-5.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6706 2023-05-01 08:35:05.000000 revChatGPT-5.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-01 08:35:05.530491 revChatGPT-5.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-05-01 08:34:36.000000 revChatGPT-5.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:35:05.526491 revChatGPT-5.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:35:05.526491 revChatGPT-5.0.1/src/revChatGPT/
+-rw-r--r--   0 runner    (1001) docker     (123)    49253 2023-05-01 08:34:36.000000 revChatGPT-5.0.1/src/revChatGPT/V1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23208 2023-05-01 08:34:36.000000 revChatGPT-5.0.1/src/revChatGPT/V3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-01 08:34:36.000000 revChatGPT-5.0.1/src/revChatGPT/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-05-01 08:34:36.000000 revChatGPT-5.0.1/src/revChatGPT/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:35:05.526491 revChatGPT-5.0.1/src/revChatGPT/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-05-01 08:34:36.000000 revChatGPT-5.0.1/src/revChatGPT/config/enable_internet.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8566 2023-05-01 08:34:36.000000 revChatGPT-5.0.1/src/revChatGPT/recipient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-05-01 08:34:36.000000 revChatGPT-5.0.1/src/revChatGPT/typings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-05-01 08:34:36.000000 revChatGPT-5.0.1/src/revChatGPT/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:35:05.526491 revChatGPT-5.0.1/src/revChatGPT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7849 2023-05-01 08:35:05.000000 revChatGPT-5.0.1/src/revChatGPT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-05-01 08:35:05.000000 revChatGPT-5.0.1/src/revChatGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 08:35:05.000000 revChatGPT-5.0.1/src/revChatGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-01 08:35:05.000000 revChatGPT-5.0.1/src/revChatGPT.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-01 08:35:05.000000 revChatGPT-5.0.1/src/revChatGPT.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:35:05.526491 revChatGPT-5.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-05-01 08:34:36.000000 revChatGPT-5.0.1/tests/test_recipient.py
```

### Comparing `revChatGPT-5.0.0/LICENSE` & `revChatGPT-5.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `revChatGPT-5.0.0/PKG-INFO` & `revChatGPT-5.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revChatGPT
-Version: 5.0.0
+Version: 5.0.1
 Summary: ChatGPT is a reverse engineering of OpenAI's ChatGPT API
 Home-page: https://github.com/acheong08/ChatGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+
 Project-URL: Feature request, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+
@@ -26,14 +26,16 @@
 
 [![PyPi](https://img.shields.io/pypi/v/revChatGPT.svg)](https://pypi.python.org/pypi/revChatGPT)
 [![Support_Platform](https://img.shields.io/pypi/pyversions/revChatGPT)](https://pypi.python.org/pypi/revChatGPT)
 [![Downloads](https://static.pepy.tech/badge/revchatgpt)](https://pypi.python.org/pypi/revChatGPT)
 
 Reverse Engineered ChatGPT API by OpenAI. Extensible for chatbots etc.
 
+Status: Working but unmaintained. 
+
 [![](https://github.com/acheong08/ChatGPT/blob/main/docs/view.gif?raw=true)](https://pypi.python.org/pypi/revChatGPT)
 
 > ## Support my work
 >
 > Make a pull request and fix my bad code.
 >
 > [![support](https://ko-fi.com/img/githubbutton_sm.svg)](https://www.youtube.com/watch?v=dQw4w9WgXcQ)
@@ -53,15 +55,15 @@
 
 <details>
 
   <summary>
 
 # V1 Standard ChatGPT
 
-Due to recent tightening of OpenAI's security, the default endpoint has been swapped over to one provided by @pengzhile. It is not open source and privacy is not guarenteed. Use it at your own risk. I am working on an open source implementation with the latest changes but that could take a while.
+Uses a proxy to get around cloudflare. It's open source: https://github.com/acheong08/ChatGPT-Proxy-V4. I currently host the default proxy. As always, no data collected other than by Cloudflare and OpenAI.
 
 </summary>
 
 ## Rate limits
 - Proxy server: 5 requests / 10 seconds
 - OpenAI: 50 requests / hour for each account
```

### Comparing `revChatGPT-5.0.0/README.md` & `revChatGPT-5.0.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 
 [![PyPi](https://img.shields.io/pypi/v/revChatGPT.svg)](https://pypi.python.org/pypi/revChatGPT)
 [![Support_Platform](https://img.shields.io/pypi/pyversions/revChatGPT)](https://pypi.python.org/pypi/revChatGPT)
 [![Downloads](https://static.pepy.tech/badge/revchatgpt)](https://pypi.python.org/pypi/revChatGPT)
 
 Reverse Engineered ChatGPT API by OpenAI. Extensible for chatbots etc.
 
+Status: Working but unmaintained. 
+
 [![](https://github.com/acheong08/ChatGPT/blob/main/docs/view.gif?raw=true)](https://pypi.python.org/pypi/revChatGPT)
 
 > ## Support my work
 >
 > Make a pull request and fix my bad code.
 >
 > [![support](https://ko-fi.com/img/githubbutton_sm.svg)](https://www.youtube.com/watch?v=dQw4w9WgXcQ)
@@ -31,15 +33,15 @@
 
 <details>
 
   <summary>
 
 # V1 Standard ChatGPT
 
-Due to recent tightening of OpenAI's security, the default endpoint has been swapped over to one provided by @pengzhile. It is not open source and privacy is not guarenteed. Use it at your own risk. I am working on an open source implementation with the latest changes but that could take a while.
+Uses a proxy to get around cloudflare. It's open source: https://github.com/acheong08/ChatGPT-Proxy-V4. I currently host the default proxy. As always, no data collected other than by Cloudflare and OpenAI.
 
 </summary>
 
 ## Rate limits
 - Proxy server: 5 requests / 10 seconds
 - OpenAI: 50 requests / hour for each account
```

### Comparing `revChatGPT-5.0.0/setup.py` & `revChatGPT-5.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 if not PATH.exists():
     with open(DOCS_PATH, encoding="utf-8") as f1:
         with open(PATH, "w+", encoding="utf-8") as f2:
             f2.write(f1.read())
 
 setup(
     name="revChatGPT",
-    version="5.0.0",
+    version="5.0.1",
     description="ChatGPT is a reverse engineering of OpenAI's ChatGPT API",
     long_description=open(PATH, encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/acheong08/ChatGPT",
     project_urls={
         "Bug Report": "https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+",
         "Feature request": "https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+",
```

### Comparing `revChatGPT-5.0.0/src/revChatGPT/V1.py` & `revChatGPT-5.0.1/src/revChatGPT/V1.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,15 +77,15 @@
             return out
 
         return wrapper
 
     return decorator
 
 
-BASE_URL = environ.get("CHATGPT_BASE_URL") or "https://ai.fakeopen.com/api/"
+BASE_URL = environ.get("CHATGPT_BASE_URL") or "https://bypass.churchless.tech/"
 
 bcolors = t.Colors()
 
 
 class Chatbot:
     """
     Chatbot class for ChatGPT
@@ -1348,15 +1348,15 @@
             print()
 
             msg = {}
             if not result.get("end_turn", True):
                 times += 1
                 if times >= 5:
                     continue
-                api = plugins.get(result["recipient"], None)
+                api = plugins.get(result["recipient"])
                 if not api:
                     msg = {
                         "id": str(uuid.uuid4()),
                         "author": {"role": "user"},
                         "content": {
                             "content_type": "text",
                             "parts": [f"Error: No plugin {result['recipient']} found"],
```

### Comparing `revChatGPT-5.0.0/src/revChatGPT/V3.py` & `revChatGPT-5.0.1/src/revChatGPT/V3.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-5.0.0/src/revChatGPT/__init__.py` & `revChatGPT-5.0.1/src/revChatGPT/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,28 +4,33 @@
 You can import the following module to use:
 revChatGPT.V1
 revChatGPT.V3
 """
 __version__ = "5.0.0"
 __all__ = ()
 
-# Available Python Version Verify
-from . import typings as t
 
-if int(__import__("platform").python_version_tuple()[0]) < 3:
-    error = t.NotAllowRunning("Not available Python version")
-    raise error
-elif int(__import__("platform").python_version_tuple()[1]) < 9:
-    error = t.NotAllowRunning(
-        f"Not available Python version: {__import__('platform').python_version()}",
-    )
-    raise error
-else:
-    if (
-        int(__import__("platform").python_version_tuple()[1]) < 10
-        and int(__import__("platform").python_version_tuple()[0]) == 3
-    ):
-        __import__("warnings").warn(
-            UserWarning(
-                "The current Python is not a recommended version, 3.10+ is recommended",
-            ),
+def verify() -> None:
+    # Available Python Version Verify
+    from . import typings as t
+
+    if int(__import__("platform").python_version_tuple()[0]) < 3:
+        error = t.NotAllowRunning("Not available Python version")
+        raise error
+    elif int(__import__("platform").python_version_tuple()[1]) < 9:
+        error = t.NotAllowRunning(
+            f"Not available Python version: {__import__('platform').python_version()}",
         )
+        raise error
+    else:
+        if (
+            int(__import__("platform").python_version_tuple()[1]) < 10
+            and int(__import__("platform").python_version_tuple()[0]) == 3
+        ):
+            __import__("warnings").warn(
+                UserWarning(
+                    "The current Python is not a recommended version, 3.10+ is recommended",
+                ),
+            )
+
+
+verify()
```

### Comparing `revChatGPT-5.0.0/src/revChatGPT/__main__.py` & `revChatGPT-5.0.1/src/revChatGPT/__main__.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-5.0.0/src/revChatGPT/config/enable_internet.json` & `revChatGPT-5.0.1/src/revChatGPT/config/enable_internet.json`

 * *Files identical despite different names*

### Comparing `revChatGPT-5.0.0/src/revChatGPT/recipient.py` & `revChatGPT-5.0.1/src/revChatGPT/recipient.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,19 +31,18 @@
 
 
 class RecipientMeta(ABCMeta):
     """
     Metaclass for the Recipient class.
     """
 
-    def __new__(mcs, name, bases, namespace, /, **kwargs):
-        if not "RECIPIENT_NAME" in namespace or not namespace["RECIPIENT_NAME"]:
+    def __new__(cls, name, bases, namespace, /, **kwargs):
+        if "RECIPIENT_NAME" not in namespace or not namespace["RECIPIENT_NAME"]:
             namespace["RECIPIENT_NAME"] = name
-        cls = super().__new__(mcs, name, bases, namespace, **kwargs)
-        return cls
+        return super().__new__(cls, name, bases, namespace, **kwargs)
 
 
 class Recipient(metaclass=RecipientMeta):
     """
     Recipient base class.
 
     Attributes
```

### Comparing `revChatGPT-5.0.0/src/revChatGPT/typings.py` & `revChatGPT-5.0.1/src/revChatGPT/typings.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-5.0.0/src/revChatGPT/utils.py` & `revChatGPT-5.0.1/src/revChatGPT/utils.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-5.0.0/src/revChatGPT.egg-info/PKG-INFO` & `revChatGPT-5.0.1/src/revChatGPT.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revChatGPT
-Version: 5.0.0
+Version: 5.0.1
 Summary: ChatGPT is a reverse engineering of OpenAI's ChatGPT API
 Home-page: https://github.com/acheong08/ChatGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+
 Project-URL: Feature request, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+
@@ -26,14 +26,16 @@
 
 [![PyPi](https://img.shields.io/pypi/v/revChatGPT.svg)](https://pypi.python.org/pypi/revChatGPT)
 [![Support_Platform](https://img.shields.io/pypi/pyversions/revChatGPT)](https://pypi.python.org/pypi/revChatGPT)
 [![Downloads](https://static.pepy.tech/badge/revchatgpt)](https://pypi.python.org/pypi/revChatGPT)
 
 Reverse Engineered ChatGPT API by OpenAI. Extensible for chatbots etc.
 
+Status: Working but unmaintained. 
+
 [![](https://github.com/acheong08/ChatGPT/blob/main/docs/view.gif?raw=true)](https://pypi.python.org/pypi/revChatGPT)
 
 > ## Support my work
 >
 > Make a pull request and fix my bad code.
 >
 > [![support](https://ko-fi.com/img/githubbutton_sm.svg)](https://www.youtube.com/watch?v=dQw4w9WgXcQ)
@@ -53,15 +55,15 @@
 
 <details>
 
   <summary>
 
 # V1 Standard ChatGPT
 
-Due to recent tightening of OpenAI's security, the default endpoint has been swapped over to one provided by @pengzhile. It is not open source and privacy is not guarenteed. Use it at your own risk. I am working on an open source implementation with the latest changes but that could take a while.
+Uses a proxy to get around cloudflare. It's open source: https://github.com/acheong08/ChatGPT-Proxy-V4. I currently host the default proxy. As always, no data collected other than by Cloudflare and OpenAI.
 
 </summary>
 
 ## Rate limits
 - Proxy server: 5 requests / 10 seconds
 - OpenAI: 50 requests / hour for each account
```

### Comparing `revChatGPT-5.0.0/tests/test_recipient.py` & `revChatGPT-5.0.1/tests/test_recipient.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,39 +2,39 @@
 import datetime
 
 import revChatGPT.V1
 from revChatGPT.recipient import PythonRecipient
 from revChatGPT.V1 import Chatbot
 
 
-def test_recipient():
+def test_recipient() -> None:
     """
     Test the chatbot
     """
     config = revChatGPT.V1.configure()
     assert "access_token" in config
     cbt = Chatbot(config)
     assert cbt is not None
 
     # Try to get the recipient which is not registered
     try:
         _ = cbt.recipients["python"]
-        assert False
+        raise AssertionError
     except Exception as ex:
         assert isinstance(ex, KeyError)
         assert ex.args[0] == "Recipient 'python' is not registered."
 
     # Register the recipient
     cbt.recipients["python"] = PythonRecipient
     assert cbt.recipients["python"].DESCRIPTION == "Python Interpreter Remote"
 
     # Try to register the recipient which is already registered
     try:
         cbt.recipients["python"] = PythonRecipient
-        assert False
+        raise AssertionError
     except Exception as ex:
         assert isinstance(ex, KeyError)
         assert ex.args[0] == "Recipient 'python' is already registered."
 
     # To get the recipient instance
     python = cbt.recipients["python"]()
 
@@ -44,15 +44,15 @@
     Current date: {datetime.datetime.now().strftime("%Y-%m-%d")}
 
     ###Available Tools:
     python
 
     {python.API_DOCS}
     """
-    for _ in cbt.ask("You are ChatGPT." + api_docs):
+    for _ in cbt.ask(f"You are ChatGPT.{api_docs}"):
         pass
 
     # Test the python recipient
     result = {}
     for _ in cbt.ask("Please calculate 27! + 8! by using python."):
         result = _
     assert result
```

