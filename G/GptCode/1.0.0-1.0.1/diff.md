# Comparing `tmp/GptCode-1.0.0.tar.gz` & `tmp/GptCode-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GptCode-1.0.0.tar", last modified: Mon May  1 15:16:50 2023, max compression
+gzip compressed data, was "GptCode-1.0.1.tar", last modified: Mon May  1 15:28:51 2023, max compression
```

## Comparing `GptCode-1.0.0.tar` & `GptCode-1.0.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 15:16:50.196520 GptCode-1.0.0/
-drwxrwxrwx   0        0        0        0 2023-05-01 15:16:50.176815 GptCode-1.0.0/GptCode/
--rw-rw-rw-   0        0        0        0 2023-05-01 13:39:37.000000 GptCode-1.0.0/GptCode/__init__.py
--rw-rw-rw-   0        0        0     2660 2023-05-01 13:40:50.000000 GptCode-1.0.0/GptCode/gpt.py
-drwxrwxrwx   0        0        0        0 2023-05-01 15:16:50.191426 GptCode-1.0.0/GptCode.egg-info/
--rw-rw-rw-   0        0        0      165 2023-05-01 15:16:50.000000 GptCode-1.0.0/GptCode.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      167 2023-05-01 15:16:50.000000 GptCode-1.0.0/GptCode.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 15:16:50.000000 GptCode-1.0.0/GptCode.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-01 15:16:50.000000 GptCode-1.0.0/GptCode.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      165 2023-05-01 15:16:50.194425 GptCode-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-05-01 15:16:50.196520 GptCode-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      369 2023-05-01 15:16:43.000000 GptCode-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 15:28:51.538740 GptCode-1.0.1/
+drwxrwxrwx   0        0        0        0 2023-05-01 15:28:51.520804 GptCode-1.0.1/GptCode/
+-rw-rw-rw-   0        0        0        0 2023-05-01 13:39:37.000000 GptCode-1.0.1/GptCode/__init__.py
+-rw-rw-rw-   0        0        0     2994 2023-05-01 15:28:27.000000 GptCode-1.0.1/GptCode/gpt.py
+drwxrwxrwx   0        0        0        0 2023-05-01 15:28:51.534740 GptCode-1.0.1/GptCode.egg-info/
+-rw-rw-rw-   0        0        0      165 2023-05-01 15:28:51.000000 GptCode-1.0.1/GptCode.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      167 2023-05-01 15:28:51.000000 GptCode-1.0.1/GptCode.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 15:28:51.000000 GptCode-1.0.1/GptCode.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-01 15:28:51.000000 GptCode-1.0.1/GptCode.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      165 2023-05-01 15:28:51.537740 GptCode-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-05-01 15:28:51.538740 GptCode-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      369 2023-05-01 15:28:27.000000 GptCode-1.0.1/setup.py
```

### Comparing `GptCode-1.0.0/GptCode/gpt.py` & `GptCode-1.0.1/GptCode/gpt.py`

 * *Files 21% similar despite different names*

```diff
@@ -41,16 +41,24 @@
 
     def get_answer(self, messages):
         response = openai.ChatCompletion.create(model=self.model, messages=messages)
         answer = response.choices[0].message['content']
         return answer
 
     # 提示chatgpt
-    def ask(self, prompt, use_history=False, history_number=5):
-        prompt = self.generate_prompt(prompt)
+    def ask(self, prompt,reference = False, use_history=False, history_number=5):
+        """
+        :param prompt:问题描述
+        :param reference: 是否列出参考的资料来源
+        :param use_history: 是否参考历史对话信息
+        :param history_number: 参考历史对话信息的条数
+        :return: 此次问题的回复
+        """
+        if reference:
+            prompt = self.generate_prompt(prompt)
         self.conversation_list.append({"role": "user", "content": prompt})
         if use_history:
             # 基于历史history_number条提问记录和当前问题进行回答,虽然会结合上下文，但是会比较耗token
             response = self.get_answer(messages=self.system_setting_list + self.conversation_list[-history_number:])
         else:
             # 只基于当前问题进行回答
             response = self.get_answer(messages=self.system_setting_list + [{'role': 'user', 'content': prompt}])
```

