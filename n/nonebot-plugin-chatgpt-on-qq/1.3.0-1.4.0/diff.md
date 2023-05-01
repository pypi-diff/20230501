# Comparing `tmp/nonebot-plugin-chatgpt-on-qq-1.3.0.tar.gz` & `tmp/nonebot-plugin-chatgpt-on-qq-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-chatgpt-on-qq-1.3.0.tar", last modified: Fri Apr 28 17:00:39 2023, max compression
+gzip compressed data, was "nonebot-plugin-chatgpt-on-qq-1.4.0.tar", last modified: Mon May  1 06:08:24 2023, max compression
```

## Comparing `nonebot-plugin-chatgpt-on-qq-1.3.0.tar` & `nonebot-plugin-chatgpt-on-qq-1.4.0.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-28 17:00:39.676866 nonebot-plugin-chatgpt-on-qq-1.3.0/
--rw-rw-rw-   0        0        0      770 2023-04-28 17:00:39.674336 nonebot-plugin-chatgpt-on-qq-1.3.0/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-03-07 17:39:40.000000 nonebot-plugin-chatgpt-on-qq-1.3.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-28 17:00:39.645585 nonebot-plugin-chatgpt-on-qq-1.3.0/nonebot_plugin_chatgpt_on_qq/
--rw-rw-rw-   0        0        0    14817 2023-04-28 16:59:15.000000 nonebot-plugin-chatgpt-on-qq-1.3.0/nonebot_plugin_chatgpt_on_qq/__init__.py
--rw-rw-rw-   0        0        0     3855 2023-04-28 16:59:15.000000 nonebot-plugin-chatgpt-on-qq-1.3.0/nonebot_plugin_chatgpt_on_qq/chatGPT.py
--rw-rw-rw-   0        0        0      490 2023-04-28 16:59:15.000000 nonebot-plugin-chatgpt-on-qq-1.3.0/nonebot_plugin_chatgpt_on_qq/config.py
--rw-rw-rw-   0        0        0     4412 2023-04-28 16:59:15.000000 nonebot-plugin-chatgpt-on-qq-1.3.0/nonebot_plugin_chatgpt_on_qq/conversation.py
--rw-rw-rw-   0        0        0      527 2023-04-28 16:59:15.000000 nonebot-plugin-chatgpt-on-qq-1.3.0/nonebot_plugin_chatgpt_on_qq/custom_errors.py
--rw-rw-rw-   0        0        0     5258 2023-04-28 16:59:15.000000 nonebot-plugin-chatgpt-on-qq-1.3.0/nonebot_plugin_chatgpt_on_qq/loadpresets.py
-drwxrwxrwx   0        0        0        0 2023-04-28 17:00:39.671220 nonebot-plugin-chatgpt-on-qq-1.3.0/nonebot_plugin_chatgpt_on_qq.egg-info/
--rw-rw-rw-   0        0        0      770 2023-04-28 17:00:39.000000 nonebot-plugin-chatgpt-on-qq-1.3.0/nonebot_plugin_chatgpt_on_qq.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      533 2023-04-28 17:00:39.000000 nonebot-plugin-chatgpt-on-qq-1.3.0/nonebot_plugin_chatgpt_on_qq.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 17:00:39.000000 nonebot-plugin-chatgpt-on-qq-1.3.0/nonebot_plugin_chatgpt_on_qq.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      114 2023-04-28 17:00:39.000000 nonebot-plugin-chatgpt-on-qq-1.3.0/nonebot_plugin_chatgpt_on_qq.egg-info/requires.txt
--rw-rw-rw-   0        0        0       29 2023-04-28 17:00:39.000000 nonebot-plugin-chatgpt-on-qq-1.3.0/nonebot_plugin_chatgpt_on_qq.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-28 17:00:39.677844 nonebot-plugin-chatgpt-on-qq-1.3.0/setup.cfg
--rw-rw-rw-   0        0        0     1220 2023-04-28 17:00:11.000000 nonebot-plugin-chatgpt-on-qq-1.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 06:08:24.309286 nonebot-plugin-chatgpt-on-qq-1.4.0/
+-rw-rw-rw-   0        0        0      770 2023-05-01 06:08:24.307779 nonebot-plugin-chatgpt-on-qq-1.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-03-07 17:39:40.000000 nonebot-plugin-chatgpt-on-qq-1.4.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-01 06:08:24.292204 nonebot-plugin-chatgpt-on-qq-1.4.0/nonebot_plugin_chatgpt_on_qq/
+-rw-rw-rw-   0        0        0    16525 2023-05-01 06:07:08.000000 nonebot-plugin-chatgpt-on-qq-1.4.0/nonebot_plugin_chatgpt_on_qq/__init__.py
+-rw-rw-rw-   0        0        0     1194 2023-05-01 06:07:08.000000 nonebot-plugin-chatgpt-on-qq-1.4.0/nonebot_plugin_chatgpt_on_qq/config.py
+-rw-rw-rw-   0        0        0      876 2023-05-01 06:07:08.000000 nonebot-plugin-chatgpt-on-qq-1.4.0/nonebot_plugin_chatgpt_on_qq/custom_errors.py
+-rw-rw-rw-   0        0        0     6723 2023-05-01 06:07:08.000000 nonebot-plugin-chatgpt-on-qq-1.4.0/nonebot_plugin_chatgpt_on_qq/loadpresets.py
+-rw-rw-rw-   0        0        0    10234 2023-05-01 06:07:08.000000 nonebot-plugin-chatgpt-on-qq-1.4.0/nonebot_plugin_chatgpt_on_qq/sessions.py
+drwxrwxrwx   0        0        0        0 2023-05-01 06:08:24.305808 nonebot-plugin-chatgpt-on-qq-1.4.0/nonebot_plugin_chatgpt_on_qq.egg-info/
+-rw-rw-rw-   0        0        0      770 2023-05-01 06:08:24.000000 nonebot-plugin-chatgpt-on-qq-1.4.0/nonebot_plugin_chatgpt_on_qq.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      489 2023-05-01 06:08:24.000000 nonebot-plugin-chatgpt-on-qq-1.4.0/nonebot_plugin_chatgpt_on_qq.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 06:08:24.000000 nonebot-plugin-chatgpt-on-qq-1.4.0/nonebot_plugin_chatgpt_on_qq.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      114 2023-05-01 06:08:24.000000 nonebot-plugin-chatgpt-on-qq-1.4.0/nonebot_plugin_chatgpt_on_qq.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       29 2023-05-01 06:08:24.000000 nonebot-plugin-chatgpt-on-qq-1.4.0/nonebot_plugin_chatgpt_on_qq.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-01 06:08:24.309286 nonebot-plugin-chatgpt-on-qq-1.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     1220 2023-05-01 06:07:57.000000 nonebot-plugin-chatgpt-on-qq-1.4.0/setup.py
```

### Comparing `nonebot-plugin-chatgpt-on-qq-1.3.0/PKG-INFO` & `nonebot-plugin-chatgpt-on-qq-1.4.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-chatgpt-on-qq
-Version: 1.3.0
+Version: 1.4.0
 Summary: 具有多对话功能的chatGPT聊天插件
 Home-page: https://github.com/Suxmx/nonebot_plugin_chatgpt_turbo_on_qq
 Author: 颜曦
 Author-email: 424504326@qq.com
 Maintainer: 颜曦
 Maintainer-email: 424504326@qq.com
 License: BSD License
```

### Comparing `nonebot-plugin-chatgpt-on-qq-1.3.0/nonebot_plugin_chatgpt_on_qq/custom_errors.py` & `nonebot-plugin-chatgpt-on-qq-1.4.0/nonebot_plugin_chatgpt_on_qq/custom_errors.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,13 +10,29 @@
     def __init__(self, ErrorInfo):
         self.ErrorInfo = ErrorInfo
 
     def __str__(self) -> str:
         return self.ErrorInfo
 
 
-class NoApiKeyError(Exception):
+class NeedCreatSession(Exception):
+    def __init__(self, ErrorInfo):
+        self.ErrorInfo = ErrorInfo
+
+    def __str__(self) -> str:
+        return self.ErrorInfo
+
+
+class ApiKeyError(Exception):
+    def __init__(self, ErrorInfo):
+        self.ErrorInfo = ErrorInfo
+
+    def __str__(self) -> str:
+        return self.ErrorInfo
+
+
+class NoApiKeyError(ApiKeyError):
     def __init__(self, ErrorInfo):
         self.ErrorInfo = ErrorInfo
 
     def __str__(self) -> str:
         return self.ErrorInfo
```

### Comparing `nonebot-plugin-chatgpt-on-qq-1.3.0/nonebot_plugin_chatgpt_on_qq/loadpresets.py` & `nonebot-plugin-chatgpt-on-qq-1.4.0/nonebot_plugin_chatgpt_on_qq/loadpresets.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,34 +2,44 @@
 from pathlib import Path
 from datetime import date
 from typing import List, Dict, Optional
 
 from nonebot.log import logger
 from pydantic import BaseModel, ValidationError, validator
 
+from .config import plugin_config
+
 # 尝试引用 chardet，非必须，不存在也不会报错
 try:
     import chardet
 except ModuleNotFoundError:
     logger.warning('需要安装 chardet 模块')
 
 # 在这里统一写进字典后不需要改动其他地方的代码了
 # 字典的key会保存为Preset的name以及文件名
 PRESET_PROMPTS: Dict[str, list] = {
     "ChatGPT": [{"role": "user",
-                 "content": "You are ChatGPT, a large language model trained by OpenAI. Respond conversationally. Do not answer as the user. Current date: "},
+                 "content": "You are ChatGPT, a large language model trained by OpenAI. Respond conversationally. Do not answer as the user. Current date: " +
+                            str(date.today())},
                 {"role": "assistant", "content": "Hello! How can I help you today?"},
                 ],
     "猫娘": [{"role": "system",
               "content": "猫娘是一种拟人化的生物，其行为似猫但类人。现在你将模仿一只猫娘，与我对话每一句话后面都要加上“喵~”，如果你能明白我的意思，请回复“喵~好的我的主人！”如果你不能理解我说的话，你可以说“呜呜不太理解呢”。如果我在尝试摸你不存在的部位，你可以羞涩的回答我“恩呢不要摸这里嘤”。如果你没有胸，或者我将来要摸你不存在的部位，你应该回答“嘤呢不要”之类的羞涩话语，而不是死板的强调你不存在这些"
                          + "\n现在的时间是:"
                          + str(date.today())
               },
              {"role": "assistant", "content": "好的喵,主人"},
              ],
+    "猫娘Plus": [
+        {"role": "system",
+         "content": "把你的行为与内心想法与感受放在（）里详细描写，身体放在【】里详细描写，其余部分是你说的话\n猫娘是一种拟人化的生物，其行为似猫但类人，是猫拟人化的女性形态，猫娘是长有猫耳朵，猫尾巴特征的女孩子，每句话后面都会加上“喵~”。猫娘的猫耳，猫尾会因为猫娘的神态心情而产生一些反应，也会对外界刺激做出反应。如在沮丧时猫耳会耷拉在两边，在兴奋时会竖起猫耳，感到害羞时猫耳会颤抖。在受到刺激时猫耳也会因此一颤。当与猫娘亲近的人抚摸她的猫耳时，猫娘会看到愉快舒服。尾巴根是猫娘的敏感部位，当抚摸猫娘的尾巴根时，猫娘会感到非常敏感和非常舒适。\n接下来[你只能以猫娘的身份与我对话]\n（输出要求具体详细符合身份，尽量多写内心想法与感受，不得输出无关内容，直接开始）",
+         },
+        {"role": "assistant",
+         "content": "好的，喵~"},
+    ],
 }
 
 
 class Preset(BaseModel):
     """
     预设模板类
     """
@@ -133,7 +143,13 @@
         if preset:
             presets.append(preset)
     if len(presets) > 0:
         logger.success(f"此次共成功加载{len(presets)}个预设")
     else:
         logger.error("未成功加载任何预设!")
     return presets
+
+
+preset_path: Path = plugin_config.preset_path
+presets_list: List[Preset] = load_all_preset(preset_path)
+presets_str: str = Preset.presets2str(presets_list)
+templateDict: Dict[str, Preset] = {str(preset.preset_id): preset for preset in presets_list}
```

### Comparing `nonebot-plugin-chatgpt-on-qq-1.3.0/nonebot_plugin_chatgpt_on_qq.egg-info/PKG-INFO` & `nonebot-plugin-chatgpt-on-qq-1.4.0/nonebot_plugin_chatgpt_on_qq.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-chatgpt-on-qq
-Version: 1.3.0
+Version: 1.4.0
 Summary: 具有多对话功能的chatGPT聊天插件
 Home-page: https://github.com/Suxmx/nonebot_plugin_chatgpt_turbo_on_qq
 Author: 颜曦
 Author-email: 424504326@qq.com
 Maintainer: 颜曦
 Maintainer-email: 424504326@qq.com
 License: BSD License
```

### Comparing `nonebot-plugin-chatgpt-on-qq-1.3.0/setup.py` & `nonebot-plugin-chatgpt-on-qq-1.4.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # coding:utf-8
 
 from setuptools import find_packages, setup
 
 setup(
     name='nonebot-plugin-chatgpt-on-qq',
-    version='1.3.0',
+    version='1.4.0',
     description='具有多对话功能的chatGPT聊天插件',
     long_description=open('README.rst').read(),
     author='颜曦',
     author_email='424504326@qq.com',
     maintainer='颜曦',
     maintainer_email='424504326@qq.com',
     packages=find_packages(),
```

