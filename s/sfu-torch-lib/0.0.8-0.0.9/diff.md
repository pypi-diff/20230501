# Comparing `tmp/sfu-torch-lib-0.0.8.tar.gz` & `tmp/sfu-torch-lib-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sfu-torch-lib-0.0.8.tar", max compression
+gzip compressed data, was "sfu-torch-lib-0.0.9.tar", max compression
```

## Comparing `sfu-torch-lib-0.0.8.tar` & `sfu-torch-lib-0.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1076 2022-04-04 17:58:13.250704 sfu-torch-lib-0.0.8/LICENSE
--rw-r--r--   0        0        0      701 2022-04-04 18:00:40.787995 sfu-torch-lib-0.0.8/pyproject.toml
--rw-r--r--   0        0        0        0 2022-04-04 17:58:13.254704 sfu-torch-lib-0.0.8/sfu_torch_lib/__init__.py
--rw-r--r--   0        0        0     4651 2022-04-04 17:58:13.254704 sfu-torch-lib-0.0.8/sfu_torch_lib/file_fetcher.py
--rw-r--r--   0        0        0     7750 2022-04-04 17:58:13.254704 sfu-torch-lib-0.0.8/sfu_torch_lib/io.py
--rw-r--r--   0        0        0     4974 2022-04-04 17:58:13.254704 sfu-torch-lib-0.0.8/sfu_torch_lib/mlflow.py
--rw-r--r--   0        0        0        0 2022-04-04 17:58:13.254704 sfu-torch-lib-0.0.8/sfu_torch_lib/modules/__init__.py
--rw-r--r--   0        0        0     2845 2022-04-04 17:58:13.254704 sfu-torch-lib-0.0.8/sfu_torch_lib/modules/batchrenorm.py
--rw-r--r--   0        0        0      671 2022-04-04 17:58:13.254704 sfu-torch-lib-0.0.8/sfu_torch_lib/modules/convolution.py
--rw-r--r--   0        0        0     4281 2022-04-04 17:58:13.254704 sfu-torch-lib-0.0.8/sfu_torch_lib/optimization.py
--rw-r--r--   0        0        0     3030 2022-04-04 17:58:13.254704 sfu-torch-lib-0.0.8/sfu_torch_lib/parameters.py
--rw-r--r--   0        0        0     5879 2022-04-04 17:58:13.254704 sfu-torch-lib-0.0.8/sfu_torch_lib/processing.py
--rw-r--r--   0        0        0     4228 2022-04-04 17:58:13.254704 sfu-torch-lib-0.0.8/sfu_torch_lib/slack.py
--rw-r--r--   0        0        0      915 2022-04-04 17:58:13.254704 sfu-torch-lib-0.0.8/sfu_torch_lib/state.py
--rw-r--r--   0        0        0     2949 2022-04-04 17:58:13.254704 sfu-torch-lib-0.0.8/sfu_torch_lib/tree.py
--rw-r--r--   0        0        0      174 2022-04-04 17:58:13.254704 sfu-torch-lib-0.0.8/sfu_torch_lib/types.py
--rw-r--r--   0        0        0     3102 2022-04-04 17:58:13.254704 sfu-torch-lib-0.0.8/sfu_torch_lib/utils.py
--rw-r--r--   0        0        0      828 2022-04-04 18:00:42.020643 sfu-torch-lib-0.0.8/setup.py
--rw-r--r--   0        0        0      703 2022-04-04 18:00:42.020985 sfu-torch-lib-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1076 2022-04-04 19:39:53.729550 sfu-torch-lib-0.0.9/LICENSE
+-rw-r--r--   0        0        0      701 2022-04-04 19:42:25.182789 sfu-torch-lib-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-04-04 19:39:53.729550 sfu-torch-lib-0.0.9/sfu_torch_lib/__init__.py
+-rw-r--r--   0        0        0     4651 2022-04-04 19:39:53.729550 sfu-torch-lib-0.0.9/sfu_torch_lib/file_fetcher.py
+-rw-r--r--   0        0        0     7750 2022-04-04 19:39:53.729550 sfu-torch-lib-0.0.9/sfu_torch_lib/io.py
+-rw-r--r--   0        0        0     4974 2022-04-04 19:39:53.729550 sfu-torch-lib-0.0.9/sfu_torch_lib/mlflow.py
+-rw-r--r--   0        0        0        0 2022-04-04 19:39:53.729550 sfu-torch-lib-0.0.9/sfu_torch_lib/modules/__init__.py
+-rw-r--r--   0        0        0     2845 2022-04-04 19:39:53.729550 sfu-torch-lib-0.0.9/sfu_torch_lib/modules/batchrenorm.py
+-rw-r--r--   0        0        0      671 2022-04-04 19:39:53.729550 sfu-torch-lib-0.0.9/sfu_torch_lib/modules/convolution.py
+-rw-r--r--   0        0        0     4281 2022-04-04 19:39:53.729550 sfu-torch-lib-0.0.9/sfu_torch_lib/optimization.py
+-rw-r--r--   0        0        0     3054 2022-04-04 19:39:53.729550 sfu-torch-lib-0.0.9/sfu_torch_lib/parameters.py
+-rw-r--r--   0        0        0     5879 2022-04-04 19:39:53.729550 sfu-torch-lib-0.0.9/sfu_torch_lib/processing.py
+-rw-r--r--   0        0        0     4228 2022-04-04 19:39:53.729550 sfu-torch-lib-0.0.9/sfu_torch_lib/slack.py
+-rw-r--r--   0        0        0      915 2022-04-04 19:39:53.729550 sfu-torch-lib-0.0.9/sfu_torch_lib/state.py
+-rw-r--r--   0        0        0     2949 2022-04-04 19:39:53.729550 sfu-torch-lib-0.0.9/sfu_torch_lib/tree.py
+-rw-r--r--   0        0        0      174 2022-04-04 19:39:53.729550 sfu-torch-lib-0.0.9/sfu_torch_lib/types.py
+-rw-r--r--   0        0        0     3102 2022-04-04 19:39:53.729550 sfu-torch-lib-0.0.9/sfu_torch_lib/utils.py
+-rw-r--r--   0        0        0      828 2022-04-04 19:42:26.394713 sfu-torch-lib-0.0.9/setup.py
+-rw-r--r--   0        0        0      703 2022-04-04 19:42:26.395028 sfu-torch-lib-0.0.9/PKG-INFO
```

### Comparing `sfu-torch-lib-0.0.8/LICENSE` & `sfu-torch-lib-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sfu-torch-lib-0.0.8/pyproject.toml` & `sfu-torch-lib-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sfu-torch-lib"
-version = "0.0.8"
+version = "0.0.9"
 description = "Libraries that support the development of machine learning models in PyTorch."
 authors = ["Anderson de Andrade <anderson_de_andrade@sfu.ca>"]
 exclude = ["tests/*"]
 
 [[tool.poetry.source]]
 name = "private"
 url = "https://pypi.org/simple"
```

### Comparing `sfu-torch-lib-0.0.8/sfu_torch_lib/file_fetcher.py` & `sfu-torch-lib-0.0.9/sfu_torch_lib/file_fetcher.py`

 * *Files identical despite different names*

### Comparing `sfu-torch-lib-0.0.8/sfu_torch_lib/io.py` & `sfu-torch-lib-0.0.9/sfu_torch_lib/io.py`

 * *Files identical despite different names*

### Comparing `sfu-torch-lib-0.0.8/sfu_torch_lib/mlflow.py` & `sfu-torch-lib-0.0.9/sfu_torch_lib/mlflow.py`

 * *Files identical despite different names*

### Comparing `sfu-torch-lib-0.0.8/sfu_torch_lib/modules/batchrenorm.py` & `sfu-torch-lib-0.0.9/sfu_torch_lib/modules/batchrenorm.py`

 * *Files identical despite different names*

### Comparing `sfu-torch-lib-0.0.8/sfu_torch_lib/modules/convolution.py` & `sfu-torch-lib-0.0.9/sfu_torch_lib/modules/convolution.py`

 * *Files identical despite different names*

### Comparing `sfu-torch-lib-0.0.8/sfu_torch_lib/optimization.py` & `sfu-torch-lib-0.0.9/sfu_torch_lib/optimization.py`

 * *Files identical despite different names*

### Comparing `sfu-torch-lib-0.0.8/sfu_torch_lib/parameters.py` & `sfu-torch-lib-0.0.9/sfu_torch_lib/parameters.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,19 +52,20 @@
 
     for index, (name, parameter) in enumerate(signature.parameters.items()):
         transformed_name = name.replace('_', '-')
 
         if index < len(positional_arguments):
             arguments[transformed_name] = positional_arguments[index]
 
-        if not ignore_keyword_arguments and transformed_name in keyword_arguments:
-            arguments[transformed_name] = keyword_arguments[transformed_name]
+        if not ignore_keyword_arguments:
+            if transformed_name in keyword_arguments:
+                arguments[transformed_name] = keyword_arguments[transformed_name]
 
-        elif parameter.default != parameter.empty:
-            arguments[transformed_name] = parameter.default
+            elif parameter.default != parameter.empty:
+                arguments[transformed_name] = parameter.default
 
     return arguments
 
 
 def flatten_dictionary(parameters: Mapping[Any, Any], delimiter: str = '/') -> Dict[str, Any]:
     def _dictionary_generator(input_dictionary, prefixes=None):
         prefixes = prefixes[:] if prefixes else []
```

### Comparing `sfu-torch-lib-0.0.8/sfu_torch_lib/processing.py` & `sfu-torch-lib-0.0.9/sfu_torch_lib/processing.py`

 * *Files identical despite different names*

### Comparing `sfu-torch-lib-0.0.8/sfu_torch_lib/slack.py` & `sfu-torch-lib-0.0.9/sfu_torch_lib/slack.py`

 * *Files identical despite different names*

### Comparing `sfu-torch-lib-0.0.8/sfu_torch_lib/state.py` & `sfu-torch-lib-0.0.9/sfu_torch_lib/state.py`

 * *Files identical despite different names*

### Comparing `sfu-torch-lib-0.0.8/sfu_torch_lib/tree.py` & `sfu-torch-lib-0.0.9/sfu_torch_lib/tree.py`

 * *Files identical despite different names*

### Comparing `sfu-torch-lib-0.0.8/sfu_torch_lib/utils.py` & `sfu-torch-lib-0.0.9/sfu_torch_lib/utils.py`

 * *Files identical despite different names*

### Comparing `sfu-torch-lib-0.0.8/setup.py` & `sfu-torch-lib-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
  'pytorch-lightning>=1,<2',
  'requests>=2,<3',
  's3fs>=2022,<2023',
  'torch>=1,<2']
 
 setup_kwargs = {
     'name': 'sfu-torch-lib',
-    'version': '0.0.8',
+    'version': '0.0.9',
     'description': 'Libraries that support the development of machine learning models in PyTorch.',
     'long_description': None,
     'author': 'Anderson de Andrade',
     'author_email': 'anderson_de_andrade@sfu.ca',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `sfu-torch-lib-0.0.8/PKG-INFO` & `sfu-torch-lib-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sfu-torch-lib
-Version: 0.0.8
+Version: 0.0.9
 Summary: Libraries that support the development of machine learning models in PyTorch.
 Author: Anderson de Andrade
 Author-email: anderson_de_andrade@sfu.ca
 Requires-Python: >=3.8,<=3.10
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
```

