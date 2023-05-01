# Comparing `tmp/skainet-0.0.0.dev8.tar.gz` & `tmp/skainet-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/skainet/skainet/dist/.tmp-6ftqtqr_/skainet-0.0.0.dev8.tar", last modified: Mon May  1 17:23:31 2023, max compression
+gzip compressed data, was "/home/runner/work/skainet/skainet/dist/.tmp-px2_gvdp/skainet-0.1.0.tar", last modified: Mon May  1 19:49:14 2023, max compression
```

## Comparing `skainet-0.0.0.dev8.tar` & `skainet-0.1.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:23:31.000000 skainet-0.0.0.dev8/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-01 17:23:31.000000 skainet-0.0.0.dev8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-05-01 17:23:16.000000 skainet-0.0.0.dev8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-05-01 17:23:16.000000 skainet-0.0.0.dev8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 17:23:31.000000 skainet-0.0.0.dev8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:23:31.000000 skainet-0.0.0.dev8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:23:31.000000 skainet-0.0.0.dev8/src/skainet/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 17:23:16.000000 skainet-0.0.0.dev8/src/skainet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-05-01 17:23:16.000000 skainet-0.0.0.dev8/src/skainet/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-05-01 17:23:16.000000 skainet-0.0.0.dev8/src/skainet/audio.py
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-01 17:23:16.000000 skainet-0.0.0.dev8/src/skainet/config.ini
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-01 17:23:16.000000 skainet-0.0.0.dev8/src/skainet/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-05-01 17:23:16.000000 skainet-0.0.0.dev8/src/skainet/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-05-01 17:23:16.000000 skainet-0.0.0.dev8/src/skainet/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     4924 2023-05-01 17:23:16.000000 skainet-0.0.0.dev8/src/skainet/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-05-01 17:23:16.000000 skainet-0.0.0.dev8/src/skainet/model.py
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-05-01 17:23:16.000000 skainet-0.0.0.dev8/src/skainet/moderate.py
--rw-r--r--   0 runner    (1001) docker     (123)    11224 2023-05-01 17:23:16.000000 skainet-0.0.0.dev8/src/skainet/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-05-01 17:23:16.000000 skainet-0.0.0.dev8/src/skainet/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:23:31.000000 skainet-0.0.0.dev8/src/skainet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-01 17:23:31.000000 skainet-0.0.0.dev8/src/skainet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-01 17:23:31.000000 skainet-0.0.0.dev8/src/skainet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 17:23:31.000000 skainet-0.0.0.dev8/src/skainet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-01 17:23:31.000000 skainet-0.0.0.dev8/src/skainet.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-01 17:23:31.000000 skainet-0.0.0.dev8/src/skainet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-01 17:23:31.000000 skainet-0.0.0.dev8/src/skainet.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:49:14.000000 skainet-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-01 19:49:14.000000 skainet-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-05-01 19:48:59.000000 skainet-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-01 19:48:59.000000 skainet-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 19:49:14.000000 skainet-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:49:14.000000 skainet-0.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:49:14.000000 skainet-0.1.0/src/skainet/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:48:59.000000 skainet-0.1.0/src/skainet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-05-01 19:48:59.000000 skainet-0.1.0/src/skainet/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-05-01 19:48:59.000000 skainet-0.1.0/src/skainet/audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-01 19:48:59.000000 skainet-0.1.0/src/skainet/config.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-05-01 19:48:59.000000 skainet-0.1.0/src/skainet/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-05-01 19:48:59.000000 skainet-0.1.0/src/skainet/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-05-01 19:48:59.000000 skainet-0.1.0/src/skainet/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4855 2023-05-01 19:48:59.000000 skainet-0.1.0/src/skainet/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-05-01 19:48:59.000000 skainet-0.1.0/src/skainet/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-01 19:48:59.000000 skainet-0.1.0/src/skainet/moderate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11372 2023-05-01 19:48:59.000000 skainet-0.1.0/src/skainet/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-05-01 19:48:59.000000 skainet-0.1.0/src/skainet/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:49:14.000000 skainet-0.1.0/src/skainet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-01 19:49:14.000000 skainet-0.1.0/src/skainet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-01 19:49:14.000000 skainet-0.1.0/src/skainet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 19:49:14.000000 skainet-0.1.0/src/skainet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-01 19:49:14.000000 skainet-0.1.0/src/skainet.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-01 19:49:14.000000 skainet-0.1.0/src/skainet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-01 19:49:14.000000 skainet-0.1.0/src/skainet.egg-info/top_level.txt
```

### Comparing `skainet-0.0.0.dev8/README.md` & `skainet-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `skainet-0.0.0.dev8/pyproject.toml` & `skainet-0.1.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [project]
 name = "skainet"
-version = "0.0.0.dev8"
+version = "0.1.0"
 authors = [
     {name = "Zach Morris", email = "zacharymorr@outlook.com"}
 ]
 requires-python = ">=3.7"
 dependencies = [
     "openai==0.27.4",
     "click==8.1.3",
@@ -26,22 +26,23 @@
 skainet = ["*.ini"]
 
 [tool.isort]
 profile = "black"
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.0.0"
+version = "0.1.0"
 version_files = [
     "pyproject.toml:^version",
 ]
 
 tag_format = "v$major.$minor.$patch$prerelease"
 bump_message = "release $current_version -> $new_version"
 
+update_changelog_on_bump = true
 changelog_file = "changelog.md"
 changelog_start_rev = "v0.0.0"
 
 style = [
     ["qmark", "fg:#ff9d00 bold"],
     ["question", "bold"],
     ["answer", "fg:#ff9d00 bold"],
```

### Comparing `skainet-0.0.0.dev8/src/skainet/__main__.py` & `skainet-0.1.0/src/skainet/__main__.py`

 * *Files identical despite different names*

### Comparing `skainet-0.0.0.dev8/src/skainet/audio.py` & `skainet-0.1.0/src/skainet/audio.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,17 +110,17 @@
             file=audio,
             temperature=temp,
             format=format,
             prompt=prompt,
             language=lang,
         )
     except openai.OpenAIError as e:
-        utils.handle_error(e)
+        utils.handle_openai_error(e)
     else:
-        print(response["text"])
+        click.echo(response["text"])
 
 
 @audio.command(context_settings={"show_default": True})
 @audio_options()
 def translate(
     audio: BinaryIO,
     prompt: str,
@@ -135,10 +135,10 @@
             model=model,
             file=audio,
             temperature=temp,
             format=format,
             prompt=prompt,
         )
     except openai.OpenAIError as e:
-        utils.handle_error(e)
+        utils.handle_openai_error(e)
     else:
-        print(response["text"])
+        click.echo(response["text"])
```

### Comparing `skainet-0.0.0.dev8/src/skainet/config.py` & `skainet-0.1.0/src/skainet/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,33 +11,33 @@
     """DOCUMENTATION"""
     pass
 
 
 @config.command()
 def show():
     """Display contents of config file"""
-    print(_CONFIG_FILE.read_text())
+    click.echo(_CONFIG_FILE.read_text())
 
 
 @config.command()
 def path():
     """Show path to config file"""
-    print(str(_CONFIG_FILE.absolute()))
+    click.echo(str(_CONFIG_FILE.absolute()))
 
 
 @config.command()
 @click.argument("setting", nargs=-1)
 @click.argument("value", type=str)
 def set(setting: List[str], value: str):
     """Set a variable in the config file"""
     config_path = setting
     try:
         dic = CONFIG
         for key in config_path[:-1]:
             dic = dic[key]
         dic[config_path[-1]] = value
     except KeyError as e:
-        print(f"{' '.join(setting)} does not exist")
+        click.echo(f"{' '.join(setting)} does not exist", err=True)
         sys.exit(1)
 
     with open(_CONFIG_FILE, "w") as configfile:
         CONFIG.write(configfile)
```

### Comparing `skainet-0.0.0.dev8/src/skainet/data.py` & `skainet-0.1.0/src/skainet/data.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,25 +2,27 @@
 import os
 import platform
 import sys
 from configparser import ConfigParser
 from pathlib import Path
 from typing import Dict, List
 
+import click
+
 ## Data Directory
 if platform.system() == "Windows":
     appdata = os.getenv("LOCALAPPDATA")
     DATA_DIR = Path(appdata) / __package__
 else:
     DATA_DIR = Path.home() / ".local" / "share" / __package__
 
 try:
     DATA_DIR.mkdir(parents=True, exist_ok=True)
 except OSError as e:
-    print(f"Error while attempting to create data directory: {e}")
+    click.echo(f"Error while attempting to create data directory: {e}", err=True)
     sys.exit(1)
 
 
 ## Key File
 _KEY_FILE = DATA_DIR / "api_key"
 if not _KEY_FILE.exists():
     _KEY_FILE.touch()
@@ -50,15 +52,15 @@
     with open(_CHAT_FILE, "w") as file:
         json.dump(chat, file, indent=2)
 
 
 # Configuration
 default_config_path = Path(__file__).parent / "config.ini"
 if not default_config_path.exists():
-    print(f"Default config ({default_config_path}) does not exist!")
+    click.echo(f"Default config ({default_config_path}) does not exist!", err=True)
     sys.exit(1)
 
 DEFAULT_CONFIG = ConfigParser()
 DEFAULT_CONFIG.read(default_config_path)
 
 
 # Create config file, copying default config if it doesn't exist
```

### Comparing `skainet-0.0.0.dev8/src/skainet/file.py` & `skainet-0.1.0/src/skainet/file.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,22 +18,22 @@
 
 @file.command()
 def list():
     """List files"""
     try:
         response = openai.File.list()
     except openai.OpenAIError as e:
-        utils.handle_error(e)
+        utils.handle_openai_error(e)
     else:
         if response["data"]:
-            print("Files:")
+            click.echo("Files:")
             for file in response["data"]:
-                print(file)
+                click.echo(file)
         else:
-            print("No files")
+            click.echo("No files")
 
 
 @file.command()
 @click.argument("file", type=click.Path(exists=True, path_type=Path))
 @click.option(
     "-p",
     "--purpose",
@@ -47,31 +47,31 @@
 ):
     """Upload file"""
     try:
         response = openai.File.create(
             file=file.read_text(), purpose=purpose, user_provided_filename=file.name
         )
     except openai.OpenAIError as e:
-        utils.handle_error(e)
+        utils.handle_openai_error(e)
     else:
-        print(response)
+        click.echo(response)
 
 
 @file.command()
 @click.argument("file_id", metavar="ID", type=str)
 def delete(
     file_id: str,
 ):
     """Delete file"""
     try:
         openai.File.delete(
             sid=file_id,
         )
     except openai.OpenAIError as e:
-        utils.handle_error(e)
+        utils.handle_openai_error(e)
     else:
         pass
 
 
 @file.command()
 @click.argument("file_id", metavar="ID", type=str)
 @click.option(
@@ -94,15 +94,15 @@
                     file_name = file_info["filename"]
 
             if not output:
                 output = Path.cwd() / file_name
             else:
                 output = output / file_name
     except openai.OpenAIError as e:
-        utils.handle_error(e)
+        utils.handle_openai_error(e)
     else:
         if output.exists():
             for num in itertools.count(start=1):
                 test_file = output.parent / (output.stem + f"{num}" + output.suffix)
                 if not test_file.exists():
                     output = test_file
                     break
@@ -123,11 +123,11 @@
     try:
         response = openai.File.find_matching_files(
             name=name,
             bytes=size,
             purpose=purpose,
         )
     except openai.OpenAIError as e:
-        utils.handle_error(e)
+        utils.handle_openai_error(e)
     else:
         for file in response:
-            print(file)
+            click.echo(file)
```

### Comparing `skainet-0.0.0.dev8/src/skainet/image.py` & `skainet-0.1.0/src/skainet/image.py`

 * *Files 4% similar despite different names*

```diff
@@ -87,15 +87,15 @@
         response = openai.Image.create(
             prompt=prompt,
             n=num,
             size=size,
             response_format=format,
         )
     except openai.OpenAIError as e:
-        utils.handle_error(e)
+        utils.handle_openai_error(e)
     else:
         display_image_response(response, format, num, print_response)
 
 
 @image.command(context_settings={"show_default": True})
 @click.argument("image", type=utils.File("rb", exts=[".png"]))
 @click.argument("mask", type=utils.File("rb", exts=[".png"]))
@@ -125,15 +125,15 @@
             mask=mask,
             prompt=prompt,
             n=num,
             size=size,
             response_format=format,
         )
     except openai.OpenAIError as e:
-        utils.handle_error(e)
+        utils.handle_openai_error(e)
     else:
         display_image_response(response, format, num, print_response)
 
 
 @image.command(
     help="Create a variation of an image", context_settings={"show_default": True}
 )
@@ -153,15 +153,15 @@
         response = openai.Image.create_variation(
             image=input_image,
             n=num,
             size=size,
             response_format=format,
         )
     except openai.OpenAIError as e:
-        utils.handle_error(e)
+        utils.handle_openai_error(e)
     else:
         display_image_response(response, format, num, print_response)
 
 
 def display_image_response(response, format, num, print_response):
     for index, generation in enumerate(response["data"]):
         if format == "url":
@@ -172,19 +172,14 @@
             temp_file = Path(tempfile.gettempdir()) / str(uuid.uuid4())
             temp_file = temp_file.with_suffix(".png")
             temp_file.write_bytes(decoded_image)
             image = temp_file
 
         if print_response is True:
             if num > 1:
-                print(f"({index}): {image}")
+                click.echo(f"({index}): {image}")
             else:
-                print(f"{image}")
+                click.echo(f"{image}")
         else:
-            try:
-                if format == "b64_json":
-                    image = image.as_uri()
-
-                webbrowser.open(image)
-            except Exception as e:
-                print(f"Error opening image: {e}")
-                sys.exit(1)
+            if format == "b64_json":
+                image = image.as_uri()  # click.launch will fail if given a bare path
+            click.launch(image)
```

### Comparing `skainet-0.0.0.dev8/src/skainet/model.py` & `skainet-0.1.0/src/skainet/model.py`

 * *Files 21% similar despite different names*

```diff
@@ -14,34 +14,34 @@
 
 @model.command()
 def list():
     """List available models"""
     try:
         model_list = openai.Model.list()["data"]
     except openai.OpenAIError as e:
-        utils.handle_error(e)
+        utils.handle_openai_error(e)
     else:
-        print("Available Models:")
+        click.echo("Available Models:")
         model_names = [model["id"] for model in model_list]
         for name in sorted(model_names):
-            print(f"{name}")
+            click.echo(f"{name}")
 
 
 @model.command()
 @click.argument("model_name", type=str)
 def show(model_name: str):
     """Get information about a model"""
     try:
         model_list = openai.Model.list()["data"]
     except openai.OpenAIError as e:
-        utils.handle_error(e)
+        utils.handle_openai_error(e)
     else:
         model_info = {}
         for model in model_list:
             if model["id"] == model_name:
                 model_info = model
 
         if model_info:
-            print(model_info)
+            click.echo(model_info)
         else:
-            print(f"No model with name '{model_name}' found.")
+            click.echo(f"No model with name '{model_name}' found.", err=True)
             sys.exit(1)
```

### Comparing `skainet-0.0.0.dev8/src/skainet/moderate.py` & `skainet-0.1.0/src/skainet/moderate.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,10 +20,10 @@
     """Check if text violates OpenAI's Content Policy"""
     try:
         response = openai.Moderation.create(
             input=input,
             model=model,
         )
     except openai.OpenAIError as e:
-        utils.handle_error(e)
+        utils.handle_openai_error(e)
     else:
-        print(response)
+        click.echo(response)
```

### Comparing `skainet-0.0.0.dev8/src/skainet/text.py` & `skainet-0.1.0/src/skainet/text.py`

 * *Files 3% similar despite different names*

```diff
@@ -135,17 +135,20 @@
     new_prompt = {"role": "user", "content": prompt}
     chat_history.append(new_prompt)
 
     # Limit chat context & instert seed prompt
     available_context = context - SYSTEM_MESSAGE_LEN
     current_context = truncate_context(chat_history, available_context)
     if current_context != chat_history:
-        print(
-            "Warning: your chat history has been truncated to fit the context limit",
-            file=sys.stderr,
+        click.echo(
+            click.style(
+                "Warning: your chat history has been truncated to fit the context limit",
+                fg="yellow",
+            ),
+            err=True,
         )
     current_context.insert(0, SYSTEM_MESSAGE)
 
     # Send request
     try:
         response = openai.ChatCompletion.create(
             model=model,
@@ -157,40 +160,40 @@
             stop=stop,
             max_tokens=maxtokens,
             # presence_penalty=args.presence_penalty,
             # frequency_penalty=args.frequency_penalty,
             # user=args.user
         )
     except openai.OpenAIError as e:
-        utils.handle_error(e)
+        utils.handle_openai_error(e)
     else:
         if num > 1:
             if no_stream:
                 for index, choice in enumerate(response["choices"]):
                     content = choice["message"]["content"]
-                    print(f"({index}) {content}")
+                    click.echo(f"({index}) {content}")
             else:
                 messages = {}
                 for chunk in response:
                     for choice in chunk["choices"]:
                         index = choice["index"]
                         if index not in messages:
                             messages[index] = ""
 
                         delta = choice["delta"]
                         if "content" in delta:
                             content = delta["content"]
                             messages[index] += content
 
                 for index in range(len(messages)):
-                    print(f"({index}) {messages[index]}")
+                    click.echo(f"({index}) {messages[index]}")
         else:
             if no_stream:
                 new_response = response["choices"][0]["message"]
-                print(new_response["content"])
+                click.echo(new_response["content"])
             else:
                 new_response = {"role": "", "content": ""}
                 for chunk in response:
                     # Parse response chunk
                     choice = chunk["choices"][0]
                     delta = choice["delta"]
                     if "role" in delta:
@@ -200,15 +203,15 @@
                         new_response["content"] += delta["content"]
                         text = delta["content"]
                     elif not delta:
                         text = "\n"
                     else:
                         text = ""
 
-                    print(text, end="")
+                    click.echo(text, nl=False)
 
             if not no_update:
                 chat_history.append(new_response)
                 chat_history = truncate_context(chat_history, MAXIMUM_CONTEXT)
                 save_chat(chat_history)
 
 
@@ -291,42 +294,42 @@
             stop=stop,
             # presence_panalty=args.presence_penalty,
             # frequency_penalty=args.frequency_penalty,
             # best_of=args.best_of,
             # logit_bias=args.logit_bias,
         )
     except openai.OpenAIError as e:
-        utils.handle_error(e)
+        utils.handle_openai_error(e)
     else:
         if num > 1:
             if no_stream:
                 for index, choice in enumerate(response["choices"]):
                     text = choice["text"]
-                    print(f"({index}) {text}")
+                    click.echo(f"({index}) {text}")
             else:
                 messages = {}
                 for chunk in response:
                     for choice in chunk["choices"]:
                         index = choice["index"]
                         if index not in messages:
                             messages[index] = ""
 
                         text = choice["text"]
                         messages[index] += text
 
                 for index, text in messages.items():
-                    print(f"({index}) {text}")
+                    click.echo(f"({index}) {text}")
         else:
             if no_stream:
                 text = response["choices"][0]["text"]
-                print(text, end="")
+                click.echo(text, nl=False)
             else:
                 for chunk in response:
                     text = chunk["choices"][0]["text"]
-                    print(text, end="")
+                    click.echo(text, nl=False)
 
 
 DEFAULT_EDIT_MODEL = CONFIG["edit"]["model"]
 DEFAULT_EDIT_TEMPERATURE = int(CONFIG["edit"]["temperature"])
 DEFAULT_EDIT_NUM = int(CONFIG["edit"]["num"])
 
 
@@ -348,15 +351,15 @@
             input=input,
             instruction=instruction,
             n=num,
             temperature=temp,
             # top_p=args.top_p,
         )
     except openai.OpenAIError as e:
-        utils.handle_error(e)
+        utils.handle_openai_error(e)
     else:
         if num > 1:
             for choice in response["choices"]:
-                print(f"({choice['index']}) {choice['text']}")
+                click.echo(f"({choice['index']}) {choice['text']}")
         else:
             text = response["choices"][0]["text"]
-            print(text)
+            click.echo(text)
```

### Comparing `skainet-0.0.0.dev8/src/skainet/utils.py` & `skainet-0.1.0/src/skainet/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,29 +16,16 @@
 def create_tempfile(ext: str) -> Path:
     temp_file = Path(tempfile.gettempdir()) / str(uuid.uuid4())
     temp_file = temp_file.with_suffix(ext)
     temp_file.touch()
     return temp_file
 
 
-def open_editor():
-    temp_file = create_tempfile(".txt")
-
-    if "EDITOR" in os.environ:
-        editor = os.environ["EDITOR"]
-    else:
-        editor = CONFIG["general"]["editor"]
-
-    subprocess.run([editor, str(temp_file)], check=True)
-
-    return temp_file.read_text()
-
-
-def handle_error(error: openai.OpenAIError):
-    print(f"{error.__class__.__name__}: {error}")
+def handle_openai_error(error: openai.OpenAIError):
+    click.echo(f"{error.__class__.__name__}: {error}", err=True)
     sys.exit(1)
 
 
 class File(click.File):
     """
     Adding extra arguments to the click.File type to support file extension validation
     """
@@ -66,10 +53,10 @@
     def convert(self, value: str, param, ctx):
         if not sys.stdin.isatty():
             if value:
                 value = value + "\n"
             value += sys.stdin.read()
 
         if not value:
-            value = open_editor()
+            value = click.edit()
 
         return value
```

