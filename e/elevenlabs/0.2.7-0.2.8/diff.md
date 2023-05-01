# Comparing `tmp/elevenlabs-0.2.7.tar.gz` & `tmp/elevenlabs-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elevenlabs-0.2.7.tar", last modified: Tue Apr 25 22:54:36 2023, max compression
+gzip compressed data, was "elevenlabs-0.2.8.tar", last modified: Mon May  1 15:14:18 2023, max compression
```

## Comparing `elevenlabs-0.2.7.tar` & `elevenlabs-0.2.8.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 22:54:36.109975 elevenlabs-0.2.7/
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-25 22:54:36.109975 elevenlabs-0.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6710 2023-04-25 22:54:21.000000 elevenlabs-0.2.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 22:54:36.109975 elevenlabs-0.2.7/elevenlabs/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-25 22:54:21.000000 elevenlabs-0.2.7/elevenlabs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 22:54:36.109975 elevenlabs-0.2.7/elevenlabs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-25 22:54:21.000000 elevenlabs-0.2.7/elevenlabs/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-04-25 22:54:21.000000 elevenlabs-0.2.7/elevenlabs/api/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-04-25 22:54:21.000000 elevenlabs-0.2.7/elevenlabs/api/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-04-25 22:54:21.000000 elevenlabs-0.2.7/elevenlabs/api/history.py
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-04-25 22:54:21.000000 elevenlabs-0.2.7/elevenlabs/api/tts.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-25 22:54:21.000000 elevenlabs-0.2.7/elevenlabs/api/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-04-25 22:54:21.000000 elevenlabs-0.2.7/elevenlabs/api/voice.py
--rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-04-25 22:54:21.000000 elevenlabs-0.2.7/elevenlabs/simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-04-25 22:54:21.000000 elevenlabs-0.2.7/elevenlabs/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 22:54:36.109975 elevenlabs-0.2.7/elevenlabs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-25 22:54:36.000000 elevenlabs-0.2.7/elevenlabs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-25 22:54:36.000000 elevenlabs-0.2.7/elevenlabs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 22:54:36.000000 elevenlabs-0.2.7/elevenlabs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-25 22:54:36.000000 elevenlabs-0.2.7/elevenlabs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-25 22:54:36.000000 elevenlabs-0.2.7/elevenlabs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 22:54:36.109975 elevenlabs-0.2.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-04-25 22:54:21.000000 elevenlabs-0.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:14:18.890002 elevenlabs-0.2.8/
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-05-01 15:14:18.890002 elevenlabs-0.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7068 2023-05-01 15:14:04.000000 elevenlabs-0.2.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:14:18.886002 elevenlabs-0.2.8/elevenlabs/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-01 15:14:04.000000 elevenlabs-0.2.8/elevenlabs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:14:18.890002 elevenlabs-0.2.8/elevenlabs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-01 15:14:04.000000 elevenlabs-0.2.8/elevenlabs/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-05-01 15:14:04.000000 elevenlabs-0.2.8/elevenlabs/api/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-05-01 15:14:04.000000 elevenlabs-0.2.8/elevenlabs/api/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-05-01 15:14:04.000000 elevenlabs-0.2.8/elevenlabs/api/history.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-01 15:14:04.000000 elevenlabs-0.2.8/elevenlabs/api/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-05-01 15:14:04.000000 elevenlabs-0.2.8/elevenlabs/api/tts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-01 15:14:04.000000 elevenlabs-0.2.8/elevenlabs/api/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-05-01 15:14:04.000000 elevenlabs-0.2.8/elevenlabs/api/voice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-05-01 15:14:04.000000 elevenlabs-0.2.8/elevenlabs/simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-05-01 15:14:04.000000 elevenlabs-0.2.8/elevenlabs/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:14:18.886002 elevenlabs-0.2.8/elevenlabs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-05-01 15:14:18.000000 elevenlabs-0.2.8/elevenlabs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-05-01 15:14:18.000000 elevenlabs-0.2.8/elevenlabs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 15:14:18.000000 elevenlabs-0.2.8/elevenlabs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-01 15:14:18.000000 elevenlabs-0.2.8/elevenlabs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-01 15:14:18.000000 elevenlabs-0.2.8/elevenlabs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 15:14:18.890002 elevenlabs-0.2.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-01 15:14:04.000000 elevenlabs-0.2.8/setup.py
```

### Comparing `elevenlabs-0.2.7/PKG-INFO` & `elevenlabs-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elevenlabs
-Version: 0.2.7
+Version: 0.2.8
 Summary: The official elevenlabs python package.
 Home-page: https://github.com/elevenlabs/elevenlabs-python
 Author: Elevenlabs
 Keywords: artificial intelligence,deep learning
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
```

### Comparing `elevenlabs-0.2.7/README.md` & `elevenlabs-0.2.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -12,39 +12,22 @@
 ```bash
 pip install elevenlabs
 ```
 
 ## 🗣️ Usage
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/gist/flavioschneider/49468d728a816c6538fd2f56b3b50b96/elevenlabs-python.ipynb)
 
-```py
-from elevenlabs import generate, play
-
-audio = generate("Hi! I'm the world's most advanced text-to-speech system, made by elevenlabs.")
-
-play(audio)
-```
-
-<details> <summary> Play </summary>
-
-<i> Don't forget to unmute the player! </i>
-
-[voice.webm](https://user-images.githubusercontent.com/12028621/232730309-e47bc907-78ec-4acf-a73a-0d77ba25fd6b.webm)
-
-</details>
-
-## 👥 Voices
 
 ```py
 from elevenlabs import generate, play
 
-voice = "Bella"
 audio = generate(
-  text=f"Hi! My name is {voice}, nice to meet you!",
-  voice=voice
+  text="Hi! My name is Bella, nice to meet you!",
+  voice="Bella",
+  model="eleven_monolingual_v1"
 )
 
 play(audio)
 ```
 
 <details> <summary> Play </summary>
 
@@ -84,16 +67,41 @@
 
 <b>Sam</b>
 
 [Sam.webm](https://user-images.githubusercontent.com/12028621/232731428-18bca274-6b84-42e4-b4d8-819b0bd0a19a.webm)
 
 </details>
 
-### List
+## 🌎 Multilingual
 
+The `eleven_multilingual_v1` model supports multiple languages, including English, German, Polish, Spanish, Italian, French, Portuguese, and Hindi.
+```py
+from elevenlabs import generate, play
+
+audio = generate(
+    text="¡Hola! Mi nombre es Arnold, encantado de conocerte!",
+    voice="Arnold",
+    model='eleven_multilingual_v1'
+)
+
+play(audio)
+```
+
+<details> <summary> Play </summary>
+
+<i> Don't forget to unmute the player! </i>
+
+[hola.webm](https://user-images.githubusercontent.com/12028621/235474694-584f7103-dab2-4c39-bb9a-8e5f00be85da.webm)
+
+</details>
+
+
+## 🗣️ Voices
+
+List all your available voices with `voices()`.
 ```py
 from elevenlabs import voices, generate
 
 voices = voices()
 
 audio = generate(text="Hello there!", voice=voices[0])
 
@@ -180,17 +188,17 @@
     ]
 )
 ```
 
 </details>
 
 
-### Add Clone
+### Clone Voice
 
-Note that voice cloning requires an API key, see below.
+Clone your voice in an instant. Note that voice cloning requires an API key, see below.
 
 ```py
 from elevenlabs import clone, generate
 
 voice = clone(
     name="Alex",
     description="An old American male voice with a slight hoarseness in his throat. Perfect for news", # Optional
@@ -200,14 +208,16 @@
 audio = generate(text="Hi! I'm a cloned voice!", voice=voice)
 
 play(audio)
 ```
 
 ## 🚿 Streaming
 
+Stream audio in real-time, as it's being generated.
+
 ```py
 from elevenlabs import generate, stream
 
 audio_stream = generate(
   text="This is a... streaming voice!!",
   stream=True
 )
```

### Comparing `elevenlabs-0.2.7/elevenlabs/api/base.py` & `elevenlabs-0.2.8/elevenlabs/api/base.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-0.2.7/elevenlabs/api/error.py` & `elevenlabs-0.2.8/elevenlabs/api/error.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-0.2.7/elevenlabs/api/history.py` & `elevenlabs-0.2.8/elevenlabs/api/history.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-0.2.7/elevenlabs/api/tts.py` & `elevenlabs-0.2.8/elevenlabs/api/tts.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,38 @@
 from __future__ import annotations
 
 from collections.abc import Iterator
 
 from .base import API, api_base_url_v1
+from .model import Model
 from .voice import Voice
 
 
 class TTS(API):
     @staticmethod
-    def generate(text: str, voice: Voice) -> bytes:
+    def generate(text: str, voice: Voice, model: Model) -> bytes:
         url = f"{api_base_url_v1}/text-to-speech/{voice.voice_id}"
         data = dict(
-            text=text, voice_settings=voice.settings.dict() if voice.settings else None
+            text=text,
+            model_id=model.model_id,
+            voice_settings=voice.settings.dict() if voice.settings else None,
         )  # type: ignore
         response = API.post(url, json=data)
         return response.content
 
     @staticmethod
     def generate_stream(
-        text: str, voice: Voice, stream_chunk_size: int = 2048
+        text: str,
+        voice: Voice,
+        model: Model,
+        stream_chunk_size: int = 2048,
     ) -> Iterator[bytes]:
         url = f"{api_base_url_v1}/text-to-speech/{voice.voice_id}/stream"
         data = dict(
-            text=text, voice_settings=voice.settings.dict() if voice.settings else None
+            text=text,
+            model_id=model.model_id,
+            voice_settings=voice.settings.dict() if voice.settings else None,
         )  # type: ignore
         response = API.post(url, json=data, stream=True)
         for chunk in response.iter_content(chunk_size=stream_chunk_size):
             if chunk:
                 yield chunk
```

### Comparing `elevenlabs-0.2.7/elevenlabs/api/voice.py` & `elevenlabs-0.2.8/elevenlabs/api/voice.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-0.2.7/elevenlabs/simple.py` & `elevenlabs-0.2.8/elevenlabs/simple.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import re
 from collections.abc import Iterator
 from typing import List, Optional, Union
 
-from .api import TTS, Voice, VoiceClone, Voices, VoiceSettings
+from .api import TTS, Model, Voice, VoiceClone, Voices, VoiceSettings
 
 
 def set_api_key(api_key: str) -> None:
     os.environ["ELEVEN_API_KEY"] = api_key
 
 
 def get_api_key() -> Optional[str]:
@@ -91,14 +91,15 @@
     return bool(re.match(r"^[a-zA-Z0-9]{20}$", val))
 
 
 def generate(
     text: str,
     api_key: Optional[str] = None,
     voice: Union[str, Voice] = VOICES_CACHE[2],  # Bella
+    model: Union[str, Model] = "eleven_monolingual_v1",
     stream: bool = False,
     stream_chunk_size: int = 2048,
 ) -> Union[bytes, Iterator[bytes]]:
     if api_key:
         set_api_key(api_key)
 
     if isinstance(voice, str):
@@ -112,13 +113,17 @@
             voice = next((v for v in VOICES_CACHE if v.name == voice), None)  # type: ignore # noqa E501
             # If not, query API
             voice = next((v for v in voices() if v.name == voice), None) if not voice else voice  # type: ignore # noqa E501
         # Raise error if voice not found
         if not voice:
             raise ValueError(f"Voice '{voice_str}' not found.")
 
+    if isinstance(model, str):
+        model = Model(model_id=model)
+
     assert isinstance(voice, Voice)
+    assert isinstance(model, Model)
 
     if stream:
-        return TTS.generate_stream(text, voice, stream_chunk_size)
+        return TTS.generate_stream(text, voice, model, stream_chunk_size)
     else:
-        return TTS.generate(text, voice)
+        return TTS.generate(text, voice, model)
```

### Comparing `elevenlabs-0.2.7/elevenlabs/utils.py` & `elevenlabs-0.2.8/elevenlabs/utils.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-0.2.7/elevenlabs.egg-info/PKG-INFO` & `elevenlabs-0.2.8/elevenlabs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elevenlabs
-Version: 0.2.7
+Version: 0.2.8
 Summary: The official elevenlabs python package.
 Home-page: https://github.com/elevenlabs/elevenlabs-python
 Author: Elevenlabs
 Keywords: artificial intelligence,deep learning
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
```

### Comparing `elevenlabs-0.2.7/setup.py` & `elevenlabs-0.2.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import find_packages, setup
 
 setup(
     name="elevenlabs",
     packages=find_packages(exclude=[]),
-    version="0.2.7",
+    version="0.2.8",
     description="The official elevenlabs python package.",
     long_description_content_type="text/markdown",
     author="Elevenlabs",
     url="https://github.com/elevenlabs/elevenlabs-python",
     keywords=["artificial intelligence", "deep learning"],
     install_requires=[
         "pydantic>=1.10",
```

