# Comparing `tmp/autocog-0.0.4.tar.gz` & `tmp/autocog-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autocog-0.0.4.tar", last modified: Thu Apr 20 11:14:14 2023, max compression
+gzip compressed data, was "autocog-0.0.5.tar", last modified: Mon May  1 09:58:29 2023, max compression
```

## Comparing `autocog-0.0.4.tar` & `autocog-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 andreas    (501) staff       (20)        0 2023-04-20 11:14:14.410949 autocog-0.0.4/
--rw-r--r--   0 andreas    (501) staff       (20)       24 2023-04-18 15:13:54.000000 autocog-0.0.4/.gitignore
--rw-r--r--   0 andreas    (501) staff       (20)     1312 2023-04-20 11:14:14.410757 autocog-0.0.4/PKG-INFO
--rw-r--r--   0 andreas    (501) staff       (20)     1267 2023-04-18 20:12:23.000000 autocog-0.0.4/README.md
-drwxr-xr-x   0 andreas    (501) staff       (20)        0 2023-04-20 11:14:14.375450 autocog-0.0.4/autocog/
--rw-r--r--   0 andreas    (501) staff       (20)        0 2023-04-20 11:13:20.000000 autocog-0.0.4/autocog/__init__.py
--rw-r--r--   0 andreas    (501) staff       (20)    17478 2023-04-18 20:03:31.000000 autocog-0.0.4/autocog/autocog.py
-drwxr-xr-x   0 andreas    (501) staff       (20)        0 2023-04-20 11:14:14.410535 autocog-0.0.4/autocog.egg-info/
--rw-r--r--   0 andreas    (501) staff       (20)     1312 2023-04-20 11:14:14.000000 autocog-0.0.4/autocog.egg-info/PKG-INFO
--rw-r--r--   0 andreas    (501) staff       (20)      256 2023-04-20 11:14:14.000000 autocog-0.0.4/autocog.egg-info/SOURCES.txt
--rw-r--r--   0 andreas    (501) staff       (20)        1 2023-04-20 11:14:14.000000 autocog-0.0.4/autocog.egg-info/dependency_links.txt
--rw-r--r--   0 andreas    (501) staff       (20)       52 2023-04-20 11:14:14.000000 autocog-0.0.4/autocog.egg-info/entry_points.txt
--rw-r--r--   0 andreas    (501) staff       (20)       20 2023-04-20 11:14:14.000000 autocog-0.0.4/autocog.egg-info/requires.txt
--rw-r--r--   0 andreas    (501) staff       (20)        8 2023-04-20 11:14:14.000000 autocog-0.0.4/autocog.egg-info/top_level.txt
--rw-r--r--   0 andreas    (501) staff       (20)       38 2023-04-20 11:14:14.410997 autocog-0.0.4/setup.cfg
--rw-r--r--   0 andreas    (501) staff       (20)      746 2023-04-20 11:14:09.000000 autocog-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 09:58:29.302406 autocog-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (122)     1614 2023-05-01 09:58:29.302406 autocog-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1569 2023-05-01 09:58:19.000000 autocog-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 09:58:29.302406 autocog-0.0.5/autocog/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-01 09:58:19.000000 autocog-0.0.5/autocog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20735 2023-05-01 09:58:19.000000 autocog-0.0.5/autocog/autocog.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1144 2023-05-01 09:58:19.000000 autocog-0.0.5/autocog/cache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1515 2023-05-01 09:58:19.000000 autocog-0.0.5/autocog/gpt.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 09:58:29.302406 autocog-0.0.5/autocog.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1614 2023-05-01 09:58:29.000000 autocog-0.0.5/autocog.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      277 2023-05-01 09:58:29.000000 autocog-0.0.5/autocog.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-01 09:58:29.000000 autocog-0.0.5/autocog.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       52 2023-05-01 09:58:29.000000 autocog-0.0.5/autocog.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       40 2023-05-01 09:58:29.000000 autocog-0.0.5/autocog.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        8 2023-05-01 09:58:29.000000 autocog-0.0.5/autocog.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-01 09:58:29.302406 autocog-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      788 2023-05-01 09:58:19.000000 autocog-0.0.5/setup.py
```

### Comparing `autocog-0.0.4/PKG-INFO` & `autocog-0.0.5/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autocog
-Version: 0.0.4
+Version: 0.0.5
 Home-page: https://github.com/andreasjansson/AutoCog
 Description-Content-Type: text/markdown
 
 # AutoCog
 
 [![PyPI version](https://badge.fury.io/py/autocog.svg)](https://badge.fury.io/py/autocog)
 
@@ -35,14 +35,16 @@
 
 If your model needs a GPU to run, you need to run AutoCog on a GPU machine.
 
 ### Human in the loop
 
 Sometimes AutoCog fails to create a working Cog configuration. In those cases you, the human, have to step in and edit the cog.yaml and predict.py files.
 
-Once you have edited them, let AutoCog continue:
+Once you have edited them, let AutoCog continue by running `autocog` again. If you'd like to recreate `predict.py` and `cog.yaml` from scratch, run `autocog --initialize`.
+
+By default, AutoCog will guess a `cog predict` command to run the model. If you want to specify your own predict command, use the `--predict-command` flag.
+
+If you want AutoCog to take the generation of `cog.yaml` and `predict.py` in a specific direction, you can use the `--tell` flag to prompt GPT4:
 
 ```
-autocog --continue
+autocog --tell="Add inputs to allow for inpainting"
 ```
-
-By default, AutoCog will guess a `cog predict` command to run the model. If you want to specify your own predict command, use the `--predict-command` flag.
```

### Comparing `autocog-0.0.4/README.md` & `autocog-0.0.5/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -30,14 +30,16 @@
 
 If your model needs a GPU to run, you need to run AutoCog on a GPU machine.
 
 ### Human in the loop
 
 Sometimes AutoCog fails to create a working Cog configuration. In those cases you, the human, have to step in and edit the cog.yaml and predict.py files.
 
-Once you have edited them, let AutoCog continue:
+Once you have edited them, let AutoCog continue by running `autocog` again. If you'd like to recreate `predict.py` and `cog.yaml` from scratch, run `autocog --initialize`.
+
+By default, AutoCog will guess a `cog predict` command to run the model. If you want to specify your own predict command, use the `--predict-command` flag.
+
+If you want AutoCog to take the generation of `cog.yaml` and `predict.py` in a specific direction, you can use the `--tell` flag to prompt GPT4:
 
 ```
-autocog --continue
+autocog --tell="Add inputs to allow for inpainting"
 ```
-
-By default, AutoCog will guess a `cog predict` command to run the model. If you want to specify your own predict command, use the `--predict-command` flag.
```

### Comparing `autocog-0.0.4/autocog/autocog.py` & `autocog-0.0.5/autocog/autocog.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,24 @@
+import time
 from collections import deque
 import sys
-from PIL import Image
 import wave
+import array
 import re
 import click
 import os
 import subprocess
-import openai
 import tempfile
-import glob
+
+from PIL import Image
+from pydub import AudioSegment
+import cv2
+
+from .cache import cached, purge_cache
+from .gpt import call_gpt, MaxTokensExceeded, set_openai_api_key
 
 
 def file_start(filename):
     return f"-- FILE_START: {filename}"
 
 
 def file_end(filename):
@@ -43,15 +49,14 @@
     ) -> Path:
         """Run a single prediction on the model"""
         processed_image = preprocess(image)
         output = self.model(processed_image)
         return postprocess(output)
 '''
 
-SYSTEM_PROMPT = "You are an expert Python machine learning developer."
 COG_PROMPT = f"""
 Below is an example of a cog.yaml file and a predict.py file.
 
 {file_start("cog.yaml")}
 {COG_YAML_EXAMPLE}
 {file_end("cog.yaml")}
 
@@ -61,15 +66,15 @@
 """
 
 
 def cog_predict_prompt(predict_contents):
     return f"""
 Below is an example of a cog predict command:
 
-cog predict -i @input.jpg
+cog predict -i input1=@input.jpg -i input2=foo
 
 Return a cog predict command for the following predict.py file (and return only the prompt, no other text):
 
 ```
 {predict_contents}
 ```
 """
@@ -146,15 +151,15 @@
 """
 
 
 def order_paths_prompt(paths, readme_contents):
     paths_list = "\n".join(paths)
 
     prompt = f"""
-Given the file paths and readme below, order them by how relevant they are for inference and in particular for building a Replicate prediction model with Cog. Return the ordered file paths in the following format (and make sure to not include anything else than the list of file paths):
+Given the file paths and readme below, order them by how relevant they are for inference and in particular for building a Replicate prediction model with Cog. Return the ordered file paths (a maximum of 25 paths) in the following format (and make sure to not include anything else than the list of file paths):
 
 most_relevant.py
 second_most_relevant.py
 third_most_relevant.py
 [...]
 least_relevant.py
 
@@ -165,49 +170,73 @@
 End of paths. Below is the readme:
 
 {readme_contents}
 """
     return prompt
 
 
-def order_paths(repo_path, *, attempt=0):
-    paths = find_python_files(repo_path)
+def truncate_error(error):
+    return error[int(len(error) * 0.4) :]
+
+
+@cached("paths.pkl")
+def order_paths(repo_path, *, attempt=0, readme_contents=None):
+    paths = find_python_files(repo_path, relative=True)
     if len(paths) == 0:
         raise ValueError(f"{repo_path} has no Python files")
 
     print("Ordering files based on importance...", file=sys.stderr)
 
-    readme_contents = ""
-    readme_path = os.path.join(repo_path, "README.md")
-    if os.path.exists(readme_path):
-        with open(readme_path) as f:
-            readme_contents = f.read()
+    if readme_contents is None:
+        readme_contents = ""
+        readme_path = os.path.join(repo_path, "README.md")
+        if os.path.exists(readme_path):
+            with open(readme_path) as f:
+                readme_contents = f.read()
+
+    try:
+        content = call_gpt(order_paths_prompt(paths, readme_contents))
+    except MaxTokensExceeded:
+        if attempt == 5:
+            raise
+
+        return order_paths(
+            repo_path, attempt=attempt + 1, readme_contents=readme_contents[:-1000]
+        )
 
-    content = call_gpt(order_paths_prompt(paths, readme_contents))
     ordered_paths = content.strip().splitlines()
-    if set(paths) != set(ordered_paths):
+    if set(ordered_paths) - set(paths):
         if attempt == 5:
             raise ValueError("Failed to order paths")
         return order_paths(repo_path, attempt=attempt + 1)
+
+    for i, path in enumerate(ordered_paths):
+        ordered_paths[i] = os.path.join(repo_path, path)
+
     return ordered_paths
 
 
-def files_prompt(repo_path, paths, max_length):
+def files_prompt(repo_path, paths, tell, max_length):
     prompt = f"""
 Given the files below, generate a predict.py and cog.yaml file. In cog.yaml, ensure that all Python packages must have pinned versions. Also in cog.yaml, add short comments to describe what parts of the code made you decide on the different parts of cog.yaml. Wrap the contents of both files in the strings '{file_start("<filename>")}' and '{file_end("<filename>")}'. Don't output any other text before or after the files.
 
 """
+    if tell:
+        prompt += tell + "\n\n"
+
     readme_path = os.path.join(repo_path, "README.md")
     if os.path.exists(readme_path):
         paths.insert(0, readme_path)
     requirements_path = os.path.join(repo_path, "requirements.txt")
     if os.path.exists(requirements_path):
         paths.insert(0, requirements_path)
 
     for path in paths:
+        if not os.path.exists(path):
+            continue
         with open(path, "r") as f:
             filename = os.path.relpath(path, repo_path)
             contents = f.read()
             is_truncated = False
             if len(prompt + contents) > max_length:
                 contents = contents[: max_length - len(prompt)]
                 is_truncated = True
@@ -217,44 +246,43 @@
             )
             if is_truncated:
                 return prompt
 
     return prompt
 
 
-def generate_files(repo_path, paths, *, attempt=0):
+def generate_files(repo_path, paths, tell, *, attempt=0):
     max_lengths = [25000, 20000, 15000, 10000]
 
     try:
         content = call_gpt(
             [
                 {"role": "user", "content": COG_PROMPT},
                 {"role": "assistant", "content": "Okay."},
                 {
                     "role": "user",
                     "content": files_prompt(
-                        repo_path, paths, max_length=max_lengths[attempt]
+                        repo_path, paths, tell, max_length=max_lengths[attempt]
                     ),
                 },
             ]
         )
-    except openai.error.InvalidRequestError as e:
-        if "context length" in str(e):
-            if attempt == len(max_lengths):
-                raise
-            return generate_files(repo_path, paths, attempt=attempt + 1)
+    except MaxTokensExceeded:
+        if attempt == len(max_lengths):
+            raise
+        return generate_files(repo_path, paths, tell, attempt=attempt + 1)
 
     if file_end("cog.yaml") not in content or file_end("predict.py") not in content:
         if attempt == len(max_lengths):
             raise ValueError("Failed to generate a predict.py file")
         print(
             f"Failed to complete the output, trying again (attempt {attempt + 1}/{len(max_lengths)})",
             file=sys.stderr,
         )
-        generate_files(repo_path, paths, attempt=attempt + 1)
+        generate_files(repo_path, paths, tell, attempt=attempt + 1)
 
     files = {
         "cog.yaml": file_from_gpt_response(content, "cog.yaml"),
         "predict.py": file_from_gpt_response(content, "predict.py"),
     }
 
     return files
@@ -279,48 +307,14 @@
                 python_files.append(path_to_return)
             elif os.path.isdir(full_entry_path):
                 queue.append(path_to_return)
 
     return python_files
 
 
-def call_gpt(messages, *, temperature=0.5):
-    if type(messages) == str:
-        messages = [{"role": "user", "content": messages}]
-
-    response = openai.ChatCompletion.create(
-        model="gpt-4",  # gpt-4-32k
-        messages=[
-            {
-                "role": "system",
-                "content": SYSTEM_PROMPT,
-            },
-        ]
-        + messages,
-        n=1,
-        stop=None,
-        temperature=temperature,
-        stream=True,
-    )
-    text = ""
-    for chunk in response:
-        if not chunk:
-            continue
-        chunk_text = chunk["choices"][0]["delta"].get("content", None)
-        if chunk_text == None:
-            continue
-        text += chunk_text
-        sys.stderr.write(chunk_text)
-        sys.stderr.flush()
-
-    sys.stderr.write("\n")
-
-    return text
-
-
 def generate_predict_command(predict_contents):
     return call_gpt(cog_predict_prompt(predict_contents))
 
 
 def file_from_gpt_response(content, filename):
     pattern = re.compile(
         rf"(?<={file_start(filename)})(?:\n```[a-z]*\n)?(.*?)(?:\n```\n)?(?={file_end(filename)})",
@@ -347,14 +341,18 @@
     )
     stderr = ""
     for line in proc.stderr:
         line = line.decode()
         sys.stderr.write(line)
         stderr += line
 
+        if "Model setup failed" in line:
+            proc.kill()
+            break
+
     proc.wait()
     # cog predict will return 0 if the model fails internally
     if proc.returncode == 0 and "Traceback (most recent call last)" not in stderr:
         return True, stderr
 
     return False, stderr
 
@@ -379,28 +377,38 @@
         img.save(filename, format="JPEG")
     elif file_type == "png":
         img = Image.new("RGBA", (256, 256), color=(0, 0, 0, 0))
         img.save(filename, format="PNG")
     elif file_type == "wav":
         with wave.open(filename, "wb") as wav_file:
             wav_file.setparams((1, 2, 44100, 0, "NONE", "not compressed"))
-            data = np.zeros((44100, 2))
-            wav_file.writeframes(data.astype(np.int16).tobytes())
+            data = array.array("h", [0] * 44100 * 2)  # 'h' is for signed short integers
+            wav_file.writeframes(data.tobytes())
     elif file_type == "mp3":
-        with open(filename, "wb") as mp3_file:
-            pass
+        silence = AudioSegment.silent(duration=1000)  # duration in milliseconds
+        silence.export(filename, format="mp3")
     elif file_type == "txt":
         with open(filename, "w") as txt_file:
-            pass
+            txt_file.write("   ")
     elif file_type == "mp4":
-        with open(filename, "wb") as mp4_file:
-            pass
+        height, width = 640, 480
+        fourcc = cv2.VideoWriter_fourcc(*"mp4v")
+        video = cv2.VideoWriter(filename, fourcc, 1, (width, height))
+        frame = np.zeros((height, width, 3), dtype=np.uint8)
+        for _ in range(30):
+            video.write(frame)
+        video.release()
     elif file_type == "avi":
-        with open(filename, "wb") as avi_file:
-            pass
+        height, width = 640, 480
+        fourcc = cv2.VideoWriter_fourcc(*"XVID")
+        video = cv2.VideoWriter(filename, fourcc, 1, (width, height))
+        frame = np.zeros((height, width, 3), dtype=np.uint8)
+        for _ in range(30):
+            video.write(frame)
+        video.release()
     else:
         raise ValueError("Unsupported file type")
 
 
 def parse_cog_predict_error(stderr, *, max_length=20000):
     if "Running prediction...\n" in stderr:
         error = stderr.split("Running prediction...\n")[1].split("panic: ")[0]
@@ -409,49 +417,90 @@
 
     return error[-max_length:]
 
 
 def diagnose_error(predict_contents, predict_command, error, *, attempt=0):
     print("Diagnosing source of error: ", file=sys.stderr)
 
-    text = call_gpt(diagnose_error_prompt(predict_contents, predict_command, error))
+    try:
+        text = call_gpt(diagnose_error_prompt(predict_contents, predict_command, error))
+    except MaxTokensExceeded:
+        if attempt == 5:
+            raise
+
+        return diagnose_error(
+            predict_contents,
+            predict_command,
+            truncate_error(error),
+            attempt=attempt + 1,
+        )
     if text not in [ERROR_PREDICT_PY, ERROR_COG_PREDICT, ERROR_COG_YAML]:
-        if attempt == 3:
+        if attempt == 5:
             raise ValueError("Failed to diagnose error")
         return diagnose_error(
             predict_contents, predict_command, error, attempt=attempt + 1
         )
     return text
 
 
 def fix_predict_py(predict_contents, error, repo_path, *, attempt=0):
-    text = call_gpt(fix_predict_py_prompt(predict_contents, error, repo_path))
+    try:
+        text = call_gpt(fix_predict_py_prompt(predict_contents, error, repo_path))
+    except MaxTokensExceeded:
+        if attempt == 5:
+            raise
+        return fix_predict_py(
+            predict_contents, truncate_error(error), repo_path, attempt=attempt + 1
+        )
+
     pattern = re.compile(
         rf"(?:\n```[a-z]*\n)?(.*)(?:\n```)?",
         re.MULTILINE | re.DOTALL,
     )
     diff = pattern.search(text)[1]
     try:
         return patch(predict_contents, diff)
     except:
-        if attempt == 3:
+        if attempt == 5:
             raise ValueError("Failed to generate patch")
-        return fix_predict_py(predict_contents, error, repo_path, attempt=attempt + 1)
+        return fix_predict_py(
+            predict_contents, truncate_error(error), repo_path, attempt=attempt + 1
+        )
 
 
 def fix_cog_yaml(cog_yaml_contents, predict_contents, error, *, attempt=0):
-    for local_attempt in range(3):
+    if attempt == 5:
+        raise ValueError("Failed to get cog.yaml fix")
+
+    try:
         text = call_gpt(
             fix_cog_yaml_prompt(cog_yaml_contents, predict_contents, error),
             temperature=0.5 + attempt / 5,
         )
-        contents = file_from_gpt_response(text, "cog.yaml")
-        if contents:
-            return contents
-    raise ValueError("Failed to get cog.yaml fix")
+    except MaxTokensExceeded:
+        if attempt == 5:
+            raise
+
+        return fix_cog_yaml(
+            cog_yaml_contents,
+            predict_contents,
+            truncate_error(error),
+            attempt=attempt + 1,
+        )
+
+    contents = file_from_gpt_response(text, "cog.yaml")
+    if contents:
+        return contents
+
+    return fix_cog_yaml(
+        cog_yaml_contents,
+        predict_contents,
+        error,
+        attempt=attempt + 1,
+    )
 
 
 def patch(contents, diff):
     with tempfile.NamedTemporaryFile(delete=False) as tmp_original:
         tmp_original.write(contents.encode())
         tmp_original.flush()
 
@@ -470,61 +519,127 @@
     # Clean up the temporary files
     os.unlink(tmp_original.name)
     os.unlink(tmp_patch.name)
 
     return patched_contents
 
 
+def is_initialized(repo_path):
+    return os.path.exists(os.path.join(repo_path, "cog.yaml")) and os.path.exists(
+        os.path.join(repo_path, "predict.py")
+    )
+
+
+def initialize_project(repo_path):
+    cog_yaml_path = os.path.join(repo_path, "cog.yaml")
+    predict_py_path = os.path.join(repo_path, "predict.py")
+    if os.path.exists(cog_yaml_path):
+        os.remove(cog_yaml_path)
+    if os.path.exists(predict_py_path):
+        os.remove(predict_py_path)
+    purge_cache(repo_path)
+
+
+def read_file(path):
+    with open(path, "r") as file:
+        content = file.read()
+    return content
+
+
 @click.command()
 @click.option(
     "-r",
     "--repo",
     default="",
     help="Path to the ML repository (default is current directory)",
 )
 @click.option(
     "-k",
     "--openai-api-key",
     default=os.environ.get("OPENAI_API_KEY", ""),
-    help="OpenAI API token (optional, defaults to the environment variable OPENAI_API_KEY)",
+    help="OpenAI API key (optional, defaults to the environment variable OPENAI_API_KEY)",
 )
 @click.option(
     "-n",
     "--attempts",
     default=5,
     type=int,
     help="Number of attempts to try to fix issues before giving up",
 )
 @click.option(
     "-p",
     "--predict-command",
     help="Initial predict command. If not specified, AutoCog will generate one",
 )
 @click.option(
+    "-t",
+    "--tell",
+    help="Tell AutoCog to ",
+)
+@click.option(
+    "-i",
+    "--initialize",
+    help="Initialize project by removing any existing predict.py and cog.yaml files. If omitted, AutoCog will continue from the current state of the repository",
+    is_flag=True,
+)
+@click.option(
     "-c",
     "--continue",
     "continue_from_existing",
     is_flag=True,
-    help="Continue to try to fix an existing predict.py and cog.yaml instead of generating them from scratch. AutoCog isn't perfect and having a human in the loop is often necessary.",
+    hidden=True,
 )
 def autocog(
-    repo, openai_api_key, attempts, predict_command, continue_from_existing
+    repo,
+    openai_api_key,
+    attempts,
+    predict_command,
+    tell,
+    initialize,
+    continue_from_existing,
 ):
-    openai.api_key = openai_api_key
+    if not openai_api_key:
+        print(
+            "OpenAI API key was not specified. Either set the OPENAI_API_KEY environment variable or pass it to autocog with the -k/--openai-api-key parameter.",
+            file=sys.stderr,
+        )
+        sys.exit(1)
+
+    set_openai_api_key(openai_api_key)
 
     repo_path = repo or os.getcwd()
 
     if continue_from_existing:
-        files = {}
-        for filename in ["cog.yaml", "predict.py"]:
-            with open(os.path.join(repo_path, filename)) as f:
-                files[filename] = f.read()
+        print(
+            "The -c/--continue argument has been deprecated and is now a no-op. If you don't specify the --initialize flag, autocog will continue from the current state of the repository",
+            file=sys.stderr,
+        )
+
+    if initialize:
+        initialize_project(repo_path)
+
+    if is_initialized(repo_path) and not tell:
+        files = {
+            "cog.yaml": read_file("cog.yaml"),
+            "predict.py": read_file("predict.py"),
+        }
+    elif tell:
+        paths = order_paths(repo_path)
+        cog_yaml_path = os.path.join(repo_path, "cog.yaml")
+        predict_py_path = os.path.join(repo_path, "predict.py")
+        paths.insert(0, cog_yaml_path)
+        if predict_py_path in paths:
+            paths.remove(predict_py_path)
+        paths.insert(0, predict_py_path)
+        tell = "Make sure to follow these instructions: " + tell
+        files = generate_files(repo_path, paths, tell=tell)
+        write_files(repo_path, files)
     else:
         paths = order_paths(repo_path)
-        files = generate_files(repo_path, paths)
+        files = generate_files(repo_path, paths, tell=None)
         write_files(repo_path, files)
 
     if not predict_command:
         predict_command = generate_predict_command(files["predict.py"])
     predict_command = create_files_for_predict_command(predict_command, repo_path)
     for attempt in range(attempts):
         success, stderr = run_cog_predict(predict_command, repo_path)
@@ -543,17 +658,19 @@
         error = parse_cog_predict_error(stderr)
         error_source = diagnose_error(files["predict.py"], predict_command, error)
         if error_source == ERROR_PREDICT_PY:
             files["predict.py"] = fix_predict_py(files["predict.py"], error, repo_path)
             write_files(repo_path, files)
         elif error_source == ERROR_COG_YAML:
             files["cog.yaml"] = fix_cog_yaml(
-                files["cog.yaml"], files["predict.py"], error, attempt=attempt
+                files["cog.yaml"], files["predict.py"], error
             )
             write_files(repo_path, files)
         elif error_source == ERROR_COG_PREDICT:
             predict_command = generate_predict_command(files["predict.py"])
-            predict_command = create_files_for_predict_command(predict_command, repo_path)
+            predict_command = create_files_for_predict_command(
+                predict_command, repo_path
+            )
 
 
 if __name__ == "__main__":
     autocog()
```

### Comparing `autocog-0.0.4/autocog.egg-info/PKG-INFO` & `autocog-0.0.5/autocog.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autocog
-Version: 0.0.4
+Version: 0.0.5
 Home-page: https://github.com/andreasjansson/AutoCog
 Description-Content-Type: text/markdown
 
 # AutoCog
 
 [![PyPI version](https://badge.fury.io/py/autocog.svg)](https://badge.fury.io/py/autocog)
 
@@ -35,14 +35,16 @@
 
 If your model needs a GPU to run, you need to run AutoCog on a GPU machine.
 
 ### Human in the loop
 
 Sometimes AutoCog fails to create a working Cog configuration. In those cases you, the human, have to step in and edit the cog.yaml and predict.py files.
 
-Once you have edited them, let AutoCog continue:
+Once you have edited them, let AutoCog continue by running `autocog` again. If you'd like to recreate `predict.py` and `cog.yaml` from scratch, run `autocog --initialize`.
+
+By default, AutoCog will guess a `cog predict` command to run the model. If you want to specify your own predict command, use the `--predict-command` flag.
+
+If you want AutoCog to take the generation of `cog.yaml` and `predict.py` in a specific direction, you can use the `--tell` flag to prompt GPT4:
 
 ```
-autocog --continue
+autocog --tell="Add inputs to allow for inpainting"
 ```
-
-By default, AutoCog will guess a `cog predict` command to run the model. If you want to specify your own predict command, use the `--predict-command` flag.
```

### Comparing `autocog-0.0.4/setup.py` & `autocog-0.0.5/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,21 +5,23 @@
 long_description = (this_directory / "README.md").read_text()
 long_description = long_description.replace("![Screen recording](https://github.com/andreasjansson/AutoCog/raw/main/assets/screen-recording.gif)\n", "")
 
 setup(
     name="autocog",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    version="0.0.4",
+    version="0.0.5",
     url="https://github.com/andreasjansson/AutoCog",
     packages=find_packages(),
     install_requires=[
         "openai",
         "click",
         "Pillow",
+        "pydub",
+        "opencv-python",
     ],
     entry_points={
         "console_scripts": [
             "autocog = autocog.autocog:autocog",
         ],
     },
 )
```

