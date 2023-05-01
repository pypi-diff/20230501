# Comparing `tmp/sorampt-0.1.5.tar.gz` & `tmp/sorampt-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sorampt-0.1.5.tar", max compression
+gzip compressed data, was "sorampt-0.1.6.tar", max compression
```

## Comparing `sorampt-0.1.5.tar` & `sorampt-0.1.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1061 2023-05-01 05:22:37.622435 sorampt-0.1.5/LICENSE
--rw-r--r--   0        0        0     2256 2023-05-01 05:22:37.622435 sorampt-0.1.5/README.md
--rw-r--r--   0        0        0     1050 2023-05-01 05:22:37.622435 sorampt-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      338 2023-05-01 05:22:37.622435 sorampt-0.1.5/sorampt/__init__.py
--rw-r--r--   0        0        0       68 2023-05-01 05:22:37.622435 sorampt-0.1.5/sorampt/__main__.py
--rw-r--r--   0        0        0      618 2023-05-01 05:22:37.622435 sorampt-0.1.5/sorampt/cli/__init__.py
--rw-r--r--   0        0        0     2851 2023-05-01 05:22:37.622435 sorampt-0.1.5/sorampt/cli/_options.py
--rw-r--r--   0        0        0     2865 2023-05-01 05:22:37.622435 sorampt-0.1.5/sorampt/cli/checkbox.py
--rw-r--r--   0        0        0     1605 2023-05-01 05:22:37.622435 sorampt-0.1.5/sorampt/cli/confirm.py
--rw-r--r--   0        0        0     1518 2023-05-01 05:22:37.622435 sorampt-0.1.5/sorampt/cli/input.py
--rw-r--r--   0        0        0     2454 2023-05-01 05:22:37.622435 sorampt-0.1.5/sorampt/cli/list.py
--rw-r--r--   0        0        0      330 2023-05-01 05:22:37.622435 sorampt-0.1.5/sorampt/prompts/__init__.py
--rw-r--r--   0        0        0     3354 2023-05-01 05:22:37.622435 sorampt-0.1.5/sorampt/prompts/_base.py
--rw-r--r--   0        0        0      230 2023-05-01 05:22:37.622435 sorampt-0.1.5/sorampt/prompts/_choice.py
--rw-r--r--   0        0        0    11809 2023-05-01 05:22:37.622435 sorampt-0.1.5/sorampt/prompts/checkbox.py
--rw-r--r--   0        0        0     4067 2023-05-01 05:22:37.622435 sorampt-0.1.5/sorampt/prompts/confirm.py
--rw-r--r--   0        0        0     5736 2023-05-01 05:22:37.622435 sorampt-0.1.5/sorampt/prompts/input.py
--rw-r--r--   0        0        0    11869 2023-05-01 05:22:37.622435 sorampt-0.1.5/sorampt/prompts/list.py
--rw-r--r--   0        0        0        0 2023-05-01 05:22:37.622435 sorampt-0.1.5/sorampt/py.typed
--rw-r--r--   0        0        0      437 2023-05-01 05:22:37.622435 sorampt-0.1.5/sorampt/utils.py
--rw-r--r--   0        0        0     2953 1970-01-01 00:00:00.000000 sorampt-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-05-01 05:45:17.912732 sorampt-0.1.6/LICENSE
+-rw-r--r--   0        0        0     2256 2023-05-01 05:45:17.912732 sorampt-0.1.6/README.md
+-rw-r--r--   0        0        0     1050 2023-05-01 05:45:17.912732 sorampt-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      338 2023-05-01 05:45:17.912732 sorampt-0.1.6/sorampt/__init__.py
+-rw-r--r--   0        0        0       68 2023-05-01 05:45:17.912732 sorampt-0.1.6/sorampt/__main__.py
+-rw-r--r--   0        0        0      618 2023-05-01 05:45:17.912732 sorampt-0.1.6/sorampt/cli/__init__.py
+-rw-r--r--   0        0        0     2851 2023-05-01 05:45:17.912732 sorampt-0.1.6/sorampt/cli/_options.py
+-rw-r--r--   0        0        0     2865 2023-05-01 05:45:17.912732 sorampt-0.1.6/sorampt/cli/checkbox.py
+-rw-r--r--   0        0        0     1605 2023-05-01 05:45:17.912732 sorampt-0.1.6/sorampt/cli/confirm.py
+-rw-r--r--   0        0        0     1518 2023-05-01 05:45:17.912732 sorampt-0.1.6/sorampt/cli/input.py
+-rw-r--r--   0        0        0     2454 2023-05-01 05:45:17.912732 sorampt-0.1.6/sorampt/cli/list.py
+-rw-r--r--   0        0        0      330 2023-05-01 05:45:17.912732 sorampt-0.1.6/sorampt/prompts/__init__.py
+-rw-r--r--   0        0        0     3354 2023-05-01 05:45:17.916732 sorampt-0.1.6/sorampt/prompts/_base.py
+-rw-r--r--   0        0        0      230 2023-05-01 05:45:17.916732 sorampt-0.1.6/sorampt/prompts/_choice.py
+-rw-r--r--   0        0        0    11809 2023-05-01 05:45:17.916732 sorampt-0.1.6/sorampt/prompts/checkbox.py
+-rw-r--r--   0        0        0     4067 2023-05-01 05:45:17.916732 sorampt-0.1.6/sorampt/prompts/confirm.py
+-rw-r--r--   0        0        0     5736 2023-05-01 05:45:17.916732 sorampt-0.1.6/sorampt/prompts/input.py
+-rw-r--r--   0        0        0    11869 2023-05-01 05:45:17.916732 sorampt-0.1.6/sorampt/prompts/list.py
+-rw-r--r--   0        0        0        0 2023-05-01 05:45:17.916732 sorampt-0.1.6/sorampt/py.typed
+-rw-r--r--   0        0        0      437 2023-05-01 05:45:17.916732 sorampt-0.1.6/sorampt/utils.py
+-rw-r--r--   0        0        0     2953 1970-01-01 00:00:00.000000 sorampt-0.1.6/PKG-INFO
```

### Comparing `sorampt-0.1.5/LICENSE` & `sorampt-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `sorampt-0.1.5/README.md` & `sorampt-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `sorampt-0.1.5/pyproject.toml` & `sorampt-0.1.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sorampt"
-version = "0.1.5"
+version = "0.1.6"
 description = "用于控制台交互的提示工具包"
 authors = ["mute231010 <mute231010@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/netsora/sorampt"
 repository = "https://github.com/netsora/sorampt"
 documentation = "https://github.com/netsora/sorampt"
```

### Comparing `sorampt-0.1.5/sorampt/cli/__init__.py` & `sorampt-0.1.6/sorampt/cli/__init__.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-from . import list, input, confirm, checkbox
 from typing import Dict, Callable
 from argparse import ArgumentParser
 
 parser = ArgumentParser(prog="sorampt", description="A simple prompt toolkit.")
 parser.add_argument(
     "--no-ansi", action="store_true", required=False, help="disable ANSI colors"
 )
 parser.add_argument(
     "-d", "--default", required=False, help="default answer when cancelled"
 )
 
 subparsers = parser.add_subparsers(title="prompt type", required=True)
 
+from . import list, input, confirm, checkbox
 
 def main():
     result = parser.parse_args()
     result = vars(result)
     prompt: Callable[..., None] = result.pop("func")
     prompt(**result)
```

### Comparing `sorampt-0.1.5/sorampt/cli/_options.py` & `sorampt-0.1.6/sorampt/cli/_options.py`

 * *Files identical despite different names*

### Comparing `sorampt-0.1.5/sorampt/cli/checkbox.py` & `sorampt-0.1.6/sorampt/cli/checkbox.py`

 * *Files identical despite different names*

### Comparing `sorampt-0.1.5/sorampt/cli/confirm.py` & `sorampt-0.1.6/sorampt/cli/confirm.py`

 * *Files identical despite different names*

### Comparing `sorampt-0.1.5/sorampt/cli/input.py` & `sorampt-0.1.6/sorampt/cli/input.py`

 * *Files identical despite different names*

### Comparing `sorampt-0.1.5/sorampt/cli/list.py` & `sorampt-0.1.6/sorampt/cli/list.py`

 * *Files identical despite different names*

### Comparing `sorampt-0.1.5/sorampt/prompts/_base.py` & `sorampt-0.1.6/sorampt/prompts/_base.py`

 * *Files identical despite different names*

### Comparing `sorampt-0.1.5/sorampt/prompts/checkbox.py` & `sorampt-0.1.6/sorampt/prompts/checkbox.py`

 * *Files identical despite different names*

### Comparing `sorampt-0.1.5/sorampt/prompts/confirm.py` & `sorampt-0.1.6/sorampt/prompts/confirm.py`

 * *Files identical despite different names*

### Comparing `sorampt-0.1.5/sorampt/prompts/input.py` & `sorampt-0.1.6/sorampt/prompts/input.py`

 * *Files identical despite different names*

### Comparing `sorampt-0.1.5/sorampt/prompts/list.py` & `sorampt-0.1.6/sorampt/prompts/list.py`

 * *Files identical despite different names*

### Comparing `sorampt-0.1.5/PKG-INFO` & `sorampt-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sorampt
-Version: 0.1.5
+Version: 0.1.6
 Summary: 用于控制台交互的提示工具包
 Home-page: https://github.com/netsora/sorampt
 License: MIT
 Keywords: prompt,inquirer,prompt-toolkit
 Author: mute231010
 Author-email: mute231010@gmail.com
 Requires-Python: >=3.10,<4.0
```

