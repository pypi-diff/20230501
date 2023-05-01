# Comparing `tmp/jsonformer-0.4.0.tar.gz` & `tmp/jsonformer-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsonformer-0.4.0.tar", max compression
+gzip compressed data, was "jsonformer-0.5.0.tar", max compression
```

## Comparing `jsonformer-0.4.0.tar` & `jsonformer-0.5.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     2631 2023-05-01 19:27:44.428173 jsonformer-0.4.0/README.md
--rw-r--r--   0        0        0       38 2023-05-01 18:49:54.058145 jsonformer-0.4.0/jsonformer/__init__.py
--rw-r--r--   0        0        0     1049 2023-05-01 17:24:41.244922 jsonformer-0.4.0/jsonformer/example.py
--rw-r--r--   0        0        0      995 2023-05-01 17:24:41.244984 jsonformer-0.4.0/jsonformer/format.py
--rw-r--r--   0        0        0     1984 2023-05-01 17:24:41.245061 jsonformer-0.4.0/jsonformer/logits_processors.py
--rw-r--r--   0        0        0     6745 2023-05-01 18:48:35.415292 jsonformer-0.4.0/jsonformer/main.py
--rw-r--r--   0        0        0      501 2023-05-01 20:31:01.717211 jsonformer-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     3286 1970-01-01 00:00:00.000000 jsonformer-0.4.0/setup.py
--rw-r--r--   0        0        0     3003 1970-01-01 00:00:00.000000 jsonformer-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     2631 2023-05-01 19:27:44.428173 jsonformer-0.5.0/README.md
+-rw-r--r--   0        0        0       85 2023-05-01 21:32:30.326739 jsonformer-0.5.0/jsonformer/__init__.py
+-rw-r--r--   0        0        0     1037 2023-05-01 21:30:35.817333 jsonformer-0.5.0/jsonformer/example.py
+-rw-r--r--   0        0        0      995 2023-05-01 17:24:41.244984 jsonformer-0.5.0/jsonformer/format.py
+-rw-r--r--   0        0        0     1984 2023-05-01 17:24:41.245061 jsonformer-0.5.0/jsonformer/logits_processors.py
+-rw-r--r--   0        0        0     6745 2023-05-01 18:48:35.415292 jsonformer-0.5.0/jsonformer/main.py
+-rw-r--r--   0        0        0      498 2023-05-01 21:32:39.450479 jsonformer-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     3286 1970-01-01 00:00:00.000000 jsonformer-0.5.0/setup.py
+-rw-r--r--   0        0        0     3003 1970-01-01 00:00:00.000000 jsonformer-0.5.0/PKG-INFO
```

### Comparing `jsonformer-0.4.0/README.md` & `jsonformer-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `jsonformer-0.4.0/jsonformer/example.py` & `jsonformer-0.5.0/jsonformer/example.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from jsonformer.format import highlight_values
 from jsonformer.main import Jsonformer
 from transformers import (
     AutoModelForCausalLM,
     AutoTokenizer,
 )
-import torch
+
 
 
 weather_schema = {
     "type": "object",
     "properties": {
         "temperature": {"type": "number"},
         "humidity": {
```

### Comparing `jsonformer-0.4.0/jsonformer/format.py` & `jsonformer-0.5.0/jsonformer/format.py`

 * *Files identical despite different names*

### Comparing `jsonformer-0.4.0/jsonformer/logits_processors.py` & `jsonformer-0.5.0/jsonformer/logits_processors.py`

 * *Files identical despite different names*

### Comparing `jsonformer-0.4.0/jsonformer/main.py` & `jsonformer-0.5.0/jsonformer/main.py`

 * *Files identical despite different names*

### Comparing `jsonformer-0.4.0/setup.py` & `jsonformer-0.5.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['termcolor>=2.3.0,<3.0.0']
 
 setup_kwargs = {
     'name': 'jsonformer',
-    'version': '0.4.0',
+    'version': '0.5.0',
     'description': '',
     'long_description': '# Jsonformer: A Bulletproof Way to Generate Structured JSON from Language Models.\n\n### Problem: Getting models to output structed JSON is hard\n\n### Solution: Only generate the content tokens and fill in the fixed tokens\n\n![cover](img/cover4.png)\n\nGenerating structured JSON from language models is a challenging task. The\ngenerated JSON must be syntactically correct, and it must conform to a schema\nthat specifies the structure of the JSON.\n\nCurrent approaches to this problem are brittle and error-prone. They rely on prompt engineering, fine-tuning, and post-processing, but they still fail to generate syntactically correct JSON in many cases.\n\nJsonformer is a new approach to this problem. In structured data, many tokens are fixed and predictable. Jsonformer is a wrapper around HuggingFace models that fills in the fixed tokens during the generation process, and only delegates the generation of content tokens to the language model. This makes it more efficient and bulletproof than existing approaches.\n\nThis currently supports a subset of JSON Schema. Below is a list of the supported schema types:\n\n- number\n- boolean\n- string\n- array\n- object\n\n## Example\n\n```python\nfrom transformers import AutoModelForCausalLM, AutoTokenizer\n\nmodel = AutoModelForCausalLM.from_pretrained("databricks/dolly-v2-12b")\ntokenizer = AutoTokenizer.from_pretrained("databricks/dolly-v2-12b")\n\nschema = {\n    "type": "object",\n    "properties": {\n        "name": {"type": "string"},\n        "age": {"type": "number"},\n        "is_student": {"type": "boolean"},\n        "courses": {\n            "type": "array",\n            "items": {"type": "string"}\n        }\n    }\n}\n\nprompt = "Generate a person\'s information based on the following schema:"\njsonformer = Jsonformer(model, tokenizer, json_schema, prompt)\ngenerated_data = jsonformer()\n\nprint(generated_data)\n```\n\n## Features\n\n- Bulletproof JSON generation: Jsonformer ensures that the generated JSON is always syntactically correct and conforms to the specified schema.\n- Efficiency: By generating only the content tokens and filling in the fixed tokens, Jsonformer is more efficient than generating a full JSON string and parsing it.\n- Flexible and extendable: Jsonformer is built on top of the HuggingFace transformers library, making it compatible with any model that supports the HuggingFace interface.\n\n## Installation\n\n```bash\npip install jsonformer\n```\n\n## License\n\nJsonformer is released under the MIT License. You are free to use, modify, and distribute this software for any purpose, commercial or non-commercial, as long as the original copyright and license notice are included.\n',
     'author': '1rgs',
     'author_email': 'rgsduke@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `jsonformer-0.4.0/PKG-INFO` & `jsonformer-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonformer
-Version: 0.4.0
+Version: 0.5.0
 Summary: 
 Author: 1rgs
 Author-email: rgsduke@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

