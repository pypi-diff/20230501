# Comparing `tmp/batdetect2-1.0.2.tar.gz` & `tmp/batdetect2-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "batdetect2-1.0.2.tar", last modified: Sat Apr 29 15:11:02 2023, max compression
+gzip compressed data, was "batdetect2-1.0.3.tar", last modified: Mon May  1 14:21:04 2023, max compression
```

## Comparing `batdetect2-1.0.2.tar` & `batdetect2-1.0.3.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0    17694 2023-04-29 15:10:53.237251 batdetect2-1.0.2/LICENSE.md
--rw-r--r--   0        0        0     5584 2023-04-29 15:10:53.237251 batdetect2-1.0.2/README.md
--rw-r--r--   0        0        0       22 2023-04-29 15:10:53.237251 batdetect2-1.0.2/batdetect2/__init__.py
--rw-r--r--   0        0        0    12537 2023-04-29 15:10:53.237251 batdetect2-1.0.2/batdetect2/api.py
--rw-r--r--   0        0        0     3522 2023-04-29 15:10:53.237251 batdetect2-1.0.2/batdetect2/cli.py
--rw-r--r--   0        0        0        0 2023-04-29 15:10:53.237251 batdetect2-1.0.2/batdetect2/detector/__init__.py
--rw-r--r--   0        0        0     4225 2023-04-29 15:10:53.237251 batdetect2-1.0.2/batdetect2/detector/compute_features.py
--rw-r--r--   0        0        0     4970 2023-04-29 15:10:53.237251 batdetect2-1.0.2/batdetect2/detector/model_helpers.py
--rw-r--r--   0        0        0    10568 2023-04-29 15:10:53.237251 batdetect2-1.0.2/batdetect2/detector/models.py
--rw-r--r--   0        0        0     7481 2023-04-29 15:10:53.237251 batdetect2-1.0.2/batdetect2/detector/parameters.py
--rw-r--r--   0        0        0     5873 2023-04-29 15:10:53.237251 batdetect2-1.0.2/batdetect2/detector/post_process.py
--rw-r--r--   0        0        0        0 2023-04-29 15:10:53.237251 batdetect2-1.0.2/batdetect2/evaluate/__init__.py
--rw-r--r--   0        0        0    25540 2023-04-29 15:10:53.237251 batdetect2-1.0.2/batdetect2/evaluate/evaluate_models.py
--rw-r--r--   0        0        0     2244 2023-04-29 15:10:53.237251 batdetect2-1.0.2/batdetect2/evaluate/readme.md
--rw-r--r--   0        0        0        0 2023-04-29 15:10:53.237251 batdetect2-1.0.2/batdetect2/finetune/__init__.py
--rw-r--r--   0        0        0     9902 2023-04-29 15:10:53.237251 batdetect2-1.0.2/batdetect2/finetune/finetune_model.py
--rw-r--r--   0        0        0     6324 2023-04-29 15:10:53.237251 batdetect2-1.0.2/batdetect2/finetune/prep_data_finetune.py
--rw-r--r--   0        0        0     3158 2023-04-29 15:10:53.237251 batdetect2-1.0.2/batdetect2/finetune/readme.md
--rw-r--r--   0        0        0  7600690 2023-04-29 15:10:53.285252 batdetect2-1.0.2/batdetect2/models/Net2DFast_UK_same.pth.tar
--rw-r--r--   0        0        0       25 2023-04-29 15:10:53.285252 batdetect2-1.0.2/batdetect2/models/readme.md
--rw-r--r--   0        0        0     9832 2023-04-29 15:10:53.285252 batdetect2-1.0.2/batdetect2/plot.py
--rw-r--r--   0        0        0        0 2023-04-29 15:10:53.285252 batdetect2-1.0.2/batdetect2/train/__init__.py
--rw-r--r--   0        0        0    20543 2023-04-29 15:10:53.285252 batdetect2-1.0.2/batdetect2/train/audio_dataloader.py
--rwxr-xr-x   0        0        0    13217 2023-04-29 15:10:53.285252 batdetect2-1.0.2/batdetect2/train/evaluate.py
--rw-r--r--   0        0        0     1580 2023-04-29 15:10:53.285252 batdetect2-1.0.2/batdetect2/train/losses.py
--rw-r--r--   0        0        0     1186 2023-04-29 15:10:53.285252 batdetect2-1.0.2/batdetect2/train/readme.md
--rw-r--r--   0        0        0    17515 2023-04-29 15:10:53.289252 batdetect2-1.0.2/batdetect2/train/train_model.py
--rw-r--r--   0        0        0    12533 2023-04-29 15:10:53.289252 batdetect2-1.0.2/batdetect2/train/train_split.py
--rw-r--r--   0        0        0     5961 2023-04-29 15:10:53.289252 batdetect2-1.0.2/batdetect2/train/train_utils.py
--rw-r--r--   0        0        0    11150 2023-04-29 15:10:53.289252 batdetect2-1.0.2/batdetect2/types.py
--rw-r--r--   0        0        0        0 2023-04-29 15:10:53.289252 batdetect2-1.0.2/batdetect2/utils/__init__.py
--rw-r--r--   0        0        0     8455 2023-04-29 15:10:53.289252 batdetect2-1.0.2/batdetect2/utils/audio_utils.py
--rw-r--r--   0        0        0    23308 2023-04-29 15:10:53.289252 batdetect2-1.0.2/batdetect2/utils/detector_utils.py
--rw-r--r--   0        0        0    16322 2023-04-29 15:10:53.289252 batdetect2-1.0.2/batdetect2/utils/plot_utils.py
--rw-r--r--   0        0        0     7940 2023-04-29 15:10:53.289252 batdetect2-1.0.2/batdetect2/utils/visualize.py
--rw-r--r--   0        0        0     8059 2023-04-29 15:10:53.289252 batdetect2-1.0.2/batdetect2/utils/wavfile.py
--rw-r--r--   0        0        0     1749 2023-04-29 15:10:53.301252 batdetect2-1.0.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-29 15:10:53.301252 batdetect2-1.0.2/tests/__init__.py
--rw-r--r--   0        0        0     8805 2023-04-29 15:10:53.305252 batdetect2-1.0.2/tests/test_api.py
--rw-r--r--   0        0        0     1223 2023-04-29 15:10:53.305252 batdetect2-1.0.2/tests/test_cli.py
--rw-r--r--   0        0        0     6537 1970-01-01 00:00:00.000000 batdetect2-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0    17694 2023-05-01 14:20:41.934413 batdetect2-1.0.3/LICENSE.md
+-rw-r--r--   0        0        0     5584 2023-05-01 14:20:41.934413 batdetect2-1.0.3/README.md
+-rw-r--r--   0        0        0       22 2023-05-01 14:20:41.934413 batdetect2-1.0.3/batdetect2/__init__.py
+-rw-r--r--   0        0        0    12537 2023-05-01 14:20:41.934413 batdetect2-1.0.3/batdetect2/api.py
+-rw-r--r--   0        0        0     3607 2023-05-01 14:20:41.934413 batdetect2-1.0.3/batdetect2/cli.py
+-rw-r--r--   0        0        0        0 2023-05-01 14:20:41.934413 batdetect2-1.0.3/batdetect2/detector/__init__.py
+-rw-r--r--   0        0        0     4225 2023-05-01 14:20:41.934413 batdetect2-1.0.3/batdetect2/detector/compute_features.py
+-rw-r--r--   0        0        0     4970 2023-05-01 14:20:41.934413 batdetect2-1.0.3/batdetect2/detector/model_helpers.py
+-rw-r--r--   0        0        0    10568 2023-05-01 14:20:41.934413 batdetect2-1.0.3/batdetect2/detector/models.py
+-rw-r--r--   0        0        0     7481 2023-05-01 14:20:41.934413 batdetect2-1.0.3/batdetect2/detector/parameters.py
+-rw-r--r--   0        0        0     5873 2023-05-01 14:20:41.934413 batdetect2-1.0.3/batdetect2/detector/post_process.py
+-rw-r--r--   0        0        0        0 2023-05-01 14:20:41.934413 batdetect2-1.0.3/batdetect2/evaluate/__init__.py
+-rw-r--r--   0        0        0    25540 2023-05-01 14:20:41.934413 batdetect2-1.0.3/batdetect2/evaluate/evaluate_models.py
+-rw-r--r--   0        0        0     2244 2023-05-01 14:20:41.934413 batdetect2-1.0.3/batdetect2/evaluate/readme.md
+-rw-r--r--   0        0        0        0 2023-05-01 14:20:41.934413 batdetect2-1.0.3/batdetect2/finetune/__init__.py
+-rw-r--r--   0        0        0     9902 2023-05-01 14:20:41.934413 batdetect2-1.0.3/batdetect2/finetune/finetune_model.py
+-rw-r--r--   0        0        0     6324 2023-05-01 14:20:41.934413 batdetect2-1.0.3/batdetect2/finetune/prep_data_finetune.py
+-rw-r--r--   0        0        0     3158 2023-05-01 14:20:41.934413 batdetect2-1.0.3/batdetect2/finetune/readme.md
+-rw-r--r--   0        0        0  7600690 2023-05-01 14:20:41.986414 batdetect2-1.0.3/batdetect2/models/Net2DFast_UK_same.pth.tar
+-rw-r--r--   0        0        0       25 2023-05-01 14:20:41.986414 batdetect2-1.0.3/batdetect2/models/readme.md
+-rw-r--r--   0        0        0     9832 2023-05-01 14:20:41.986414 batdetect2-1.0.3/batdetect2/plot.py
+-rw-r--r--   0        0        0        0 2023-05-01 14:20:41.986414 batdetect2-1.0.3/batdetect2/train/__init__.py
+-rw-r--r--   0        0        0    20543 2023-05-01 14:20:41.986414 batdetect2-1.0.3/batdetect2/train/audio_dataloader.py
+-rwxr-xr-x   0        0        0    13217 2023-05-01 14:20:41.986414 batdetect2-1.0.3/batdetect2/train/evaluate.py
+-rw-r--r--   0        0        0     1580 2023-05-01 14:20:41.986414 batdetect2-1.0.3/batdetect2/train/losses.py
+-rw-r--r--   0        0        0     1186 2023-05-01 14:20:41.986414 batdetect2-1.0.3/batdetect2/train/readme.md
+-rw-r--r--   0        0        0    17515 2023-05-01 14:20:41.990414 batdetect2-1.0.3/batdetect2/train/train_model.py
+-rw-r--r--   0        0        0    12533 2023-05-01 14:20:41.990414 batdetect2-1.0.3/batdetect2/train/train_split.py
+-rw-r--r--   0        0        0     5961 2023-05-01 14:20:41.990414 batdetect2-1.0.3/batdetect2/train/train_utils.py
+-rw-r--r--   0        0        0    11150 2023-05-01 14:20:41.990414 batdetect2-1.0.3/batdetect2/types.py
+-rw-r--r--   0        0        0        0 2023-05-01 14:20:41.990414 batdetect2-1.0.3/batdetect2/utils/__init__.py
+-rw-r--r--   0        0        0     8455 2023-05-01 14:20:41.990414 batdetect2-1.0.3/batdetect2/utils/audio_utils.py
+-rw-r--r--   0        0        0    23308 2023-05-01 14:20:41.990414 batdetect2-1.0.3/batdetect2/utils/detector_utils.py
+-rw-r--r--   0        0        0    16322 2023-05-01 14:20:41.990414 batdetect2-1.0.3/batdetect2/utils/plot_utils.py
+-rw-r--r--   0        0        0     7940 2023-05-01 14:20:41.990414 batdetect2-1.0.3/batdetect2/utils/visualize.py
+-rw-r--r--   0        0        0     8059 2023-05-01 14:20:41.990414 batdetect2-1.0.3/batdetect2/utils/wavfile.py
+-rw-r--r--   0        0        0     1749 2023-05-01 14:20:42.002414 batdetect2-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-01 14:20:42.006414 batdetect2-1.0.3/tests/__init__.py
+-rw-r--r--   0        0        0     8805 2023-05-01 14:20:42.006414 batdetect2-1.0.3/tests/test_api.py
+-rw-r--r--   0        0        0     1844 2023-05-01 14:20:42.006414 batdetect2-1.0.3/tests/test_cli.py
+-rw-r--r--   0        0        0     6537 1970-01-01 00:00:00.000000 batdetect2-1.0.3/PKG-INFO
```

### Comparing `batdetect2-1.0.2/LICENSE.md` & `batdetect2-1.0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `batdetect2-1.0.2/README.md` & `batdetect2-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `batdetect2-1.0.2/batdetect2/api.py` & `batdetect2-1.0.3/batdetect2/api.py`

 * *Files identical despite different names*

### Comparing `batdetect2-1.0.2/batdetect2/cli.py` & `batdetect2-1.0.3/batdetect2/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,14 +73,15 @@
     default=DEFAULT_MODEL_PATH,
     help="Path to trained BatDetect2 model",
 )
 def detect(
     audio_dir: str,
     ann_dir: str,
     detection_threshold: float,
+    time_expansion_factor: int,
     **args,
 ):
     """Detect bat calls in files in AUDIO_DIR and save predictions to ANN_DIR.
 
     DETECTION_THRESHOLD is the detection threshold. All predictions with a
     score below this threshold will be discarded. Values between 0 and 1.
 
@@ -99,14 +100,15 @@
     click.echo(f"Number of audio files: {len(files)}")
     click.echo(f"\nSaving results to: {ann_dir}")
 
     config = api.get_config(
         **{
             **params,
             **args,
+            'time_expansion': time_expansion_factor,
             "spec_slices": False,
             "chunk_size": 2,
             "detection_threshold": detection_threshold,
         }
     )
 
     # process files
```

### Comparing `batdetect2-1.0.2/batdetect2/detector/compute_features.py` & `batdetect2-1.0.3/batdetect2/detector/compute_features.py`

 * *Files identical despite different names*

### Comparing `batdetect2-1.0.2/batdetect2/detector/model_helpers.py` & `batdetect2-1.0.3/batdetect2/detector/model_helpers.py`

 * *Files identical despite different names*

### Comparing `batdetect2-1.0.2/batdetect2/detector/models.py` & `batdetect2-1.0.3/batdetect2/detector/models.py`

 * *Files identical despite different names*

### Comparing `batdetect2-1.0.2/batdetect2/detector/parameters.py` & `batdetect2-1.0.3/batdetect2/detector/parameters.py`

 * *Files identical despite different names*

### Comparing `batdetect2-1.0.2/batdetect2/detector/post_process.py` & `batdetect2-1.0.3/batdetect2/detector/post_process.py`

 * *Files identical despite different names*

### Comparing `batdetect2-1.0.2/batdetect2/evaluate/evaluate_models.py` & `batdetect2-1.0.3/batdetect2/evaluate/evaluate_models.py`

 * *Files identical despite different names*

### Comparing `batdetect2-1.0.2/batdetect2/evaluate/readme.md` & `batdetect2-1.0.3/batdetect2/evaluate/readme.md`

 * *Files identical despite different names*

### Comparing `batdetect2-1.0.2/batdetect2/finetune/finetune_model.py` & `batdetect2-1.0.3/batdetect2/finetune/finetune_model.py`

 * *Files identical despite different names*

### Comparing `batdetect2-1.0.2/batdetect2/finetune/prep_data_finetune.py` & `batdetect2-1.0.3/batdetect2/finetune/prep_data_finetune.py`

 * *Files identical despite different names*

### Comparing `batdetect2-1.0.2/batdetect2/finetune/readme.md` & `batdetect2-1.0.3/batdetect2/finetune/readme.md`

 * *Files identical despite different names*

### Comparing `batdetect2-1.0.2/batdetect2/models/Net2DFast_UK_same.pth.tar` & `batdetect2-1.0.3/batdetect2/models/Net2DFast_UK_same.pth.tar`

 * *Files identical despite different names*

### Comparing `batdetect2-1.0.2/batdetect2/plot.py` & `batdetect2-1.0.3/batdetect2/plot.py`

 * *Files identical despite different names*

### Comparing `batdetect2-1.0.2/batdetect2/train/audio_dataloader.py` & `batdetect2-1.0.3/batdetect2/train/audio_dataloader.py`

 * *Files identical despite different names*

### Comparing `batdetect2-1.0.2/batdetect2/train/evaluate.py` & `batdetect2-1.0.3/batdetect2/train/evaluate.py`

 * *Files identical despite different names*

### Comparing `batdetect2-1.0.2/batdetect2/train/losses.py` & `batdetect2-1.0.3/batdetect2/train/losses.py`

 * *Files identical despite different names*

### Comparing `batdetect2-1.0.2/batdetect2/train/readme.md` & `batdetect2-1.0.3/batdetect2/train/readme.md`

 * *Files identical despite different names*

### Comparing `batdetect2-1.0.2/batdetect2/train/train_model.py` & `batdetect2-1.0.3/batdetect2/train/train_model.py`

 * *Files identical despite different names*

### Comparing `batdetect2-1.0.2/batdetect2/train/train_split.py` & `batdetect2-1.0.3/batdetect2/train/train_split.py`

 * *Files identical despite different names*

### Comparing `batdetect2-1.0.2/batdetect2/train/train_utils.py` & `batdetect2-1.0.3/batdetect2/train/train_utils.py`

 * *Files identical despite different names*

### Comparing `batdetect2-1.0.2/batdetect2/types.py` & `batdetect2-1.0.3/batdetect2/types.py`

 * *Files identical despite different names*

### Comparing `batdetect2-1.0.2/batdetect2/utils/audio_utils.py` & `batdetect2-1.0.3/batdetect2/utils/audio_utils.py`

 * *Files identical despite different names*

### Comparing `batdetect2-1.0.2/batdetect2/utils/detector_utils.py` & `batdetect2-1.0.3/batdetect2/utils/detector_utils.py`

 * *Files identical despite different names*

### Comparing `batdetect2-1.0.2/batdetect2/utils/plot_utils.py` & `batdetect2-1.0.3/batdetect2/utils/plot_utils.py`

 * *Files identical despite different names*

### Comparing `batdetect2-1.0.2/batdetect2/utils/visualize.py` & `batdetect2-1.0.3/batdetect2/utils/visualize.py`

 * *Files identical despite different names*

### Comparing `batdetect2-1.0.2/batdetect2/utils/wavfile.py` & `batdetect2-1.0.3/batdetect2/utils/wavfile.py`

 * *Files identical despite different names*

### Comparing `batdetect2-1.0.2/pyproject.toml` & `batdetect2-1.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     "tests",
 ]
 venvPath = "."
 venv = ".venv"
 
 [project]
 name = "batdetect2"
-version = "1.0.2"
+version = "1.0.3"
 description = "Deep learning model for detecting and classifying bat echolocation calls in high frequency audio recordings."
 authors = [
     { name = "Oisin Mac Aodha", email = "oisin.macaodha@ed.ac.uk" },
     { name = "Santiago Martinez Balvanera", email = "santiago.balvanera.20@ucl.ac.uk" },
 ]
 dependencies = [
     "librosa",
```

### Comparing `batdetect2-1.0.2/tests/test_api.py` & `batdetect2-1.0.3/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `batdetect2-1.0.2/tests/test_cli.py` & `batdetect2-1.0.3/tests/test_cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,7 +38,32 @@
             "0.3",
         ],
     )
     assert result.exit_code == 0
     assert results_dir.exists()
     assert len(list(results_dir.glob("*.csv"))) == 3
     assert len(list(results_dir.glob("*.json"))) == 3
+
+
+def test_cli_detect_command_with_non_trivial_time_expansion(tmp_path):
+    """Test the detect command with a non-trivial time expansion factor."""
+    results_dir = tmp_path / "results"
+
+    # Remove results dir if it exists
+    if results_dir.exists():
+        results_dir.rmdir()
+
+    runner = CliRunner()
+    result = runner.invoke(
+        cli,
+        [
+            "detect",
+            "example_data/audio",
+            str(results_dir),
+            "0.3",
+            "--time_expansion_factor",
+            "10",
+        ],
+    )
+
+    assert result.exit_code == 0
+    assert 'time_exp_fact 10' in result.stdout
```

### Comparing `batdetect2-1.0.2/PKG-INFO` & `batdetect2-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: batdetect2
-Version: 1.0.2
+Version: 1.0.3
 Summary: Deep learning model for detecting and classifying bat echolocation calls in high frequency audio recordings.
 License: CC-by-nc-4
 Keywords: bat,echolocation,deep learning,audio,machine learning,classification,detection
 Author-email: Oisin Mac Aodha <oisin.macaodha@ed.ac.uk>,Santiago Martinez Balvanera <santiago.balvanera.20@ucl.ac.uk>
 Requires-Python: >=3.8,<3.11
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

