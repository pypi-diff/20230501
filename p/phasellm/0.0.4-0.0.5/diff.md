# Comparing `tmp/phasellm-0.0.4.tar.gz` & `tmp/phasellm-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phasellm-0.0.4.tar", last modified: Thu Apr 27 21:33:26 2023, max compression
+gzip compressed data, was "phasellm-0.0.5.tar", last modified: Mon May  1 21:37:59 2023, max compression
```

## Comparing `phasellm-0.0.4.tar` & `phasellm-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-27 21:33:26.816733 phasellm-0.0.4/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1083 2023-04-27 21:29:32.000000 phasellm-0.0.4/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      739 2023-04-27 21:33:26.816733 phasellm-0.0.4/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4845 2023-04-27 21:29:32.000000 phasellm-0.0.4/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-27 21:33:26.812734 phasellm-0.0.4/phasellm/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-27 21:29:32.000000 phasellm-0.0.4/phasellm/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1338 2023-04-27 21:29:41.000000 phasellm-0.0.4/phasellm/agents.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3499 2023-04-27 21:29:41.000000 phasellm-0.0.4/phasellm/eval.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2013 2023-04-27 21:29:41.000000 phasellm-0.0.4/phasellm/exceptions.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13653 2023-04-27 21:29:41.000000 phasellm-0.0.4/phasellm/llms.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-27 21:33:26.812734 phasellm-0.0.4/phasellm.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      739 2023-04-27 21:33:26.000000 phasellm-0.0.4/phasellm.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      282 2023-04-27 21:33:26.000000 phasellm-0.0.4/phasellm.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-04-27 21:33:26.000000 phasellm-0.0.4/phasellm.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      126 2023-04-27 21:33:26.000000 phasellm-0.0.4/phasellm.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2023-04-27 21:33:26.000000 phasellm-0.0.4/phasellm.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-04-27 21:33:26.816733 phasellm-0.0.4/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1167 2023-04-27 21:29:41.000000 phasellm-0.0.4/setup.py
+drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-05-01 21:37:59.684568 phasellm-0.0.5/
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     1083 2023-05-01 21:37:50.000000 phasellm-0.0.5/LICENSE
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      739 2023-05-01 21:37:59.684568 phasellm-0.0.5/PKG-INFO
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     4976 2023-05-01 21:37:50.000000 phasellm-0.0.5/README.md
+drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-05-01 21:37:59.684568 phasellm-0.0.5/phasellm/
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      653 2023-05-01 21:37:50.000000 phasellm-0.0.5/phasellm/__init__.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     5152 2023-05-01 21:37:50.000000 phasellm-0.0.5/phasellm/agents.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     3499 2023-05-01 21:37:50.000000 phasellm-0.0.5/phasellm/eval.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     2013 2023-05-01 21:37:50.000000 phasellm-0.0.5/phasellm/exceptions.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)    13653 2023-05-01 21:37:50.000000 phasellm-0.0.5/phasellm/llms.py
+drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-05-01 21:37:59.684568 phasellm-0.0.5/phasellm.egg-info/
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      739 2023-05-01 21:37:59.000000 phasellm-0.0.5/phasellm.egg-info/PKG-INFO
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      282 2023-05-01 21:37:59.000000 phasellm-0.0.5/phasellm.egg-info/SOURCES.txt
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)        1 2023-05-01 21:37:59.000000 phasellm-0.0.5/phasellm.egg-info/dependency_links.txt
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      126 2023-05-01 21:37:59.000000 phasellm-0.0.5/phasellm.egg-info/requires.txt
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)        9 2023-05-01 21:37:59.000000 phasellm-0.0.5/phasellm.egg-info/top_level.txt
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)       38 2023-05-01 21:37:59.684568 phasellm-0.0.5/setup.cfg
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     1167 2023-05-01 21:37:50.000000 phasellm-0.0.5/setup.py
```

### Comparing `phasellm-0.0.4/LICENSE` & `phasellm-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `phasellm-0.0.4/PKG-INFO` & `phasellm-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phasellm
-Version: 0.0.4
+Version: 0.0.5
 Summary: Wrappers for common large langugae models (LLMs) with support for evaluation.
 Home-page: UNKNOWN
 Author: Wojciech Gryc
 Author-email: hello@phaseai.com
 License: MIT
 Keywords: llm,nlp,evaluation,ai
 Platform: UNKNOWN
```

### Comparing `phasellm-0.0.4/README.md` & `phasellm-0.0.5/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # PhaseLLM
 
 Large language model evaluation and workflow framework from [Phase AI](https://phaseai.com/).
 
 - [Follow us on Twitter](https://twitter.com/phasellm) for updates.
 - [Star us on GitHub](https://github.com/wgryc/phasellm).
+- [Read the Docs](https://phasellm.com/docs/) -- currently limited to the module reference. Tutorials and code examples are below.
 
 ## Installation
 
 You can install PhaseLLM via pip:
 
 ```
 pip install phasellm
```

### Comparing `phasellm-0.0.4/phasellm/eval.py` & `phasellm-0.0.5/phasellm/eval.py`

 * *Files identical despite different names*

### Comparing `phasellm-0.0.4/phasellm/exceptions.py` & `phasellm-0.0.5/phasellm/exceptions.py`

 * *Files identical despite different names*

### Comparing `phasellm-0.0.4/phasellm/llms.py` & `phasellm-0.0.5/phasellm/llms.py`

 * *Files identical despite different names*

### Comparing `phasellm-0.0.4/phasellm.egg-info/PKG-INFO` & `phasellm-0.0.5/phasellm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phasellm
-Version: 0.0.4
+Version: 0.0.5
 Summary: Wrappers for common large langugae models (LLMs) with support for evaluation.
 Home-page: UNKNOWN
 Author: Wojciech Gryc
 Author-email: hello@phaseai.com
 License: MIT
 Keywords: llm,nlp,evaluation,ai
 Platform: UNKNOWN
```

### Comparing `phasellm-0.0.4/setup.py` & `phasellm-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.0.4"
+VERSION = "0.0.5"
 
 DESCRIPTION = "Wrappers for common large langugae models (LLMs) with support for evaluation."
 
 LONG_DESCRIPTION = "PhaseLLM provides wrappers for common large language models and use cases. This makes it easy to swap models in and out as needed. We also provide support for evaluation of models so you can choose which models are better to use."
 
 setup(
     name="phasellm",
```

