# Comparing `tmp/fluidsdk-0.1.tar.gz` & `tmp/fluidsdk-0.2.tar.gz`

## Comparing `fluidsdk-0.1.tar` & `fluidsdk-0.2.tar`

### file list

```diff
@@ -1,15 +1,35 @@
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 fluidsdk-0.1/src/fluidsdk/__init__.py
--rw-r--r--   0        0        0     8228 2020-02-02 00:00:00.000000 fluidsdk-0.1/src/fluidsdk/conversational_modules.py
--rw-r--r--   0        0        0     2080 2020-02-02 00:00:00.000000 fluidsdk-0.1/src/fluidsdk/conversations_v3.py
--rw-r--r--   0        0        0     6437 2020-02-02 00:00:00.000000 fluidsdk-0.1/src/fluidsdk/filters.py
--rw-r--r--   0        0        0     3048 2020-02-02 00:00:00.000000 fluidsdk-0.1/src/fluidsdk/flow.py
--rw-r--r--   0        0        0    18516 2020-02-02 00:00:00.000000 fluidsdk-0.1/src/fluidsdk/intents.py
--rw-r--r--   0        0        0    15128 2020-02-02 00:00:00.000000 fluidsdk-0.1/src/fluidsdk/message.py
--rw-r--r--   0        0        0     5110 2020-02-02 00:00:00.000000 fluidsdk-0.1/src/fluidsdk/reminders.py
--rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 fluidsdk-0.1/src/fluidsdk/status_webhook.py
--rw-r--r--   0        0        0     3978 2020-02-02 00:00:00.000000 fluidsdk-0.1/src/fluidsdk/templates.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 fluidsdk-0.1/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fluidsdk-0.1/LICENSE
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 fluidsdk-0.1/README.md
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 fluidsdk-0.1/pyproject.toml
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 fluidsdk-0.1/PKG-INFO
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 fluidsdk-0.2/docs/Makefile
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 fluidsdk-0.2/docs/make.bat
+-rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 fluidsdk-0.2/docs/source/conf.py
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 fluidsdk-0.2/docs/source/fluid.rst
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 fluidsdk-0.2/docs/source/index.rst
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 fluidsdk-0.2/docs/source/_autosummary/fluidsdk.conversations_v3.Conversations_Model_v3.rst
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 fluidsdk-0.2/docs/source/_autosummary/fluidsdk.flow.Flow.rst
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 fluidsdk-0.2/docs/source/_autosummary/fluidsdk.flow.rst
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 fluidsdk-0.2/docs/source/_autosummary/fluidsdk.intents.rst
+-rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 fluidsdk-0.2/docs/source/getting_started/example.py
+-rw-r--r--   0        0        0     2677 2020-02-02 00:00:00.000000 fluidsdk-0.2/docs/source/getting_started/index.rst
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 fluidsdk-0.2/docs/source/pyrite/builder.rst
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 fluidsdk-0.2/docs/source/pyrite/index.rst
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 fluidsdk-0.2/docs/source/pyrite/library.rst
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 fluidsdk-0.2/src/fluidsdk/__init__.py
+-rw-r--r--   0        0        0     8228 2020-02-02 00:00:00.000000 fluidsdk-0.2/src/fluidsdk/conversational_modules.py
+-rw-r--r--   0        0        0     2080 2020-02-02 00:00:00.000000 fluidsdk-0.2/src/fluidsdk/conversations_v3.py
+-rw-r--r--   0        0        0     6437 2020-02-02 00:00:00.000000 fluidsdk-0.2/src/fluidsdk/filters.py
+-rw-r--r--   0        0        0     3068 2020-02-02 00:00:00.000000 fluidsdk-0.2/src/fluidsdk/flow.py
+-rw-r--r--   0        0        0    18596 2020-02-02 00:00:00.000000 fluidsdk-0.2/src/fluidsdk/intents.py
+-rw-r--r--   0        0        0    13243 2020-02-02 00:00:00.000000 fluidsdk-0.2/src/fluidsdk/macros.py
+-rw-r--r--   0        0        0    15128 2020-02-02 00:00:00.000000 fluidsdk-0.2/src/fluidsdk/message.py
+-rw-r--r--   0        0        0     5110 2020-02-02 00:00:00.000000 fluidsdk-0.2/src/fluidsdk/reminders.py
+-rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 fluidsdk-0.2/src/fluidsdk/status_webhook.py
+-rw-r--r--   0        0        0     3979 2020-02-02 00:00:00.000000 fluidsdk-0.2/src/fluidsdk/templates.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 fluidsdk-0.2/src/fluidsdk/pyrite/__init__.py
+-rw-r--r--   0        0        0    23286 2020-02-02 00:00:00.000000 fluidsdk-0.2/src/fluidsdk/pyrite/builder.py
+-rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 fluidsdk-0.2/src/fluidsdk/pyrite/consts.py
+-rw-r--r--   0        0        0     8371 2020-02-02 00:00:00.000000 fluidsdk-0.2/src/fluidsdk/pyrite/library.py
+-rw-r--r--   0        0        0     3633 2020-02-02 00:00:00.000000 fluidsdk-0.2/src/fluidsdk/pyrite/utils.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 fluidsdk-0.2/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fluidsdk-0.2/LICENSE
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 fluidsdk-0.2/README.md
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 fluidsdk-0.2/pyproject.toml
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 fluidsdk-0.2/PKG-INFO
```

### Comparing `fluidsdk-0.1/src/fluidsdk/conversational_modules.py` & `fluidsdk-0.2/src/fluidsdk/conversational_modules.py`

 * *Files identical despite different names*

### Comparing `fluidsdk-0.1/src/fluidsdk/conversations_v3.py` & `fluidsdk-0.2/src/fluidsdk/conversations_v3.py`

 * *Files identical despite different names*

### Comparing `fluidsdk-0.1/src/fluidsdk/filters.py` & `fluidsdk-0.2/src/fluidsdk/filters.py`

 * *Files identical despite different names*

### Comparing `fluidsdk-0.1/src/fluidsdk/flow.py` & `fluidsdk-0.2/src/fluidsdk/flow.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+"""
+Flow model
+"""
+
 from typing import TYPE_CHECKING, Dict, List, Union
 
 from pydantic import BaseModel, Field
 
 from fluidsdk.filters import Filter
 from fluidsdk.intents import *
 from fluidsdk.message import *
```

### Comparing `fluidsdk-0.1/src/fluidsdk/intents.py` & `fluidsdk-0.2/src/fluidsdk/intents.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,14 +55,15 @@
             return type(self).parse_obj(output)
         else:
             raise TypeError
 
     class Config:
         fields = {"mixtrack": {"exclude": True}}
         allow_population_by_field_name = True
+        copy_on_model_validation = "none"
 
 
 @_basemodel_decorator
 class NextConfig(BaseModel):
     next: str
 
 
@@ -249,15 +250,20 @@
         description="Field in the user's Conversation_Model.data to store the answer in.",
     )
 
 
 @_basemodel_decorator
 class GPTSearchIntent(Intent):
     intent_type: Literal["gpt-search"] = "gpt-search"
-    engine: Literal["davinci", "curie", "babbage", "ada",] = Field(
+    engine: Literal[
+        "davinci",
+        "curie",
+        "babbage",
+        "ada",
+    ] = Field(
         "davinci",
         title="Engine",
         description="Name of the large language model to use.",
     )
     query: str = Field(
         ...,
         title="Query",
```

### Comparing `fluidsdk-0.1/src/fluidsdk/message.py` & `fluidsdk-0.2/src/fluidsdk/message.py`

 * *Files identical despite different names*

### Comparing `fluidsdk-0.1/src/fluidsdk/reminders.py` & `fluidsdk-0.2/src/fluidsdk/reminders.py`

 * *Files identical despite different names*

### Comparing `fluidsdk-0.1/src/fluidsdk/status_webhook.py` & `fluidsdk-0.2/src/fluidsdk/status_webhook.py`

 * *Files identical despite different names*

### Comparing `fluidsdk-0.1/src/fluidsdk/templates.py` & `fluidsdk-0.2/src/fluidsdk/templates.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import time
-from typing import List, TYPE_CHECKING
+from typing import TYPE_CHECKING, List
 
-from fluidsdk.conversational_modules import GPTConfig, OpenAIGPTConfig
 from pydantic import BaseModel, Field, PrivateAttr
 
+from fluidsdk.conversational_modules import GPTConfig, OpenAIGPTConfig
+
 template_cache = {}
 
 if TYPE_CHECKING:
     from dataclasses import dataclass as _basemodel_decorator
 else:
     _basemodel_decorator = lambda x: x
```

