# Comparing `tmp/opentrain-0.0.4.tar.gz` & `tmp/opentrain-0.1.0.tar.gz`

## Comparing `opentrain-0.0.4.tar` & `opentrain-0.1.0.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 opentrain-0.0.4/mkdocs.yml
--rw-r--r--   0        0        0     9670 2020-02-02 00:00:00.000000 opentrain-0.0.4/examples/text_classification_imdb.ipynb
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 opentrain-0.0.4/src/opentrain/__init__.py
--rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 opentrain-0.0.4/src/opentrain/predict.py
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 opentrain-0.0.4/src/opentrain/schemas.py
--rw-r--r--   0        0        0     3856 2020-02-02 00:00:00.000000 opentrain-0.0.4/src/opentrain/train.py
--rw-r--r--   0        0        0     2741 2020-02-02 00:00:00.000000 opentrain-0.0.4/src/opentrain/utils.py
--rw-r--r--   0        0        0     1316 2020-02-02 00:00:00.000000 opentrain-0.0.4/.gitignore
--rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 opentrain-0.0.4/LICENSE
--rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 opentrain-0.0.4/README.md
--rw-r--r--   0        0        0     2468 2020-02-02 00:00:00.000000 opentrain-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     3447 2020-02-02 00:00:00.000000 opentrain-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 opentrain-0.1.0/mkdocs.yml
+-rw-r--r--   0        0        0     9628 2020-02-02 00:00:00.000000 opentrain-0.1.0/examples/text_classification_imdb.ipynb
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 opentrain-0.1.0/src/opentrain/__init__.py
+-rw-r--r--   0        0        0     6758 2020-02-02 00:00:00.000000 opentrain-0.1.0/src/opentrain/dataset.py
+-rw-r--r--   0        0        0     3083 2020-02-02 00:00:00.000000 opentrain-0.1.0/src/opentrain/inference.py
+-rw-r--r--   0        0        0     1845 2020-02-02 00:00:00.000000 opentrain-0.1.0/src/opentrain/schemas.py
+-rw-r--r--   0        0        0     5446 2020-02-02 00:00:00.000000 opentrain-0.1.0/src/opentrain/train.py
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 opentrain-0.1.0/src/opentrain/typing.py
+-rw-r--r--   0        0        0     1316 2020-02-02 00:00:00.000000 opentrain-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 opentrain-0.1.0/LICENSE
+-rw-r--r--   0        0        0     2138 2020-02-02 00:00:00.000000 opentrain-0.1.0/README.md
+-rw-r--r--   0        0        0     2468 2020-02-02 00:00:00.000000 opentrain-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3650 2020-02-02 00:00:00.000000 opentrain-0.1.0/PKG-INFO
```

### Comparing `opentrain-0.0.4/mkdocs.yml` & `opentrain-0.1.0/mkdocs.yml`

 * *Files 4% similar despite different names*

```diff
@@ -44,8 +44,11 @@
     - icon: fontawesome/brands/twitter
       link: https://twitter.com/alvarobartt
     - icon: fontawesome/brands/linkedin
       link: https://www.linkedin.com/in/alvarobartt/
 
 nav:
   - Home: index.md
+  - Usage: usage.md
+  - Warning: warning.md
+  - TODOs: todos.md
   - License: license.md
```

### Comparing `opentrain-0.0.4/examples/text_classification_imdb.ipynb` & `opentrain-0.1.0/examples/text_classification_imdb.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9963541666666667%*

 * *Differences: {"'cells'": "{10: {'source': ['from opentrain import Train']}, 11: {'source': ['trainer = "*

 * *            'Train(model="curie")\']}, 12: {\'outputs\': {0: {\'text\': '*

 * *            '["/var/folders/tq/d6srhsd134l2b6x4sj01hpqr0000gn/T/ipykernel_14681/526391229.py:1: '*

 * *            'UserWarning: Since the OpenAI API may take from minutes to hours depending on the '*

 * *            "size of the training data, then from now on, you'll be able to check its progress via "*

 * *            'the following command: `openai api fi […]*

```diff
@@ -149,42 +149,42 @@
         },
         {
             "cell_type": "code",
             "execution_count": 54,
             "metadata": {},
             "outputs": [],
             "source": [
-                "from opentrain.train import OpenAITrainer"
+                "from opentrain import Train"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 55,
             "metadata": {},
             "outputs": [],
             "source": [
-                "trainer = OpenAITrainer(model=\"curie\")"
+                "trainer = Train(model=\"curie\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 56,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
-                        "/var/folders/tq/d6srhsd134l2b6x4sj01hpqr0000gn/T/ipykernel_14681/526391229.py:1: UserWarning: Since the OpenAI API may take from minutes to hours depending on the size of the training data, then from now on, you'll be able to check its progress via the following command: `openai api fine_tunes.follow -i ft-nbCAuynTlICBi7HfJ82XFB9F`. Once the training is completed, then you'll be able to use `OpenAIPredict` with the either the fine tune id returned, or from the model name generated by OpenAI linked to your account.\n",
-                        "  fine_tune_id = trainer.train(\"imdb.jsonl\", epochs=5, batch_size=64)\n"
+                        "/var/folders/tq/d6srhsd134l2b6x4sj01hpqr0000gn/T/ipykernel_14681/526391229.py:1: UserWarning: Since the OpenAI API may take from minutes to hours depending on the size of the training data, then from now on, you'll be able to check its progress via the following command: `openai api fine_tunes.follow -i ft-nbCAuynTlICBi7HfJ82XFB9F`. Once the training is completed, then you'll be able to use `Inference` with the either the fine tune id returned, or from the model name generated by OpenAI linked to your account.\n",
+                        "  fine_tune_id = trainer.train(\"imdb.jsonl\", n_epochs=5, batch_size=64)\n"
                     ]
                 }
             ],
             "source": [
-                "fine_tune_id = trainer.train(\"imdb.jsonl\", epochs=5, batch_size=64)"
+                "fine_tune_id = trainer.train(\"imdb.jsonl\", n_epochs=5, batch_size=64)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 57,
             "metadata": {},
             "outputs": [
@@ -284,34 +284,34 @@
                         "  \"message\": \"Fine-tune succeeded\",\n",
                         "  \"object\": \"fine-tune-event\"\n",
                         "}\n"
                     ]
                 }
             ],
             "source": [
-                "for event in trainer.track_training():\n",
+                "for event in trainer.track():\n",
                 "    print(event)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 61,
             "metadata": {},
             "outputs": [],
             "source": [
-                "from opentrain.predict import OpenAIPredict"
+                "from opentrain import Inference"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 62,
             "metadata": {},
             "outputs": [],
             "source": [
-                "predict = OpenAIPredict(fine_tune_id=fine_tune_id)"
+                "predict = Inference.from_fine_tune_id(fine_tune_id)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 63,
             "metadata": {},
             "outputs": [
```

### Comparing `opentrain-0.0.4/.gitignore` & `opentrain-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `opentrain-0.0.4/LICENSE` & `opentrain-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `opentrain-0.0.4/README.md` & `opentrain-0.1.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -9,23 +9,36 @@
 
 `opentrain` is a simple Python package to fine-tune OpenAI models for task-specific purposes such as text classification, token classification, or question answering.
 
 More information about OpenAI Fine-tuning at https://platform.openai.com/docs/guides/fine-tuning.
 
 ## 💻 Usage
 
+### 📦 Data management
+
+```python
+import openai
+from opentrain import Dataset
+
+openai.api_key = "<ADD_OPENAI_API_KEY_HERE>"
+
+dataset = Dataset.from_file("data.jsonl")
+dataset.info
+dataset.download(output_path="downloaded-data.jsonl")
+```
+
 ### 🦾 Fine-tune
 
 ```python
 import openai
-from opentrain.train import OpenAITrainer
+from opentrain import Train
 
 openai.api_key = "<ADD_OPENAI_API_KEY_HERE>"
 
-trainer = OpenAITrainer(model="ada")
+trainer = Train(model="ada")
 trainer.train(
     [
         {
             "prompt": "I love to play soccer ->",
             "completion": " soccer",
         },
         {
@@ -36,19 +49,19 @@
 )
 ```
 
 ### 🤖 Predict
 
 ```python
 import openai
-from opentrain.predict import OpenAIPredict
+from opentrain import Inference
 
 openai.api_key = "<ADD_OPENAI_API_KEY_HERE>"
 
-predict = OpenAIPredict(model="ada:ft-personal-2021-03-01-00-00-01")
+predict = Inference(model="ada:ft-personal-2021-03-01-00-00-01")
 predict.predict("I love to play ->")
 ```
 
 ## ⚠️ Warning
 
 Fine-tuning OpenAI models via their API may take too long, so please be patient. Also, bear in mind
 that in some cases you just won't need to fine-tune an OpenAI model for your task.
```

### Comparing `opentrain-0.0.4/pyproject.toml` & `opentrain-0.1.0/pyproject.toml`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -50,20 +50,20 @@
 [tool.hatch.envs.quality]
 features = [
   "quality",
 ]
 
 [tool.hatch.envs.quality.scripts]
 check = [
-  "ruff src tests",
   "black --check --diff --preview src tests",
+  "ruff src tests",
 ]
 style = [
-  "ruff --fix src tests",
   "black --preview src tests",
+  "ruff --fix src tests",
   "check",
 ]
 
 [tool.ruff]
 ignore = [
   "E501", # line too long, handled by black
   "B008", # do not perform function calls in argument defaults
```

### Comparing `opentrain-0.0.4/PKG-INFO` & `opentrain-0.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentrain
-Version: 0.0.4
+Version: 0.1.0
 Summary: 🚂 Fine-tune OpenAI models for text classification, question answering, and more
 Project-URL: Documentation, https://alvarobartt.github.io/opentrain
 Project-URL: Issues, https://github.com/alvarobartt/opentrain/issues
 Project-URL: Source, https://github.com/alvarobartt/opentrain
 Author-email: Alvaro Bartolome <alvarobartt@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
@@ -43,23 +43,36 @@
 
 `opentrain` is a simple Python package to fine-tune OpenAI models for task-specific purposes such as text classification, token classification, or question answering.
 
 More information about OpenAI Fine-tuning at https://platform.openai.com/docs/guides/fine-tuning.
 
 ## 💻 Usage
 
+### 📦 Data management
+
+```python
+import openai
+from opentrain import Dataset
+
+openai.api_key = "<ADD_OPENAI_API_KEY_HERE>"
+
+dataset = Dataset.from_file("data.jsonl")
+dataset.info
+dataset.download(output_path="downloaded-data.jsonl")
+```
+
 ### 🦾 Fine-tune
 
 ```python
 import openai
-from opentrain.train import OpenAITrainer
+from opentrain import Train
 
 openai.api_key = "<ADD_OPENAI_API_KEY_HERE>"
 
-trainer = OpenAITrainer(model="ada")
+trainer = Train(model="ada")
 trainer.train(
     [
         {
             "prompt": "I love to play soccer ->",
             "completion": " soccer",
         },
         {
@@ -70,19 +83,19 @@
 )
 ```
 
 ### 🤖 Predict
 
 ```python
 import openai
-from opentrain.predict import OpenAIPredict
+from opentrain import Inference
 
 openai.api_key = "<ADD_OPENAI_API_KEY_HERE>"
 
-predict = OpenAIPredict(model="ada:ft-personal-2021-03-01-00-00-01")
+predict = Inference(model="ada:ft-personal-2021-03-01-00-00-01")
 predict.predict("I love to play ->")
 ```
 
 ## ⚠️ Warning
 
 Fine-tuning OpenAI models via their API may take too long, so please be patient. Also, bear in mind
 that in some cases you just won't need to fine-tune an OpenAI model for your task.
```

