# Comparing `tmp/span_marker-0.2.2.tar.gz` & `tmp/span_marker-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "span_marker-0.2.2.tar", last modified: Thu Apr 13 14:12:02 2023, max compression
+gzip compressed data, was "span_marker-1.0.0.tar", last modified: Mon May  1 13:02:54 2023, max compression
```

## Comparing `span_marker-0.2.2.tar` & `span_marker-1.0.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 14:12:02.552919 span_marker-0.2.2/
--rw-rw-rw-   0        0        0     1088 2023-03-28 09:30:50.000000 span_marker-0.2.2/LICENSE
--rw-rw-rw-   0        0        0     4407 2023-04-13 14:12:02.552919 span_marker-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     3830 2023-04-07 10:47:40.000000 span_marker-0.2.2/README.md
--rw-rw-rw-   0        0        0     2349 2023-04-13 12:27:58.000000 span_marker-0.2.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-13 14:12:02.552919 span_marker-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0       41 2023-03-28 09:28:01.000000 span_marker-0.2.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-13 14:12:02.534551 span_marker-0.2.2/span_marker/
--rw-rw-rw-   0        0        0      352 2023-04-13 14:11:49.000000 span_marker-0.2.2/span_marker/__init__.py
--rw-rw-rw-   0        0        0     6408 2023-04-13 14:08:07.000000 span_marker-0.2.2/span_marker/configuration.py
--rw-rw-rw-   0        0        0     5389 2023-04-13 14:08:07.000000 span_marker-0.2.2/span_marker/data_collator.py
--rw-rw-rw-   0        0        0     4295 2023-04-13 14:08:07.000000 span_marker-0.2.2/span_marker/evaluation.py
--rw-rw-rw-   0        0        0     4831 2023-04-06 07:35:29.000000 span_marker-0.2.2/span_marker/label_normalizer.py
--rw-rw-rw-   0        0        0     1089 2023-04-07 14:45:51.000000 span_marker-0.2.2/span_marker/model_card.py
--rw-rw-rw-   0        0        0    21801 2023-04-13 14:08:07.000000 span_marker-0.2.2/span_marker/modeling.py
--rw-rw-rw-   0        0        0     1686 2023-04-06 14:00:45.000000 span_marker-0.2.2/span_marker/output.py
--rw-rw-rw-   0        0        0     6313 2023-04-13 14:08:07.000000 span_marker-0.2.2/span_marker/tokenizer.py
--rw-rw-rw-   0        0        0    11036 2023-04-11 11:25:40.000000 span_marker-0.2.2/span_marker/trainer.py
-drwxrwxrwx   0        0        0        0 2023-04-13 14:12:02.549567 span_marker-0.2.2/span_marker.egg-info/
--rw-rw-rw-   0        0        0     4407 2023-04-13 14:12:02.000000 span_marker-0.2.2/span_marker.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      548 2023-04-13 14:12:02.000000 span_marker-0.2.2/span_marker.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 14:12:02.000000 span_marker-0.2.2/span_marker.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      189 2023-04-13 14:12:02.000000 span_marker-0.2.2/span_marker.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-13 14:12:02.000000 span_marker-0.2.2/span_marker.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-13 14:12:02.551916 span_marker-0.2.2/tests/
--rw-rw-rw-   0        0        0      961 2023-04-06 07:35:29.000000 span_marker-0.2.2/tests/test_configuration.py
--rw-rw-rw-   0        0        0     3534 2023-04-06 07:35:29.000000 span_marker-0.2.2/tests/test_modeling.py
--rw-rw-rw-   0        0        0     3992 2023-04-06 07:35:29.000000 span_marker-0.2.2/tests/test_trainer.py
+drwxrwxrwx   0        0        0        0 2023-05-01 13:02:54.894052 span_marker-1.0.0/
+-rw-rw-rw-   0        0        0    11558 2023-05-01 10:45:08.000000 span_marker-1.0.0/LICENSE
+-rw-rw-rw-   0        0        0     7173 2023-05-01 13:02:54.893052 span_marker-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     6596 2023-05-01 10:45:08.000000 span_marker-1.0.0/README.md
+-rw-rw-rw-   0        0        0     2436 2023-05-01 10:45:08.000000 span_marker-1.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-01 13:02:54.894052 span_marker-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0       41 2023-03-28 09:28:01.000000 span_marker-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 13:02:54.887052 span_marker-1.0.0/span_marker/
+-rw-rw-rw-   0        0        0      446 2023-05-01 12:56:43.000000 span_marker-1.0.0/span_marker/__init__.py
+-rw-rw-rw-   0        0        0     6368 2023-05-01 10:45:08.000000 span_marker-1.0.0/span_marker/configuration.py
+-rw-rw-rw-   0        0        0     6154 2023-05-01 10:45:08.000000 span_marker-1.0.0/span_marker/data_collator.py
+-rw-rw-rw-   0        0        0     4684 2023-05-01 10:45:08.000000 span_marker-1.0.0/span_marker/evaluation.py
+-rw-rw-rw-   0        0        0     5230 2023-05-01 10:45:08.000000 span_marker-1.0.0/span_marker/label_normalizer.py
+-rw-rw-rw-   0        0        0     2488 2023-05-01 10:45:08.000000 span_marker-1.0.0/span_marker/model_card.py
+-rw-rw-rw-   0        0        0    26327 2023-05-01 11:48:11.000000 span_marker-1.0.0/span_marker/modeling.py
+-rw-rw-rw-   0        0        0     1745 2023-05-01 10:45:08.000000 span_marker-1.0.0/span_marker/output.py
+-rw-rw-rw-   0        0        0    12478 2023-05-01 10:45:08.000000 span_marker-1.0.0/span_marker/tokenizer.py
+-rw-rw-rw-   0        0        0    11257 2023-05-01 10:45:08.000000 span_marker-1.0.0/span_marker/trainer.py
+drwxrwxrwx   0        0        0        0 2023-05-01 13:02:54.891054 span_marker-1.0.0/span_marker.egg-info/
+-rw-rw-rw-   0        0        0     7173 2023-05-01 13:02:54.000000 span_marker-1.0.0/span_marker.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      548 2023-05-01 13:02:54.000000 span_marker-1.0.0/span_marker.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 13:02:54.000000 span_marker-1.0.0/span_marker.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      244 2023-05-01 13:02:54.000000 span_marker-1.0.0/span_marker.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-01 13:02:54.000000 span_marker-1.0.0/span_marker.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-01 13:02:54.893052 span_marker-1.0.0/tests/
+-rw-rw-rw-   0        0        0      961 2023-05-01 11:30:18.000000 span_marker-1.0.0/tests/test_configuration.py
+-rw-rw-rw-   0        0        0     4708 2023-05-01 11:48:11.000000 span_marker-1.0.0/tests/test_modeling.py
+-rw-rw-rw-   0        0        0     8518 2023-05-01 11:40:43.000000 span_marker-1.0.0/tests/test_trainer.py
```

### Comparing `span_marker-0.2.2/pyproject.toml` & `span_marker-1.0.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -21,18 +21,21 @@
     {name = "Tom Aarsen"}
 ]
 maintainers = [
     {name = "Tom Aarsen"}
 ]
 dependencies = [
     "torch",
-    "transformers>4.19.0", # required for EvalPrediction.inputs
-    "datasets",
+    "transformers>=4.19.0", # required for EvalPrediction.inputs
+    "datasets>=2.0.0",
+    "packaging>=20.0",
     "evaluate",
-    "seqeval"
+    "seqeval",
+    "jinja2",
+    "huggingface_hub"
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 dev = [
     "pre-commit",
     "ruff",
@@ -43,15 +46,16 @@
 docs = [
     "nltk_theme",
     "sphinx",
     "m2r2",
     "better-apidoc",
     "nbsphinx",
     "nbconvert<7",
-    "pandoc<3"
+    "pandoc<3",
+    "ipython"
 ]
 wandb = [
     "wandb"
 ]
 
 [project.urls]
 Documentation = "https://tomaarsen.github.io/SpanMarkerNER"
```

### Comparing `span_marker-0.2.2/span_marker/configuration.py` & `span_marker-1.0.0/span_marker/configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,54 +1,55 @@
 from collections import defaultdict
 from typing import Any, Dict, Iterable, Optional, Set, Union
 
 from transformers import PretrainedConfig
 
 
 class SpanMarkerConfig(PretrainedConfig):
+    """Configuration class for SpanMarkerModel instances.
+
+    Args:
+        encoder_config (`Optional[Dict[str, Any]]`): The configuration dictionary for the
+            underlying encoder used by the SpanMarkerModel instance. Defaults to None.
+        model_max_length (`Optional[int]`): The total number of tokens that can be processed before
+            truncation. If None, the tokenizer its `model_max_length` is used, and if that value is
+            not defined, it becomes 512 instead. Defaults to None.
+        marker_max_length (`int`): The maximum length for each of the span markers. A value of 128
+            means that each training and inferencing sample contains a maximum of 128 start markers
+            and 128 end markers, for a total of 256 markers per sample. Defaults to 128.
+        entity_max_length (`int`): The maximum length of an entity span in terms of words.
+            Defaults to 8.
+
+    Example::
+
+        # These configuration settings are provided via kwargs to `SpanMarkerModel.from_pretrained`:
+        model = SpanMarkerModel.from_pretrained(
+            "bert-base-cased",
+            labels=labels,
+            model_max_length=256,
+            marker_max_length=128,
+            entity_max_length=8,
+        )
+
+    Raises:
+        ValueError: If the labels provided to :meth:`~span_marker.modeling.SpanMarkerModel.from_pretrained` do not
+            contain the required `"O"` label.
+    """
+
     model_type: str = "span-marker"
     is_composition = True
 
     def __init__(
         self,
         encoder_config: Optional[Dict[str, Any]] = None,
         model_max_length: Optional[int] = None,
-        marker_max_length: int = 256,
-        entity_max_length: int = 16,
+        marker_max_length: int = 128,
+        entity_max_length: int = 8,
         **kwargs,
     ) -> None:
-        """Configuration class for SpanMarkerModel instances.
-
-        Args:
-            encoder_config (`Optional[Dict[str, Any]]`): The configuration dictionary for the
-                underlying encoder used by the SpanMarkerModel instance. Defaults to None.
-            model_max_length (`Optional[int]`): The total number of tokens that can be processed before
-                truncation. If None, the tokenizer its `model_max_length` is used, and if that value is
-                not defined, it becomes 512 instead. Defaults to None.
-            marker_max_length (`int`): The maximum length for each of the span markers. A value of 256
-                means that each training and inferencing sample contains a maximum of 256 start markers
-                and 256 end markers. Defaults to 256.
-            entity_max_length (`int`): The maximum length of an entity span in terms of words.
-                Defaults to 16.
-
-        Example::
-
-            # These configuration settings are provided via kwargs to `SpanMarkerModel.from_pretrained`:
-            model = SpanMarkerModel.from_pretrained(
-                "bert-base-cased",
-                labels=labels,
-                model_max_length=256,
-                marker_max_length=128,
-                entity_max_length=8,
-            )
-
-        Raises:
-            ValueError: If the labels provided to `SpanMarkerModel.from_pretrained` does not contain a "O",
-                a ValueError is raised.
-        """
         self.encoder = encoder_config
         self.model_max_length = model_max_length
         self.model_max_length_default = 512
         self.marker_max_length = marker_max_length
         self.entity_max_length = entity_max_length
         self.span_marker_version = kwargs.pop("span_marker_version", None)
         super().__init__(**kwargs)
```

### Comparing `span_marker-0.2.2/span_marker/data_collator.py` & `span_marker-1.0.0/span_marker/data_collator.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 from span_marker.tokenizer import SpanMarkerTokenizer
 
 
 @dataclass
 class SpanMarkerDataCollator:
     """
     Data Collator class responsible for converting the minimal outputs from the tokenizer into
-    complete and meaningful inputs to the model. In particular, the `input_ids` from the tokenizer
+    complete and meaningful inputs to the model. In particular, the ``input_ids`` from the tokenizer
     features are padded, and the correct amount of start and end markers (with padding) are added.
 
-    Furthermore, the position IDs are generated for the input IDs, and `start_position_ids` and
-    `end_position_ids` are used alongside some padding to create a full position ID vector.
+    Furthermore, the position IDs are generated for the input IDs, and ``start_position_ids`` and
+    ``end_position_ids`` are used alongside some padding to create a full position ID vector.
 
     Lastly, the attention matrix is computed.
 
     The expected usage is something like:
 
     >>> collator = SpanMarkerDataCollator(...)
     >>> tokenized = tokenizer(...)
@@ -28,59 +28,63 @@
     >>> output = model(**batch)
     """
 
     tokenizer: SpanMarkerTokenizer
     marker_max_length: int
 
     def __call__(self, features: List[Dict[str, Any]]) -> Dict[str, torch.Tensor]:
-        """Convert the minimal tokenizer outputs into inputs ready for `model.forward`.
+        """Convert the minimal tokenizer outputs into inputs ready for :meth:`~span_marker.modeling.SpanMarkerModel.forward`.
 
         Args:
             features (List[Dict[str, Any]]): A list of dictionaries, one element per sample in the batch.
                 The dictionaries contain the following keys:
 
-                * `input_ids`: The non-padded input IDs.
-                * `num_spans`: The number of spans that should be encoded in each sample.
-                * `start_position_ids`: The position IDs of the start markers in the sample.
-                * `end_position_ids`: The position IDs of the end markers in the sample.
-                * `labels` (optional): The labels corresponding to each of the spans in the sample.
-                * `num_words` (optional): The number of words in the input sample.
+                * ``input_ids``: The non-padded input IDs.
+                * ``num_spans``: The number of spans that should be encoded in each sample.
+                * ``start_position_ids``: The position IDs of the start markers in the sample.
+                * ``end_position_ids``: The position IDs of the end markers in the sample.
+                * ``labels`` (optional): The labels corresponding to each of the spans in the sample.
+                * ``num_words`` (optional): The number of words in the input sample.
                     Required for some evaluation metrics.
 
         Returns:
-            Dict[str, torch.Tensor]: Batch dictionary ready to be fed into :meth:`~SpanMarkerModel.forward`.
+            Dict[str, torch.Tensor]: Batch dictionary ready to be fed into :meth:`~span_marker.modeling.SpanMarkerModel.forward`.
         """
         total_size = self.tokenizer.model_max_length + 2 * self.marker_max_length
-        start_marker_idx = self.tokenizer.model_max_length
-        end_marker_idx = self.tokenizer.model_max_length + self.marker_max_length
         batch = defaultdict(list)
         num_words = []
+        start_marker_indices = []
+        num_marker_pairs = []
         for sample in features:
             input_ids = sample["input_ids"]
             num_spans = sample["num_spans"]
             num_tokens = len(input_ids)
 
+            # The start markers start after the input IDs, rounded up to the nearest even number
+            start_marker_idx = num_tokens + num_tokens % 2
+            end_marker_idx = start_marker_idx + num_spans
+
             # Prepare input_ids by padding and adding start and end markers
             if not isinstance(input_ids, torch.Tensor):
                 input_ids = torch.tensor(input_ids, dtype=torch.int)
             else:
                 input_ids.to(torch.int)
             input_ids = F.pad(input_ids, (0, total_size - len(input_ids)), value=self.tokenizer.pad_token_id)
             input_ids[start_marker_idx : start_marker_idx + num_spans] = self.tokenizer.start_marker_id
             input_ids[end_marker_idx : end_marker_idx + num_spans] = self.tokenizer.end_marker_id
             batch["input_ids"].append(input_ids)
 
             # Prepare position IDs
-            position_ids = torch.arange(num_tokens, dtype=torch.int) + 2
+            position_ids = torch.arange(num_tokens, dtype=torch.int)
             position_ids = F.pad(position_ids, (0, total_size - len(position_ids)), value=0)
-            position_ids[start_marker_idx : start_marker_idx + num_spans] = (
-                torch.tensor(sample["start_position_ids"]) + 2
-            )
-            position_ids[end_marker_idx : end_marker_idx + num_spans] = torch.tensor(sample["end_position_ids"]) + 2
-            batch["position_ids"].append(position_ids)
+            position_ids[start_marker_idx : start_marker_idx + num_spans] = torch.tensor(sample["start_position_ids"])
+            position_ids[end_marker_idx : end_marker_idx + num_spans] = torch.tensor(sample["end_position_ids"])
+            # Increase the position_ids by 2, inspired by PL-Marker. The intuition is that these position IDs
+            # better match the circumstances under which the underlying encoders are trained.
+            batch["position_ids"].append(position_ids + 2)
 
             # Prepare attention mask matrix
             attention_mask = torch.zeros((total_size, total_size), dtype=torch.bool)
             # text tokens self-attention
             attention_mask[:num_tokens, :num_tokens] = 1
             # let markers attend text tokens
             attention_mask[start_marker_idx : start_marker_idx + num_spans, :num_tokens] = 1
@@ -90,21 +94,26 @@
             end_index_list = list(range(end_marker_idx, end_marker_idx + num_spans))
             attention_mask[start_index_list, start_index_list] = 1
             attention_mask[start_index_list, end_index_list] = 1
             attention_mask[end_index_list, start_index_list] = 1
             attention_mask[end_index_list, end_index_list] = 1
             batch["attention_mask"].append(attention_mask)
 
+            # Add start of the markers, so the model knows where the input IDs end and where the markers start
+            start_marker_indices.append(start_marker_idx)
+            num_marker_pairs.append(end_marker_idx - start_marker_idx)
+
             if "labels" in sample:
                 labels = torch.tensor(sample["labels"])
-                labels = F.pad(labels, (0, self.marker_max_length - len(labels)), value=-100)
+                labels = F.pad(labels, (0, (total_size // 2) - len(labels)), value=-100)
                 batch["labels"].append(labels)
 
             if "num_words" in sample:
                 num_words.append(sample["num_words"])
 
         batch = {key: torch.stack(value) for key, value in batch.items()}
         # Used for evaluation, does not need to be padded/stacked
         if num_words:
             batch["num_words"] = torch.tensor(num_words)
-
+        batch["start_marker_indices"] = torch.tensor(start_marker_indices)
+        batch["num_marker_pairs"] = torch.tensor(num_marker_pairs)
         return batch
```

### Comparing `span_marker-0.2.2/span_marker/evaluation.py` & `span_marker-1.0.0/span_marker/evaluation.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,32 @@
+import warnings
 from typing import Dict
 
 import evaluate
 import torch
+from sklearn.exceptions import UndefinedMetricWarning
 from transformers import EvalPrediction
 
 from span_marker.tokenizer import SpanMarkerTokenizer
 
 
 def compute_f1_via_seqeval(tokenizer: SpanMarkerTokenizer, eval_prediction: EvalPrediction) -> Dict[str, float]:
-    """Compute micro-F1, recall, precision and accuracy scores using `seqeval` for the evaluation predictions.
+    """Compute micro-F1, recall, precision and accuracy scores using ``seqeval`` for the evaluation predictions.
 
     Note:
         We assume that samples are not shuffled for the evaluation/prediction.
         With other words, don't use this on the (shuffled) train dataset!
 
     Args:
-        tokenizer (SpanMarkerTokenizer):
-        eval_prediction (EvalPrediction): _description_
+        tokenizer (SpanMarkerTokenizer): The model its tokenizer.
+        eval_prediction (~transformers.EvalPrediction): The predictions resulting from the evaluations.
 
     Returns:
-        Dict[str, float]: Dictionary with `"overall_precision"`, `"overall_recall"`, `"overall_f1"`
-            and `"overall_accuracy"` keys.
+        Dict[str, float]: Dictionary with ``"overall_precision"``, ``"overall_recall"``, ``"overall_f1"``
+            and ``"overall_accuracy"`` keys.
     """
     inputs = eval_prediction.inputs
     gold_labels = eval_prediction.label_ids
     logits = eval_prediction.predictions[0]
     num_words = eval_prediction.predictions[-1]
 
     # Compute probabilities via softmax and extract 'winning' scores/labels
@@ -35,25 +37,27 @@
     sample_dict = {}
     for sample_idx in range(inputs.shape[0]):
         tokens = inputs[sample_idx]
         text = tokenizer.decode(tokens, skip_special_tokens=True)
         token_hash = hash(text)
         if token_hash not in sample_dict:
             spans = list(tokenizer.get_all_valid_spans(num_words[sample_idx], tokenizer.config.entity_max_length))
+            mask = gold_labels[sample_idx] != -100
             sample_dict[token_hash] = {
                 "text": text,
                 "spans": spans,
-                "gold_labels": gold_labels[sample_idx].tolist(),
-                "pred_labels": pred_labels[sample_idx].tolist(),
+                "gold_labels": gold_labels[sample_idx][mask].tolist(),
+                "pred_labels": pred_labels[sample_idx][mask].tolist(),
                 "scores": scores[sample_idx].tolist(),
                 "num_words": num_words[sample_idx],
             }
         else:
-            sample_dict[token_hash]["gold_labels"] += gold_labels[sample_idx].tolist()
-            sample_dict[token_hash]["pred_labels"] += pred_labels[sample_idx].tolist()
+            mask = gold_labels[sample_idx] != -100
+            sample_dict[token_hash]["gold_labels"] += gold_labels[sample_idx][mask].tolist()
+            sample_dict[token_hash]["pred_labels"] += pred_labels[sample_idx][mask].tolist()
             sample_dict[token_hash]["scores"] += scores[sample_idx].tolist()
 
     outside_id = tokenizer.config.outside_id
     id2label = tokenizer.config.id2label
     # seqeval works wonders for NER evaluation
     seqeval = evaluate.load("seqeval")
     for sample in sample_dict.values():
@@ -75,12 +79,14 @@
         for _, span, pred_label in sorted(zip(scores, spans, pred_labels), key=lambda tup: tup[0], reverse=True):
             if pred_label != outside_id and all(pred_labels_per_tokens[i] == "O" for i in range(span[0], span[1])):
                 pred_labels_per_tokens[span[0]] = "B-" + id2label[pred_label]
                 pred_labels_per_tokens[span[0] + 1 : span[1]] = ["I-" + id2label[pred_label]] * (span[1] - span[0] - 1)
 
         seqeval.add(prediction=pred_labels_per_tokens, reference=gold_labels_per_tokens)
 
-    results = seqeval.compute()
+    with warnings.catch_warnings():
+        warnings.simplefilter("ignore", UndefinedMetricWarning)
+        results = seqeval.compute()
     # `results` also contains e.g. "person-athlete": {'precision': 0.5982658959537572, 'recall': 0.9, 'f1': 0.71875, 'number': 230}
     # logging this all is overkill. Tensorboard doesn't even support it, WandB does, but it's not very useful generally.
     # I'd like to revisit this to expose this information somehow still
     return {key: value for key, value in results.items() if isinstance(value, float)}
```

### Comparing `span_marker-0.2.2/span_marker/modeling.py` & `span_marker-1.0.0/span_marker/modeling.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,33 @@
+import logging
 import os
+import re
+import warnings
 from typing import Callable, Dict, List, Optional, Type, TypeVar, Union
 
 import torch
-from torch import nn
+import torch.nn.functional as F
+from packaging.version import Version, parse
+from torch import device, nn
 from transformers import AutoConfig, AutoModel, PretrainedConfig, PreTrainedModel
+from typing_extensions import Self
 
 from span_marker import __version__ as span_marker_version
 from span_marker.configuration import SpanMarkerConfig
 from span_marker.data_collator import SpanMarkerDataCollator
-from span_marker.model_card import MODEL_CARD_TEMPLATE
+from span_marker.model_card import MODEL_CARD_TEMPLATE, generate_model_card
 from span_marker.output import SpanMarkerOutput
 from span_marker.tokenizer import SpanMarkerTokenizer
 
+logger = logging.getLogger(__name__)
+
 T = TypeVar("T", bound="SpanMarkerModel")
 
+UNEXPECTED_KEYWORD_PATTERN = re.compile("\S+ got an unexpected keyword argument '([^']*)'")
+
 
 class SpanMarkerModel(PreTrainedModel):
     """
     This SpanMarker model allows for Named Entity Recognition (NER) using a variety of underlying encoders,
     such as BERT and RoBERTa. The model should be initialized using :meth:`~SpanMarkerModel.from_pretrained`,
     e.g. like so:
 
@@ -34,15 +44,24 @@
      {'span': 'Marek', 'label': 'person-other', 'score': 0.9100819230079651, 'char_start_index': 99, 'char_end_index': 104},
      {'span': 'Aston Martin DB7', 'label': 'product-car', 'score': 0.9931442737579346, 'char_start_index': 143, 'char_end_index': 159}]
     """
 
     config_class = SpanMarkerConfig
     base_model_prefix = "encoder"
 
-    def __init__(self, config: SpanMarkerConfig, encoder=None, **kwargs) -> None:
+    def __init__(self, config: SpanMarkerConfig, encoder: Optional[PreTrainedModel] = None, **kwargs) -> None:
+        """Initialize a SpanMarkerModel using configuration.
+
+        Do not manually initialize a SpanMarkerModel this way! Use :meth:`~SpanMarkerModel.from_pretrained` instead.
+
+        Args:
+            config (SpanMarkerConfig): The configuration for this model.
+            encoder (Optional[PreTrainedModel]): A PreTrainedModel acting as the underlying encoder.
+                Defaults to None.
+        """
         super().__init__(config)
         self.config = config
         # `encoder` will be specified if this Model is initializer via .from_pretrained with an encoder
         # If .from_pretrained is called with a SpanMarkerModel instance, then we use the "traditional"
         # PreTrainedModel.from_pretrained, which won't include an encoder keyword argument. In that case,
         # we must create an "empty" encoder for PreTrainedModel.from_pretrained to fill with the correct
         # weights.
@@ -91,54 +110,68 @@
             module.bias.data.zero_()
 
     def forward(
         self,
         input_ids: torch.Tensor,
         attention_mask: torch.Tensor,
         position_ids: torch.Tensor,
+        start_marker_indices: torch.Tensor,
+        num_marker_pairs: torch.Tensor,
         labels: Optional[torch.Tensor] = None,
         num_words: Optional[torch.Tensor] = None,
     ) -> SpanMarkerOutput:
         """Forward call of the SpanMarkerModel.
 
         Args:
-            input_ids (torch.Tensor): Input IDs including start/end markers.
-            attention_mask (torch.Tensor): Attention mask matrix including one-directional attention for markers.
-            position_ids (torch.Tensor): Position IDs including start/end markers.
-            labels (Optional[torch.Tensor], optional): The labels for each span candidate. Defaults to None.
-            num_words (Optional[torch.Tensor], optional): The number of words for each batch sample. Defaults to None.
+            input_ids (~torch.Tensor): Input IDs including start/end markers.
+            attention_mask (~torch.Tensor): Attention mask matrix including one-directional attention for markers.
+            position_ids (~torch.Tensor): Position IDs including start/end markers.
+            start_marker_indices (~torch.Tensor): The indices where the start markers begin per batch sample.
+            num_marker_pairs (~torch.Tensor): The number of start/end marker pairs per batch sample.
+            labels (Optional[~torch.Tensor]): The labels for each span candidate. Defaults to None.
+            num_words (Optional[~torch.Tensor]): The number of words for each batch sample. Defaults to None.
 
         Returns:
             SpanMarkerOutput: The output dataclass.
         """
         token_type_ids = torch.zeros_like(input_ids)
         outputs = self.encoder(
             input_ids,
             attention_mask=attention_mask,
             token_type_ids=token_type_ids,
             position_ids=position_ids,
         )
         last_hidden_state = outputs[0]
         last_hidden_state = self.dropout(last_hidden_state)
 
+        batch_size = last_hidden_state.size(0)
         sequence_length = last_hidden_state.size(1)
-        start_marker_idx = sequence_length - 2 * self.config.marker_max_length
-        end_marker_idx = start_marker_idx + self.config.marker_max_length
-        # TODO: Can we use view, which may be more efficient?
-        # Answer: Yes, but only if we move to using start-end-...-start-end instead
-        # of start-start-...-end-end.
-
-        # The start marker embeddings concatenated with the end marker embeddings
-        feature_vector = torch.cat(
-            (
-                last_hidden_state[:, start_marker_idx:end_marker_idx],
-                last_hidden_state[:, end_marker_idx:],
-            ),
-            dim=-1,
-        )
+
+        # Get the indices where the end markers start
+        end_marker_indices = start_marker_indices + num_marker_pairs
+
+        # The start marker embeddings concatenated with the end marker embeddings.
+        # This is kind of breaking the cardinal rule of GPU-based ML, as this is processing
+        # the batch iteratively per sample, but every sample produces a different shape matrix
+        # and this is the most convenient way to recombine them into a matrix.
+        embeddings = [
+            torch.cat(
+                (
+                    last_hidden_state[i, start_marker_indices[i] : end_marker_indices[i]],
+                    last_hidden_state[i, end_marker_indices[i] : end_marker_indices[i] + num_marker_pairs[i]],
+                ),
+                dim=-1,
+            )
+            for i in range(batch_size)
+        ]
+        padded_embeddings = [
+            F.pad(embedding, (0, 0, 0, sequence_length // 2 - len(embedding))) for embedding in embeddings
+        ]
+        feature_vector = torch.stack(padded_embeddings)
+
         # NOTE: This was wrong in the older tests
         feature_vector = self.dropout(feature_vector)
         logits = self.classifier(feature_vector)
 
         if labels is not None:
             loss = self.loss_func(logits.view(-1, self.config.num_labels), labels.view(-1))
 
@@ -161,52 +194,62 @@
             >>> # Initialize a SpanMarkerModel using a pretrained encoder
             >>> model = SpanMarkerModel.from_pretrained("bert-base-cased", labels=["O", "B-PER", "I-PER", "B-ORG", "I-ORG", ...])
             >>> # Load a pretrained SpanMarker model
             >>> model = SpanMarkerModel.from_pretrained("tomaarsen/span-marker-bert-base-fewnerd-fine-super")
 
         Args:
             pretrained_model_name_or_path (Union[str, os.PathLike]):
-                Either a pretrained encoder (e.g. `bert-base-cased`, `roberta-large`, etc.), or a pretrained SpanMarkerModel.
+                Either a pretrained encoder (e.g. ``bert-base-cased``, ``roberta-large``, etc.), or a pretrained SpanMarkerModel.
                 Can be either:
 
                     - A string, the *model id* of a pretrained model hosted inside a model repo on huggingface.co.
-                      Valid model ids can be located at the root-level, like `bert-base-uncased`, or namespaced under a
-                      user or organization name, like `dbmdz/bert-base-german-cased`.
+                      Valid model ids can be located at the root-level, like ``bert-base-uncased``, or namespaced under a
+                      user or organization name, like ``dbmdz/bert-base-german-cased``.
                     - A path to a *directory* containing model weights saved using
-                      `.save_pretrained`, e.g., `./my_model_directory/`.
-                    - A path or url to a *tensorflow index checkpoint file* (e.g, `./tf_model/model.ckpt.index`). In
-                      this case, `from_tf` should be set to `True` and a configuration object should be provided as
-                      `config` argument. This loading path is slower than converting the TensorFlow checkpoint in a
+                      :meth:`SpanMarkerModel.save_pretrained`, e.g., ``./my_model_directory/``.
+                    - A path or url to a *tensorflow index checkpoint file* (e.g, ``./tf_model/model.ckpt.index``). In
+                      this case, ``from_tf`` should be set to ``True`` and a configuration object should be provided as
+                      ``config`` argument. This loading path is slower than converting the TensorFlow checkpoint in a
                       PyTorch model using the provided conversion scripts and loading the PyTorch model afterwards.
                     - A path or url to a model folder containing a *flax checkpoint file* in *.msgpack* format (e.g,
-                      `./flax_model/` containing `flax_model.msgpack`). In this case, `from_flax` should be set to
-                      `True`.
+                      ``./flax_model/`` containing ``flax_model.msgpack``). In this case, ``from_flax`` should be set to
+                      ``True``.
 
-            labels (List[str], optional): A list of string labels corresponding to the `ner_tags` in your datasets.
+            labels (List[str], optional): A list of string labels corresponding to the ``ner_tags`` in your datasets.
                 Only necessary when loading a SpanMarker model using a pretrained encoder. Defaults to None.
 
-        Additional arguments are passed to the `from_pretrained` methods of `AutoConfig`, `AutoModel` and
-        `SpanMarkerTokenizer`.
+        Additional arguments are passed to :class:`~span_marker.configuration.SpanMarkerConfig` and the ``from_pretrained`` methods of
+        :class:`~transformers.AutoConfig`, :class:`~transformers.AutoModel` and :class:`~span_marker.tokenizer.SpanMarkerTokenizer`.
 
         Returns:
-            SpanMarkerModel: A SpanMarkerModel instance, either ready for training using the `Trainer` or for
-                inference via `model.predict()`.
+            SpanMarkerModel: A :class:`SpanMarkerModel` instance, either ready for training using the :class:`Trainer` or\
+                for inference via :meth:`SpanMarkerModel.predict`.
         """
         # If loading a SpanMarkerConfig, then we don't want to override id2label and label2id
         # Create an encoder or SpanMarker config
         config: PretrainedConfig = AutoConfig.from_pretrained(pretrained_model_name_or_path, *model_args, **kwargs)
 
         # if 'pretrained_model_name_or_path' refers to a SpanMarkerModel instance, initialize it directly
         if isinstance(config, cls.config_class):
+            model_span_marker_version = config.get("span_marker_version") or "0.1.0"
+            if parse(model_span_marker_version) < Version("1.0.0.dev"):
+                logger.warning(
+                    f"Loading a model trained using SpanMarker v{model_span_marker_version},"
+                    f" while SpanMarker v{span_marker_version} is installed. Due to large changes"
+                    " introduced in v1.0.0, this is not recommended. Either retrain your model for"
+                    f" v{span_marker_version}, or install `span_marker < 1.0.0`."
+                )
             model = super().from_pretrained(pretrained_model_name_or_path, *model_args, config=config, **kwargs)
 
         # If 'pretrained_model_name_or_path' refers to an encoder (roberta, bert, distilbert, electra, etc.),
         # then initialize it and create the SpanMarker config and model using the encoder and its config.
         else:
-            encoder = AutoModel.from_pretrained(pretrained_model_name_or_path, *model_args, config=config)
+            encoder = SpanMarkerModel._load_encoder_with_kwargs(
+                pretrained_model_name_or_path, config, *model_args, **kwargs.copy()
+            )
             if labels is None:
                 raise ValueError(
                     "Please provide a `labels` list to `SpanMarkerModel.from_pretrained()`, e.g.\n"
                     ">>> SpanMarkerModel.from_pretrained(\n"
                     f'...     "{pretrained_model_name_or_path}",\n'
                     '...     labels=["O", "B-PER", "I-PER", "B-ORG", "I-ORG", ...]\n'
                     "... )\n"
@@ -230,20 +273,53 @@
             config.encoder.get("_name_or_path", pretrained_model_name_or_path), config=config, **kwargs
         )
         model.set_tokenizer(tokenizer)
         model.resize_token_embeddings(len(tokenizer))
 
         return model
 
+    @classmethod
+    def _load_encoder_with_kwargs(
+        cls, pretrained_model_name_or_path: str, config: PretrainedConfig, *model_args, **kwargs
+    ) -> PreTrainedModel:
+        """Load an underlying encoder using keyword arguments, even if those kwargs are not (all) supported.
+
+        Args:
+            pretrained_model_name_or_path (str): The model name or path, e.g. ``bert-base-cased``.
+            config (PretrainedConfig): The config corresponding with the encoder.
+
+        Returns:
+            PreTrainedModel: The loaded encoder.
+        """
+        try:
+            return AutoModel.from_pretrained(
+                pretrained_model_name_or_path,
+                *model_args,
+                config=config,
+                **kwargs,
+            )
+        except TypeError as exc:
+            # If we can find a specific keyword that is causing issues, remove it and try again
+            match = UNEXPECTED_KEYWORD_PATTERN.search(str(exc))
+            if match:
+                problematic_keyword = match.group(1)
+                if problematic_keyword in kwargs:
+                    kwargs.pop(problematic_keyword)
+                    return SpanMarkerModel._load_encoder_with_kwargs(
+                        pretrained_model_name_or_path, config, *model_args, **kwargs
+                    )
+            # Otherwise, just raise the exception
+            raise exc
+
     def predict(
         self, inputs: Union[str, List[str], List[List[str]]], allow_overlapping: bool = False
     ) -> Union[List[Dict[str, Union[str, int, float]]], List[List[Dict[str, Union[str, int, float]]]]]:
         """Predict named entities from input texts.
 
-        Example:
+        Example::
 
             >>> model = SpanMarkerModel.from_pretrained(...)
             >>> model.predict("Amelia Earhart flew her single engine Lockheed Vega 5B across the Atlantic to Paris.")
             [{'span': 'Amelia Earhart', 'label': 'person-other', 'score': 0.7629689574241638, 'char_start_index': 0, 'char_end_index': 14},
              {'span': 'Lockheed Vega 5B', 'label': 'product-airplane', 'score': 0.9833564758300781, 'char_start_index': 38, 'char_end_index': 54},
              {'span': 'Atlantic', 'label': 'location-bodiesofwater', 'score': 0.7621214389801025, 'char_start_index': 66, 'char_end_index': 74},
              {'span': 'Paris', 'label': 'location-GPE', 'score': 0.9807717204093933, 'char_start_index': 78, 'char_end_index': 83}]
@@ -265,24 +341,33 @@
                 have good support for this, so False is recommended. Defaults to False.
 
         Returns:
             Union[List[Dict[str, Union[str, int, float]]], List[List[Dict[str, Union[str, int, float]]]]]:
                 If the input is a single sentence, then we output a list of dictionaries. Each dictionary
                 represents one predicted entity, and contains the following keys:
 
-                * `label`: The predicted entity label.
-                * `span`: The text that the model deems an entity.
-                * `score`: The model its confidence.
-                * `word_start_index` & `word_end_index`: The word indices for the start/end of the entity,
+                * ``label``: The predicted entity label.
+                * ``span``: The text that the model deems an entity.
+                * ``score``: The model its confidence.
+                * ``word_start_index`` & ``word_end_index``: The word indices for the start/end of the entity,
                   if the input is pre-tokenized.
-                * `char_start_index` & `char_end_index`: The character indices for the start/end of the entity,
+                * ``char_start_index`` & ``char_end_index``: The character indices for the start/end of the entity,
                   if the input is a string.
 
                 If the input is multiple sentences, then we return a list containing multiple of the aforementioned lists.
         """
+        if torch.cuda.is_available() and self.device == torch.device("cpu"):
+            warnings.warn(
+                "SpanMarker model predictions are being computed on the CPU while CUDA is available."
+                " Moving the model to CUDA using `model.cuda()` before performing predictions is heavily"
+                " recommended to significantly boost prediction speeds.",
+                UserWarning,
+                stacklevel=2,
+            )
+
         if not inputs:
             return []
 
         # Check if inputs is a string, i.e. a string sentence, or
         # if it is a list of strings without spaces, i.e. if it's 1 tokenized sentence
         if isinstance(inputs, str) or (
             isinstance(inputs, list) and all(isinstance(element, str) and " " not in element for element in inputs)
@@ -388,16 +473,27 @@
             save_function=save_function,
             push_to_hub=push_to_hub,
             max_shard_size=max_shard_size,
             safe_serialization=safe_serialization,
             variant=variant,
             **kwargs,
         )
-        if "_name_or_path" in self.config.encoder:
-            encoder_name_or_path = repr(self.config.encoder["_name_or_path"])
-        else:
-            encoder_name_or_path = "an unknown model"
-        model_card_content = MODEL_CARD_TEMPLATE.format(
-            model_name=save_directory, encoder_name_or_path=encoder_name_or_path
-        )
         with open(os.path.join(save_directory, "README.md"), "w", encoding="utf-8") as f:
-            f.write(model_card_content)
+            f.write(generate_model_card(save_directory, self.config))
+
+    def try_cuda(self, device: Optional[Union[int, device]] = None) -> Self:
+        """Try to moves all model parameters and buffers to the GPU, do nothing if failed.
+
+        .. note::
+            This method modifies the module in-place.
+
+        Args:
+            device (int, optional): if specified, all parameters will be
+                copied to that device
+
+        Returns:
+            Module: self
+        """
+        try:
+            return self.cuda(device)
+        except (AssertionError, RuntimeError):
+            return self
```

### Comparing `span_marker-0.2.2/span_marker/output.py` & `span_marker-1.0.0/span_marker/output.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,31 +4,32 @@
 import torch
 from transformers.modeling_outputs import TokenClassifierOutput
 
 
 @dataclass
 class SpanMarkerOutput(TokenClassifierOutput):
     """
-    Class for outputs of SpanMarker models.
+    Class for outputs of :class:`~span_marker.modeling.SpanMarkerModel`.
 
     Args:
-        loss (`torch.FloatTensor` of shape `(1,)`, *optional*, returned when `labels` is provided):
-            Classification loss.
-        logits (`torch.FloatTensor` of shape `(batch_size, sequence_length, config.num_labels)`):
-            Classification scores (before SoftMax).
-        hidden_states (`tuple(torch.FloatTensor)`, *optional*, returned when `config.output_hidden_states=True`):
-            Tuple of `torch.FloatTensor` (one for the output of the embeddings, if the model has an embedding layer, +
-            one for the output of each layer) of shape `(batch_size, sequence_length, hidden_size)`.
+        loss (Optional[torch.FloatTensor]):
+            Classification loss of shape ``(1,)``, returned when ``labels`` is provided.
+        logits (torch.FloatTensor):
+            Classification scores before softmax with shape ``(batch_size, sequence_length, config.num_labels)``.
+        hidden_states (Optional[Tuple[torch.FloatTensor]]):
+            Tuple of :class:`~torch.FloatTensor` (one for the output of the embeddings, if the model has an embedding layer, +
+            one for the output of each layer) of shape ``(batch_size, sequence_length, hidden_size)``.
+            Returned when ``config.output_hidden_states=True``.
 
             Hidden-states of the model at the output of each layer plus the optional initial embedding outputs.
-        attentions (`tuple(torch.FloatTensor)`, *optional*, returned when `config.output_attentions=True`):
-            Tuple of `torch.FloatTensor` (one for each layer) of shape `(batch_size, num_heads, sequence_length,
-            sequence_length)`.
+        attentions (Optional[Tuple[torch.FloatTensor]]):
+            Tuple of :class:`~torch.FloatTensor` (one for each layer) of shape ``(batch_size, num_heads, sequence_length,
+            sequence_length)``. Returned when ``config.output_attentions=True``.
 
             Attentions weights after the attention softmax, used to compute the weighted average in the self-attention
             heads.
-        num_words (`torch.Tensor`, *optional*):
-            A vector with length `batch_size` that tracks how many words were in the input of each sample in the batch.
+        num_words (Optional[~torch.Tensor]):
+            A vector with shape ``(batch_size,)`` that tracks how many words were in the input of each sample in the batch.
             Required for evaluation purposes.
     """
 
     num_words: Optional[torch.Tensor] = None
```

### Comparing `span_marker-0.2.2/span_marker/trainer.py` & `span_marker-1.0.0/span_marker/trainer.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import warnings
+import logging
 from typing import Callable, Dict, List, Optional, Tuple
 
 import torch
 from datasets import Dataset
 from torch.utils.data import DataLoader
 from transformers import (
     EvalPrediction,
@@ -13,69 +13,71 @@
 from transformers.trainer_utils import PredictionOutput
 
 from span_marker.evaluation import compute_f1_via_seqeval
 from span_marker.label_normalizer import AutoLabelNormalizer, LabelNormalizer
 from span_marker.modeling import SpanMarkerModel
 from span_marker.tokenizer import SpanMarkerTokenizer
 
+logger = logging.getLogger(__name__)
+
 
 class Trainer(TransformersTrainer):
     """
     Trainer is a simple but feature-complete training and eval loop for SpanMarker,
-    built tightly on top of the 🤗 Transformers `Trainer <https://huggingface.co/docs/transformers/main_classes/trainer>`_.
+    built tightly on top of the 🤗 Transformers :external:doc:`Trainer <main_classes/trainer>`.
 
     Args:
         model (Optional[SpanMarkerModel]):
-            The model to train, evaluate or use for predictions. If not provided, a `model_init` must be passed.
-        args (Optional[TrainingArguments]):
-            The arguments to tweak for training. Will default to a basic instance of [`TrainingArguments`] with the
-            `output_dir` set to a directory named *tmp_trainer* in the current directory if not provided.
-        train_dataset (Optional[datasets.Dataset]):
+            The model to train, evaluate or use for predictions. If not provided, a ``model_init`` must be passed.
+        args (Optional[~transformers.TrainingArguments]):
+            The arguments to tweak for training. Will default to a basic instance of :class:`~transformers.TrainingArguments` with the
+            ``output_dir`` set to a directory named *models/my_span_marker_model* in the current directory if not provided.
+        train_dataset (Optional[~datasets.Dataset]):
             The dataset to use for training.
-        eval_dataset (Optional[datasets.Dataset]):
+        eval_dataset (Optional[~datasets.Dataset]):
              The dataset to use for evaluation.
         model_init (Optional[Callable[[], SpanMarkerModel]]):
-            A function that instantiates the model to be used. If provided, each call to `Trainer.train` will start
+            A function that instantiates the model to be used. If provided, each call to :meth:`Trainer.train` will start
             from a new instance of the model as given by this function.
 
             The function may have zero argument, or a single one containing the optuna/Ray Tune/SigOpt trial object, to
             be able to choose different architectures according to hyper parameters (such as layer count, sizes of
             inner layers, dropout probabilities etc).
-        compute_metrics (Optional[Callable[[EvalPrediction], Dict]]):
-            The function that will be used to compute metrics at evaluation. Must take a [`EvalPrediction`] and return
+        compute_metrics (Optional[Callable[[~transformers.EvalPrediction], Dict]]):
+            The function that will be used to compute metrics at evaluation. Must take a :class:`~transformers.EvalPrediction` and return
             a dictionary string to metric values.
-        callbacks (Optional[List[TrainerCallback]]):
+        callbacks (Optional[List[~transformers.TrainerCallback]]):
             A list of callbacks to customize the training loop. Will add those to the list of default callbacks
-            detailed in [here](https://huggingface.co/docs/transformers/main/en/main_classes/callback).
+            detailed in the Hugging Face :external:doc:`Callback documentation <main_classes/callback>`.
 
-            If you want to remove one of the default callbacks used, use the [`Trainer.remove_callback`] method.
-        optimizers (Tuple[Optional[torch.optim.Optimizer], Optional[torch.optim.lr_scheduler.LambdaLR]]): A tuple
-            containing the optimizer and the scheduler to use. Will default to an instance of `AdamW` on your model
-            and a scheduler given by `get_linear_schedule_with_warmup` controlled by `args`.
-        preprocess_logits_for_metrics (Optional[Callable[[torch.Tensor, torch.Tensor], torch.Tensor]]):
+            If you want to remove one of the default callbacks used, use the :meth:`~Trainer.remove_callback` method.
+        optimizers (Tuple[Optional[~torch.optim.Optimizer], Optional[~torch.optim.lr_scheduler.LambdaLR]]): A tuple
+            containing the optimizer and the scheduler to use. Will default to an instance of ``AdamW`` on your model
+            and a scheduler given by ``get_linear_schedule_with_warmup`` controlled by ``args``.
+        preprocess_logits_for_metrics (Optional[Callable[[~torch.Tensor, ~torch.Tensor], ~torch.Tensor]]):
             A function that preprocess the logits right before caching them at each evaluation step. Must take two
             tensors, the logits and the labels, and return the logits once processed as desired. The modifications made
-            by this function will be reflected in the predictions received by `compute_metrics`.
+            by this function will be reflected in the predictions received by ``compute_metrics``.
 
-            Note that the labels (second parameter) will be `None` if the dataset does not have them.
+            Note that the labels (second parameter) will be ``None`` if the dataset does not have them.
 
     Important attributes:
 
         - **model** -- Always points to the core model.
         - **model_wrapped** -- Always points to the most external model in case one or more other modules wrap the
-          original model. This is the model that should be used for the forward pass. For example, under `DeepSpeed`,
-          the inner model is wrapped in `DeepSpeed` and then again in `torch.nn.DistributedDataParallel`. If the inner
-          model hasn't been wrapped, then `self.model_wrapped` is the same as `self.model`.
+          original model. This is the model that should be used for the forward pass. For example, under ``DeepSpeed``,
+          the inner model is wrapped in ``DeepSpeed`` and then again in :class:`torch.nn.DistributedDataParallel`. If the
+          inner model hasn't been wrapped, then ``self.model_wrapped`` is the same as ``self.model``.
         - **is_model_parallel** -- Whether or not a model has been switched to a model parallel mode (different from
           data parallelism, this means some of the model layers are split on different GPUs).
         - **place_model_on_device** -- Whether or not to automatically place the model on the device - it will be set
-          to `False` if model parallel or deepspeed is used, or if the default
-          `TrainingArguments.place_model_on_device` is overridden to return `False` .
-        - **is_in_train** -- Whether or not a model is currently running `train` (e.g. when `evaluate` is called while
-          in `train`)
+          to ``False`` if model parallel or deepspeed is used, or if the default
+          `TrainingArguments.place_model_on_device` is overridden to return ``False``.
+        - **is_in_train** -- Whether or not a model is currently running :meth:`~Trainer.train` (e.g. when ``evaluate`` is called while
+          in ``train``)
     """
 
     def __init__(
         self,
         model: Optional[SpanMarkerModel] = None,
         args: Optional[TrainingArguments] = None,
         train_dataset: Optional[Dataset] = None,
@@ -132,49 +134,49 @@
         self,
         dataset: Dataset,
         label_normalizer: LabelNormalizer,
         tokenizer: SpanMarkerTokenizer,
         dataset_name: str = "train",
         is_evaluate: bool = False,
     ) -> Dataset:
-        """Normalize the `ner_tags` labels and call tokenizer on `tokens`.
+        """Normalize the ``ner_tags`` labels and call tokenizer on ``tokens``.
 
         Args:
-            dataset (Dataset): A Hugging Face dataset with `tokens` and `ner_tags` columns.
-            label_normalizer (LabelNormalizer): A callable that normalizes `ner_tags` into start-end-label tuples.
-            tokenizer (SpanMarkerTokenizer): The tokenizer responsible for tokenizing `tokens` into input IDs,
+            dataset (~datasets.Dataset): A Hugging Face dataset with ``tokens`` and ``ner_tags`` columns.
+            label_normalizer (LabelNormalizer): A callable that normalizes ``ner_tags`` into start-end-label tuples.
+            tokenizer (SpanMarkerTokenizer): The tokenizer responsible for tokenizing ``tokens`` into input IDs,
                 and adding start and end markers.
             dataset_name (str, optional): The name of the dataset. Defaults to "train".
             is_evaluate (bool, optional): Whether to return the number of words for each sample.
                 Required for evaluation. Defaults to False.
 
         Raises:
-            ValueError: If the `dataset` does not contain `tokens` and `ner_tags` columns.
+            ValueError: If the ``dataset`` does not contain ``tokens`` and ``ner_tags`` columns.
 
         Returns:
             Dataset: The normalized and tokenized version of the input dataset.
         """
         for column in ("tokens", "ner_tags"):
             if column not in dataset.column_names:
                 raise ValueError(f"The {dataset_name} dataset must contain a {column!r} column.")
 
         # Normalize the labels to a common format (list of label-start-end tuples)
         dataset = dataset.map(
             label_normalizer,
-            input_columns="ner_tags",
-            batched=True,
+            input_columns=("tokens", "ner_tags"),
             desc=f"Label normalizing the {dataset_name} dataset",
         )
         # Tokenize and add start/end markers
-        dataset = dataset.map(
-            lambda batch: tokenizer(batch["tokens"], labels=batch["ner_tags"], return_num_words=is_evaluate),
-            batched=True,
-            remove_columns=dataset.column_names,
-            desc=f"Tokenizing the {dataset_name} dataset",
-        )
+        with tokenizer.entity_tracker(split=dataset_name):
+            dataset = dataset.map(
+                lambda batch: tokenizer(batch["tokens"], labels=batch["ner_tags"], return_num_words=is_evaluate),
+                batched=True,
+                remove_columns=dataset.column_names,
+                desc=f"Tokenizing the {dataset_name} dataset",
+            )
         return dataset
 
     def get_train_dataloader(self) -> DataLoader:
         """Return the preprocessed training DataLoader."""
         self.train_dataset = self.preprocess_dataset(self.train_dataset, self.label_normalizer, self.tokenizer)
         return super().get_train_dataloader()
 
@@ -193,14 +195,12 @@
             test_dataset, self.label_normalizer, self.tokenizer, dataset_name="test", is_evaluate=True
         )
         return super().get_test_dataloader(test_dataset)
 
     def predict(
         self, test_dataset: Dataset, ignore_keys: Optional[List[str]] = None, metric_key_prefix: str = "test"
     ) -> PredictionOutput:
-        warnings.warn(
+        logger.warning(
             f"`Trainer.predict` is not recommended for a {self.model.__class__.__name__}. "
-            f"Consider using `{self.model.__class__.__name__}.predict` instead.",
-            UserWarning,
-            stacklevel=2,
+            f"Consider using `{self.model.__class__.__name__}.predict` instead."
         )
         return super().predict(test_dataset, ignore_keys, metric_key_prefix)
```

### Comparing `span_marker-0.2.2/span_marker.egg-info/SOURCES.txt` & `span_marker-1.0.0/span_marker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `span_marker-0.2.2/tests/test_configuration.py` & `span_marker-1.0.0/tests/test_configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,13 +10,13 @@
     with pytest.raises(ValueError, match=re.escape("'O' label")):
         SpanMarkerModel.from_pretrained(TINY_BERT, labels=["person", "location", "misc"])
 
 
 def test_config_get_default(finetuned_conll_span_marker_model: SpanMarkerModel) -> None:
     config = finetuned_conll_span_marker_model.config
     # Verify that we can fetch directly from top-level SpanMarkerConfig
-    assert config.get("marker_max_length") == 256
+    assert config.get("marker_max_length") == 128
     # Verify that we can fetch from the underlying encoder, even with multiple options
     assert config.get("hidden_dropout_prob") == 0.1
     assert config.get(["dropout_rate", "hidden_dropout_prob"]) == 0.1
     # Verify that we get the default if the config value does not exist
     assert config.get(["does_not_exist", "also_does_not_exist"], default=12) == 12
```

### Comparing `span_marker-0.2.2/tests/test_modeling.py` & `span_marker-1.0.0/tests/test_modeling.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import re
 from typing import Dict, List, Optional, Union
 
 import pytest
+import torch
 
 from span_marker.configuration import SpanMarkerConfig
 from span_marker.modeling import SpanMarkerModel
 from span_marker.tokenizer import SpanMarkerTokenizer
 from tests.constants import CONLL_LABELS, FEWNERD_COARSE_LABELS, TINY_BERT
 from tests.helpers import compare_entities
 
@@ -84,7 +85,35 @@
     pred_entities = model.predict(inputs)
     compare_entities(pred_entities, gold_entities)
 
     # Multiple sentences
     pred_entity_list = model.predict([inputs] * 3)
     for pred_entities in pred_entity_list:
         compare_entities(pred_entities, gold_entities)
+
+
+@pytest.mark.parametrize(
+    "kwargs",
+    [
+        # Reasonable kwargs that will be used by SpanMarkerConfig
+        {
+            "model_max_length": 256,
+            "marker_max_length": 128,
+            "entity_max_length": 8,
+        },
+        # Kwargs that will be used by from_pretrained of the Encoder
+        {"low_cpu_mem_usage": True},
+        # Completely arbitrary kwargs that should be discarded/ignored
+        {"this_is_completely_unused_I_hope": True},
+    ],
+)
+def test_load_with_kwargs(kwargs) -> None:
+    # We only test that the model can be loaded without issues
+    model = SpanMarkerModel.from_pretrained(TINY_BERT, labels=CONLL_LABELS, kwargs=kwargs)
+    assert isinstance(model, SpanMarkerModel)
+
+
+def test_try_cuda(finetuned_conll_span_marker_model: SpanMarkerModel) -> None:
+    # This should not crash, regardless of whether Torch is compiled with CUDA or not
+    finetuned_conll_span_marker_model.try_cuda()
+    # The model is on CUDA if CUDA is available, and not on CUDA if CUDA is not available.
+    assert (finetuned_conll_span_marker_model.device.type == "cuda") == torch.cuda.is_available()
```

