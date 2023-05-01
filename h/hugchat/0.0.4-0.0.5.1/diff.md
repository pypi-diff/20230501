# Comparing `tmp/hugchat-0.0.4.tar.gz` & `tmp/hugchat-0.0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hugchat-0.0.4.tar", last modified: Mon May  1 00:48:05 2023, max compression
+gzip compressed data, was "hugchat-0.0.5.1.tar", last modified: Mon May  1 18:00:57 2023, max compression
```

## Comparing `hugchat-0.0.4.tar` & `hugchat-0.0.5.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-01 00:48:05.688083 hugchat-0.0.4/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    34523 2023-05-01 00:33:11.000000 hugchat-0.0.4/LICENSE
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1688 2023-05-01 00:48:05.688083 hugchat-0.0.4/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      670 2023-05-01 00:33:11.000000 hugchat-0.0.4/README.md
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-05-01 00:48:05.688083 hugchat-0.0.4/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1405 2023-05-01 00:35:41.000000 hugchat-0.0.4/setup.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-01 00:48:05.684083 hugchat-0.0.4/src/
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-01 00:48:05.684083 hugchat-0.0.4/src/hugchat/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4076 2023-05-01 00:43:53.000000 hugchat-0.0.4/src/hugchat/hugchat.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-01 00:48:05.684083 hugchat-0.0.4/src/hugchat.egg-info/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1688 2023-05-01 00:48:05.000000 hugchat-0.0.4/src/hugchat.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      223 2023-05-01 00:48:05.000000 hugchat-0.0.4/src/hugchat.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-05-01 00:48:05.000000 hugchat-0.0.4/src/hugchat.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        9 2023-05-01 00:48:05.000000 hugchat-0.0.4/src/hugchat.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        8 2023-05-01 00:48:05.000000 hugchat-0.0.4/src/hugchat.egg-info/top_level.txt
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-01 18:00:57.589077 hugchat-0.0.5.1/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    34523 2023-05-01 00:33:11.000000 hugchat-0.0.5.1/LICENSE
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1690 2023-05-01 18:00:57.589077 hugchat-0.0.5.1/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      670 2023-05-01 00:33:11.000000 hugchat-0.0.5.1/README.md
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-05-01 18:00:57.589077 hugchat-0.0.5.1/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1407 2023-05-01 18:00:50.000000 hugchat-0.0.5.1/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-01 18:00:57.585077 hugchat-0.0.5.1/src/
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-01 18:00:57.589077 hugchat-0.0.5.1/src/hugchat/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4696 2023-05-01 17:58:33.000000 hugchat-0.0.5.1/src/hugchat/hugchat.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-01 18:00:57.589077 hugchat-0.0.5.1/src/hugchat.egg-info/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1690 2023-05-01 18:00:57.000000 hugchat-0.0.5.1/src/hugchat.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      223 2023-05-01 18:00:57.000000 hugchat-0.0.5.1/src/hugchat.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-05-01 18:00:57.000000 hugchat-0.0.5.1/src/hugchat.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        9 2023-05-01 18:00:57.000000 hugchat-0.0.5.1/src/hugchat.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        8 2023-05-01 18:00:57.000000 hugchat-0.0.5.1/src/hugchat.egg-info/top_level.txt
```

### Comparing `hugchat-0.0.4/LICENSE` & `hugchat-0.0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hugchat-0.0.4/PKG-INFO` & `hugchat-0.0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hugchat
-Version: 0.0.4
+Version: 0.0.5.1
 Summary: A huggingchat python api.
 Home-page: https://github.com/Soulter/hugging-chat-api
 Author: Soulter
 Author-email: 905617992@qq.com
 License: GNU Affero General Public License v3.0
 Project-URL: Bug Report, https://github.com/Soulter/hugging-chat-api/issues
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `hugchat-0.0.4/README.md` & `hugchat-0.0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `hugchat-0.0.4/setup.py` & `hugchat-0.0.5.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import find_namespace_packages
 from setuptools import setup
 
 setup(
     name="hugchat",
-    version="0.0.4",
+    version="0.0.5.1",
     description="A huggingchat python api.",
     long_description=open("README.md", "rt", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/Soulter/hugging-chat-api",
     project_urls={
         "Bug Report": "https://github.com/Soulter/hugging-chat-api/issues"
     },
```

### Comparing `hugchat-0.0.4/src/hugchat/hugchat.py` & `hugchat-0.0.5.1/src/hugchat/hugchat.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,50 +4,55 @@
 
 hf_url = "https://huggingface.co/chat"
 
 
 class ChatBot:
     def __init__(self) -> None:
         self.session = self.get_hc_session()
-        self.conversation_list = []
+        self.conversation_id_list = []
         self.now_conversation = self.new_conversation()
 
     def get_hc_session(self) -> Session:
         session = Session()
         session.get(hf_url)
         return session
     
     def change_conversation(self, conversation_id: str) -> bool:
-        if conversation_id not in self.conversation_list:
+        if conversation_id not in self.conversation_id_list:
             raise Exception("Invalid conversation id. Please check conversation id list.")
         self.now_conversation = conversation_id
         return True
     
+    # Return a list that contains id of conversations.
     def get_conversation_list(self) -> list:
-        return self.conversation_list
+        return self.conversation_id_list
     
     def new_conversation(self) -> str:
         err_count = 0
         resp = ""
         while True:
             try:
                 resp = self.session.post(hf_url + "/conversation")
-                return json.loads(resp.text)['conversationId']
+                cid = json.loads(resp.text)['conversationId']
+                self.conversation_id_list.append(cid)
+                return cid
             except BaseException as e:
                 err_count += 1
                 print(f"[Error] Failed to create new conversation. Retrying... ({err_count})")
                 if err_count > 5:
                     raise e
                 continue
 
     def get_cookies(self) -> dict:
         return self.session.cookies.get_dict()
         
 
-    def chat(self, text: str, temperature=0.9, top_p=0.95, repetition_penalty=1.2, top_k=50, truncate=1024, watermark=False, max_new_tokens=1024, stop=["</s>"], return_full_text=False, stream=True, use_cache=False, is_retry=False) -> str:
+    def chat(self, text: str, temperature=0.9, top_p=0.95, repetition_penalty=1.2, top_k=50, truncate=1024, watermark=False, max_new_tokens=1024, stop=["</s>"], return_full_text=False, stream=True, use_cache=False, is_retry=False, retry_count=5) -> str:
+        if retry_count <= 0:
+            raise Exception("the parameter retry_count must be greater than 0.")
         if self.now_conversation == "":
             self.now_conversation = self.new_conversation()
         req_json = {
             "inputs": text,
             "parameters": {
                 "temperature": temperature,
                 "top_p": top_p,
@@ -75,31 +80,44 @@
             "Sec-Fetch-Dest": "empty",
             "Sec-Fetch-Mode": "cors",
             "Sec-Fetch-Site": "same-origin",
             "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/112.0.0.0 Safari/537.36 Edg/112.0.1722.64",
             "Content-Type": "application/json",
             "Accept": "*/*",
         }
-        resp = self.session.post(hf_url + f"/conversation/{self.now_conversation}", json=req_json, stream=True, headers=headers, cookies=self.session.cookies.get_dict())
-        res_text = ""
-        if resp.status_code == 200:
-            for line in resp.iter_lines():
-                if line:
-                    res = line.decode("utf-8")
-                    obj = json.loads(res[1:-1])
-                    if "generated_text" in obj:
-                        self.conversation_list.append(obj["generated_text"])
-                        res_text += obj["generated_text"]
-                    elif "error" in obj:
-                        raise Exception(obj["error"])
-            return res_text
-        else:
-            raise Exception(f"Failed to chat. Status code: {resp.status_code}")
-    
 
-if __name__ == "__main__":
+        while retry_count > 0:
+            resp = self.session.post(hf_url + f"/conversation/{self.now_conversation}", json=req_json, stream=True, headers=headers, cookies=self.session.cookies.get_dict())
+            res_text = ""
+            if resp.status_code == 200:
+                for line in resp.iter_lines():
+                    if line:
+                        res = line.decode("utf-8")
+                        obj = json.loads(res[1:-1])
+                        if "generated_text" in obj:
+                            res_text += obj["generated_text"]
+                        elif "error" in obj:
+                            raise Exception(obj["error"])
+                return res_text
+            else:
+                retry_count -= 1
+                if retry_count <= 0:
+                    raise Exception(f"Failed to chat. ({resp.status_code})")
+
+def cli():
     chatbot = ChatBot()
     print("-----HuggingChat-----")
     while True:
         question = input("> ")
+        if question == "/new":
+            cid = chatbot.new_conversation()
+            print("the new conversation id is: " + cid)
+            chatbot.change_conversation(cid)
+            print("conversation changed successfully.")
+            continue
         res = chatbot.chat(question)
         print("< " + res)
+    
+
+if __name__ == "__main__":
+    cli()
+
```

### Comparing `hugchat-0.0.4/src/hugchat.egg-info/PKG-INFO` & `hugchat-0.0.5.1/src/hugchat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hugchat
-Version: 0.0.4
+Version: 0.0.5.1
 Summary: A huggingchat python api.
 Home-page: https://github.com/Soulter/hugging-chat-api
 Author: Soulter
 Author-email: 905617992@qq.com
 License: GNU Affero General Public License v3.0
 Project-URL: Bug Report, https://github.com/Soulter/hugging-chat-api/issues
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

