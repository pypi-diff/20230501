# Comparing `tmp/python_voice_assistant-0.0.1.tar.gz` & `tmp/python_voice_assistant-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_voice_assistant-0.0.1.tar", max compression
+gzip compressed data, was "python_voice_assistant-1.0.1.tar", max compression
```

## Comparing `python_voice_assistant-0.0.1.tar` & `python_voice_assistant-1.0.1.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0      614 2023-04-29 11:10:00.377926 python_voice_assistant-0.0.1/pyproject.toml
--rw-r--r--   0        0        0       52 2023-04-28 14:37:23.261030 python_voice_assistant-0.0.1/python_voice_assistant/__init__.py
--rw-r--r--   0        0        0     2988 2023-04-28 21:57:34.984858 python_voice_assistant-0.0.1/python_voice_assistant/Helper.py
--rw-r--r--   0        0        0      152 2023-04-27 13:59:40.355889 python_voice_assistant-0.0.1/python_voice_assistant/languages/en.json
--rw-r--r--   0        0        0      239 2023-04-27 13:59:40.356890 python_voice_assistant-0.0.1/python_voice_assistant/languages/ru.json
--rw-r--r--   0        0        0     5728 2023-04-29 10:42:45.085407 python_voice_assistant-0.0.1/python_voice_assistant/Listener.py
--rw-r--r--   0        0        0      664 2023-04-28 14:37:23.262024 python_voice_assistant-0.0.1/python_voice_assistant/settings.py
--rw-r--r--   0        0        0     1090 2023-04-28 21:57:12.282313 python_voice_assistant-0.0.1/python_voice_assistant/Speaker.py
--rw-r--r--   0        0        0      839 2023-04-29 11:01:22.770789 python_voice_assistant-0.0.1/README.md
--rw-r--r--   0        0        0     1704 1970-01-01 00:00:00.000000 python_voice_assistant-0.0.1/setup.py
--rw-r--r--   0        0        0     1485 1970-01-01 00:00:00.000000 python_voice_assistant-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      970 2023-05-01 09:49:00.984520 python_voice_assistant-1.0.1/README.md
+-rw-r--r--   0        0        0      589 2023-05-01 09:49:20.464616 python_voice_assistant-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2896 2023-05-01 09:49:00.984520 python_voice_assistant-1.0.1/python_voice_assistant/Helper.py
+-rw-r--r--   0        0        0     5575 2023-05-01 09:49:00.984520 python_voice_assistant-1.0.1/python_voice_assistant/Listener.py
+-rw-r--r--   0        0        0     1053 2023-05-01 09:49:00.984520 python_voice_assistant-1.0.1/python_voice_assistant/Speaker.py
+-rw-r--r--   0        0        0       48 2023-05-01 09:49:00.984520 python_voice_assistant-1.0.1/python_voice_assistant/__init__.py
+-rw-r--r--   0        0        0      147 2023-05-01 09:49:00.984520 python_voice_assistant-1.0.1/python_voice_assistant/languages/en.json
+-rw-r--r--   0        0        0      234 2023-05-01 09:49:00.984520 python_voice_assistant-1.0.1/python_voice_assistant/languages/ru.json
+-rw-r--r--   0        0        0      636 2023-05-01 09:49:00.984520 python_voice_assistant-1.0.1/python_voice_assistant/settings.py
+-rw-r--r--   0        0        0     1649 1970-01-01 00:00:00.000000 python_voice_assistant-1.0.1/PKG-INFO
```

### Comparing `python_voice_assistant-0.0.1/pyproject.toml` & `python_voice_assistant-1.0.1/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-[tool.poetry]
-name = "python-voice-assistant"
-version = "0.0.1"
-description = "Create your own voice assistant like jarvis"
-authors = ["Zeph1rr <grianton535@gmail.com>"]
-readme = "README.md"
-packages = [{include = "python_voice_assistant"}]
-
-[tool.poetry.dependencies]
-python = "^3.10"
-vosk = "^0.3.45"
-loguru = "^0.7.0"
-silero = "^0.4.1"
-sounddevice = "^0.4.6"
-numpy = "^1.24.3"
-pydantic = "^1.10.7"
-python-dotenv = "^1.0.0"
-
-[tool.poetry.group.dev.dependencies]
-pre-commit = "^3.2.2"
-pytest = "^7.3.1"
-
-[build-system]
-requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
+[tool.poetry]
+name = "python-voice-assistant"
+version = "1.0.1"
+description = "Create your own voice assistant like jarvis"
+authors = ["Zeph1rr <grianton535@gmail.com>"]
+readme = "README.md"
+packages = [{include = "python_voice_assistant"}]
+
+[tool.poetry.dependencies]
+python = "^3.10"
+vosk = "^0.3.45"
+loguru = "^0.7.0"
+silero = "^0.4.1"
+sounddevice = "^0.4.6"
+numpy = "^1.24.3"
+pydantic = "^1.10.7"
+python-dotenv = "^1.0.0"
+
+[tool.poetry.group.dev.dependencies]
+pre-commit = "^3.2.2"
+pytest = "^7.3.1"
+
+[build-system]
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `python_voice_assistant-0.0.1/python_voice_assistant/Speaker.py` & `python_voice_assistant-1.0.1/python_voice_assistant/Speaker.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,39 @@
-import time
-
-import sounddevice as sd
-import torch
-from loguru import logger
-
-from .settings import settings
-
-
-class Speaker:
-    """Class for generating speech by text"""
-    def __init__(self) -> None:
-        self.model, _ = torch.hub.load(
-            repo_or_dir=settings.repo_or_dir,
-            model=settings.model,
-            language=settings.language,
-            speaker=settings.model_id,
-        )
-        self.model.to(torch.device(settings.device_type))
-        logger.debug("Speaker initialized")
-
-    def say(self, text: str):
-        """
-        Мethod for generating and playing sound
-
-        :param text: message for converting and playing
-        :type text: str
-        """
-        audio = self.model.apply_tts(
-            text=text,
-            speaker=settings.speaker,
-            sample_rate=settings.sample_rate,
-            put_accent=settings.put_accent,
-            put_yo=settings.put_yo,
-        )
-        sd.play(audio, settings.sample_rate)
-        time.sleep(len(audio) / settings.sample_rate)
-        sd.stop()
+import time
+
+import sounddevice as sd
+import torch
+from loguru import logger
+
+from .settings import settings
+
+
+class Speaker:
+    """Class for generating speech by text"""
+
+    def __init__(self) -> None:
+        self.model, _ = torch.hub.load(
+            repo_or_dir=settings.repo_or_dir,
+            model=settings.model,
+            language=settings.language,
+            speaker=settings.model_id,
+        )
+        self.model.to(torch.device(settings.device_type))
+        logger.debug("Speaker initialized")
+
+    def say(self, text: str):
+        """
+        Мethod for generating and playing sound
+
+        :param text: message for converting and playing
+        :type text: str
+        """
+        audio = self.model.apply_tts(
+            text=text,
+            speaker=settings.speaker,
+            sample_rate=settings.sample_rate,
+            put_accent=settings.put_accent,
+            put_yo=settings.put_yo,
+        )
+        sd.play(audio, settings.sample_rate)
+        time.sleep(len(audio) / settings.sample_rate)
+        sd.stop()
```

### Comparing `python_voice_assistant-0.0.1/PKG-INFO` & `python_voice_assistant-1.0.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-voice-assistant
-Version: 0.0.1
+Version: 1.0.1
 Summary: Create your own voice assistant like jarvis
 Author: Zeph1rr
 Author-email: grianton535@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -21,15 +21,15 @@
 
 <p align="center">
       <img src="https://i.ibb.co/MZ3PgBR/python-voice-assistant.png" alt="Project Logo" width="726">
 </p>
 
 <p align="center">
     <img src="https://img.shields.io/badge/Python-3.10-blueviolet" alt="Python Version">
-    <img src="https://img.shields.io/badge/Version-1.0.0-blue" alt="Game Version">
+    <img src="https://img.shields.io/pypi/v/python-voice-assistant?color=blue&label=Version" alt="Package version">
     <img src="https://img.shields.io/badge/License-MIT-success" alt="License">
 </p>
 
 ## About
 
 Python package for creating your own voice assistants like Siri or Jarvis
 
@@ -37,17 +37,18 @@
 
 ```
 pip install python_voice_assistant
 ```
 
 ## Documentation
 
-- [Русский](docs/ru_doc.md)
-- [English](docs/en_doc.md)
+- [Русский](https://github.com/zeph1rrinc/python_voice_assistant/tree/master/docs/ru_doc.md)
+- [English](https://github.com/zeph1rrinc/python_voice_assistant/tree/master/docs/en_doc.md)
 
 ## CONTRIBUTORS
 
 - [Zeph1rr](https://github.com/Zeph1rr) (Developer)
 
 ## License
 
 Project Python voice assistant is distributed under the MIT license.
+
```

