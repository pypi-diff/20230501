# Comparing `tmp/fold_wrappers-0.1.0.tar.gz` & `tmp/fold_wrappers-0.1.1.tar.gz`

## Comparing `fold_wrappers-0.1.0.tar` & `fold_wrappers-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,19 @@
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 fold_wrappers-0.1.0/.flake8
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 fold_wrappers-0.1.0/.isort.cfg
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 fold_wrappers-0.1.0/.vscode/settings.json
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 fold_wrappers-0.1.0/examples/statsforecast.py
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 fold_wrappers-0.1.0/fold_wrappers/__init__.py
--rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 fold_wrappers-0.1.0/fold_wrappers/convenience.py
--rw-r--r--   0        0        0     1943 2020-02-02 00:00:00.000000 fold_wrappers-0.1.0/fold_wrappers/lightgbm.py
--rw-r--r--   0        0        0     2990 2020-02-02 00:00:00.000000 fold_wrappers-0.1.0/fold_wrappers/neuralforecast.py
--rw-r--r--   0        0        0     3221 2020-02-02 00:00:00.000000 fold_wrappers-0.1.0/fold_wrappers/prophet.py
--rw-r--r--   0        0        0     3178 2020-02-02 00:00:00.000000 fold_wrappers-0.1.0/fold_wrappers/sktime.py
--rw-r--r--   0        0        0     3135 2020-02-02 00:00:00.000000 fold_wrappers-0.1.0/fold_wrappers/statsforecast.py
--rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 fold_wrappers-0.1.0/fold_wrappers/statsmodels.py
--rw-r--r--   0        0        0     2154 2020-02-02 00:00:00.000000 fold_wrappers-0.1.0/fold_wrappers/xgboost.py
--rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 fold_wrappers-0.1.0/.gitignore
--rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 fold_wrappers-0.1.0/LICENSE
--rw-r--r--   0        0        0     9479 2020-02-02 00:00:00.000000 fold_wrappers-0.1.0/README.md
--rw-r--r--   0        0        0     3162 2020-02-02 00:00:00.000000 fold_wrappers-0.1.0/pyproject.toml
--rw-r--r--   0        0        0    13270 2020-02-02 00:00:00.000000 fold_wrappers-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 fold_wrappers-0.1.1/.flake8
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 fold_wrappers-0.1.1/.isort.cfg
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 fold_wrappers-0.1.1/.vscode/settings.json
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 fold_wrappers-0.1.1/examples/statsforecast.py
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 fold_wrappers-0.1.1/fold_wrappers/__init__.py
+-rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 fold_wrappers-0.1.1/fold_wrappers/arch.py
+-rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 fold_wrappers-0.1.1/fold_wrappers/convenience.py
+-rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 fold_wrappers-0.1.1/fold_wrappers/lightgbm.py
+-rw-r--r--   0        0        0     2973 2020-02-02 00:00:00.000000 fold_wrappers-0.1.1/fold_wrappers/neuralforecast.py
+-rw-r--r--   0        0        0     3210 2020-02-02 00:00:00.000000 fold_wrappers-0.1.1/fold_wrappers/prophet.py
+-rw-r--r--   0        0        0     3161 2020-02-02 00:00:00.000000 fold_wrappers-0.1.1/fold_wrappers/sktime.py
+-rw-r--r--   0        0        0     3118 2020-02-02 00:00:00.000000 fold_wrappers-0.1.1/fold_wrappers/statsforecast.py
+-rw-r--r--   0        0        0     2767 2020-02-02 00:00:00.000000 fold_wrappers-0.1.1/fold_wrappers/statsmodels.py
+-rw-r--r--   0        0        0     2082 2020-02-02 00:00:00.000000 fold_wrappers-0.1.1/fold_wrappers/xgboost.py
+-rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 fold_wrappers-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 fold_wrappers-0.1.1/LICENSE
+-rw-r--r--   0        0        0     9467 2020-02-02 00:00:00.000000 fold_wrappers-0.1.1/README.md
+-rw-r--r--   0        0        0     3190 2020-02-02 00:00:00.000000 fold_wrappers-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0    13324 2020-02-02 00:00:00.000000 fold_wrappers-0.1.1/PKG-INFO
```

### Comparing `fold_wrappers-0.1.0/.vscode/settings.json` & `fold_wrappers-0.1.1/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `fold_wrappers-0.1.0/examples/statsforecast.py` & `fold_wrappers-0.1.1/examples/statsforecast.py`

 * *Files identical despite different names*

### Comparing `fold_wrappers-0.1.0/fold_wrappers/convenience.py` & `fold_wrappers-0.1.1/fold_wrappers/convenience.py`

 * *Files identical despite different names*

### Comparing `fold_wrappers-0.1.0/fold_wrappers/lightgbm.py` & `fold_wrappers-0.1.1/fold_wrappers/lightgbm.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
         if isinstance(self.model, LGBMRegressor):
             self.properties.model_type = Model.Properties.ModelType.regressor
         elif isinstance(self.model, LGBMClassifier):
             self.properties.model_type = Model.Properties.ModelType.classifier
         else:
             raise ValueError(f"Unknown model type: {type(self.model)}")
-        self.name = f"WrapLGBM-{self.model_class.__class__.__name__}"
+        self.name = self.model_class.__class__.__name__
 
     @classmethod
     def from_model(
         cls,
         model,
     ) -> WrapLGBM:
         return WrapLGBM(model.__class__, {}, instance=model)
```

### Comparing `fold_wrappers-0.1.0/fold_wrappers/neuralforecast.py` & `fold_wrappers-0.1.1/fold_wrappers/neuralforecast.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         init_args: Optional[Dict],
         instance: Optional[Any] = None,
     ) -> None:
         self.init_args = init_args
         init_args = {} if init_args is None else init_args
         self.model = model_class(**init_args) if instance is None else instance
         self.model_class = model_class
-        self.name = f"WrapNeuraForecast-{self.model.__class__.__name__}"
+        self.name = self.model_class.__class__.__name__
 
     @classmethod
     def from_model(
         cls,
         model,
     ) -> WrapNeuralForecast:
         return cls(
```

### Comparing `fold_wrappers-0.1.0/fold_wrappers/prophet.py` & `fold_wrappers-0.1.1/fold_wrappers/prophet.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         self.model = model_class(**init_args) if instance is None else instance
         self.model_class = model_class
         self.properties.mode = (
             Model.Properties.Mode.online
             if online_mode
             else Model.Properties.Mode.minibatch
         )
-        self.name = f"WrapProphet-{self.model.__class__.__name__}"
+        self.name = self.model_class.__class__.__name__
 
     @classmethod
     def from_model(
         cls,
         model,
         online_mode: bool = False,
     ) -> WrapProphet:
```

### Comparing `fold_wrappers-0.1.0/fold_wrappers/sktime.py` & `fold_wrappers-0.1.1/fold_wrappers/sktime.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         self.model_class = model_class
         self.use_exogenous = use_exogenous
         self.properties.mode = (
             Model.Properties.Mode.online
             if online_mode
             else Model.Properties.Mode.minibatch
         )
-        self.name = f"WrapStatsForecast-{self.model.__class__.__name__}"
+        self.name = self.model_class.__class__.__name__
 
     @classmethod
     def from_model(
         cls,
         model,
         use_exogenous: Optional[bool] = None,
         online_mode: bool = False,
```

### Comparing `fold_wrappers-0.1.0/fold_wrappers/statsforecast.py` & `fold_wrappers-0.1.1/fold_wrappers/statsforecast.py`

 * *Files 11% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         self.model_class = model_class
         self.use_exogenous = use_exogenous
         self.properties.mode = (
             Model.Properties.Mode.online
             if online_mode
             else Model.Properties.Mode.minibatch
         )
-        self.name = f"WrapStatsForecast-{self.model.__class__.__name__}"
+        self.name = self.model_class.__class__.__name__
 
     @classmethod
     def from_model(
         cls,
         model,
         use_exogenous: Optional[bool] = None,
         online_mode: bool = False,
```

### Comparing `fold_wrappers-0.1.0/fold_wrappers/statsmodels.py` & `fold_wrappers-0.1.1/fold_wrappers/statsmodels.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         self.model_class = model_class
         self.use_exogenous = use_exogenous
         self.properties.mode = (
             Model.Properties.Mode.online
             if online_mode
             else Model.Properties.Mode.minibatch
         )
-        self.name = f"WrapStatsModels-{self.model_class.__class__.__name__}"
+        self.name = self.model_class.__class__.__name__
         self.instance = instance
 
     def fit(
         self, X: pd.DataFrame, y: pd.Series, sample_weights: Optional[pd.Series] = None
     ) -> None:
         use_exogenous = (
             is_X_available(X) if self.use_exogenous is None else self.use_exogenous
```

### Comparing `fold_wrappers-0.1.0/fold_wrappers/xgboost.py` & `fold_wrappers-0.1.1/fold_wrappers/xgboost.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,26 +18,25 @@
         self.init_args = init_args
         init_args = {} if init_args is None else init_args
         self.model_class = model_class
 
         self.model = model_class(**init_args) if instance is None else instance
         from xgboost import XGBClassifier, XGBRegressor, XGBRFClassifier, XGBRFRegressor
 
-        self.name = f"XGB-{self.model.__class__.__name__}"
         if isinstance(self.model, XGBRegressor) or isinstance(
             self.model, XGBRFRegressor
         ):
             self.properties.model_type = Model.Properties.ModelType.regressor
         elif isinstance(self.model, XGBClassifier) or isinstance(
             self.model, XGBRFClassifier
         ):
             self.properties.model_type = Model.Properties.ModelType.classifier
         else:
             raise ValueError(f"Unknown model type: {type(self.model)}")
-        self.name = f"WrapXGB-{self.model_class.__class__.__name__}"
+        self.name = self.model_class.__class__.__name__
 
     @classmethod
     def from_model(
         cls,
         model,
     ) -> WrapXGB:
         return WrapXGB(model.__class__, {}, instance=model)
```

### Comparing `fold_wrappers-0.1.0/.gitignore` & `fold_wrappers-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `fold_wrappers-0.1.0/LICENSE` & `fold_wrappers-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fold_wrappers-0.1.0/README.md` & `fold_wrappers-0.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 <p align="center" style="display:flex; width:100%; align-items:center; justify-content:center;">
   <a style="margin:2px" href="https://github.com/dream-faster/fold-wrappers/actions/workflows/test-statsforecast.yaml"><img alt="Statsforecast Tests" src="https://github.com/dream-faster/fold-wrappers/actions/workflows/test-statsforecast.yaml/badge.svg"/></a>
   <a style="margin:2px" href="https://github.com/dream-faster/fold-wrappers/actions/workflows/test-statsmodels.yaml"><img alt="StatsModels Tests" src="https://github.com/dream-faster/fold-wrappers/actions/workflows/test-statsmodels.yaml/badge.svg"/></a>
   <a style="margin:2px" href="https://github.com/dream-faster/fold-wrappers/actions/workflows/test-xgboost.yaml"><img alt="XGBoost Tests" src="https://github.com/dream-faster/fold-wrappers/actions/workflows/test-xgboost.yaml/badge.svg"/></a>
   <a style="margin:2px" href="https://github.com/dream-faster/fold-wrappers/actions/workflows/test-sktime.yaml"><img alt="Sktime Tests" src="https://github.com/dream-faster/fold-wrappers/actions/workflows/test-sktime.yaml/badge.svg"/></a>
   <a style="margin:2px" href="https://github.com/dream-faster/fold-wrappers/actions/workflows/test-prophet.yaml"><img alt="Prophet Test" src="https://github.com/dream-faster/fold-wrappers/actions/workflows/test-prophet.yaml/badge.svg"/></a>
   <a style="margin:2px" href="https://discord.gg/EKJQgfuBpE"><img alt="Discord Community" src="https://img.shields.io/badge/Discord-%235865F2.svg?logo=discord&logoColor=white"></a>
-  <a style="margin:2px" href="https://calendly.com/mark-szulyovszky/consultation"><img alt="Calendly Booking" src="https://shields.io/badge/-Speak%20with%20us-orange?logo=minutemailer&logoColor=white"></a>
+  <a style="margin:2px" href="https://calendly.com/nowcasting/consultation"><img alt="Calendly Booking" src="https://shields.io/badge/-Speak%20with%20us-orange?logo=minutemailer&logoColor=white"></a>
 </p>
 
 <!-- PROJECT LOGO -->
 
 <br />
 <div align="center">
   <a href="https://dream-faster.github.io/fold/">
@@ -89,15 +89,15 @@
 ## Our Open-core Time Series Toolkit
 
 [![Krisi](https://raw.githubusercontent.com/dream-faster/fold/main/docs/images/overview_diagrams/dream_faster_suite_krisi.svg)](https://github.com/dream-faster/krisi)
 [![Fold](https://raw.githubusercontent.com/dream-faster/fold/main/docs/images/overview_diagrams/dream_faster_suite_fold.svg)](https://github.com/dream-faster/fold)
 [![Fold/Models](https://raw.githubusercontent.com/dream-faster/fold/main/docs/images/overview_diagrams/dream_faster_suite_fold_models.svg)](https://github.com/dream-faster/fold-models)
 [![Fold/Wrapper](https://raw.githubusercontent.com/dream-faster/fold/main/docs/images/overview_diagrams/dream_faster_suite_fold_wrappers.svg)](https://github.com/dream-faster/fold-wrappers)
 
-If you want to try them out, we'd love to hear about your use case and help, [please book a free 30-min call with us](https://calendly.com/mark-szulyovszky/consultation)!
+If you want to try them out, we'd love to hear about your use case and help, [please book a free 30-min call with us](https://calendly.com/nowcasting/consultation)!
 
 ## Contribution
 
 Join our [Discord](https://discord.gg/EKJQgfuBpE) for live discussion!
 
 Submit an issue or reach out to us on info at dream-faster.ai for any inquiries.
```

#### html2text {}

```diff
@@ -62,13 +62,13 @@
 dream_faster_suite_fold.svg)](https://github.com/dream-faster/fold) [![Fold/
 Models](https://raw.githubusercontent.com/dream-faster/fold/main/docs/images/
 overview_diagrams/dream_faster_suite_fold_models.svg)](https://github.com/
 dream-faster/fold-models) [![Fold/Wrapper](https://raw.githubusercontent.com/
 dream-faster/fold/main/docs/images/overview_diagrams/
 dream_faster_suite_fold_wrappers.svg)](https://github.com/dream-faster/fold-
 wrappers) If you want to try them out, we'd love to hear about your use case
-and help, [please book a free 30-min call with us](https://calendly.com/mark-
-szulyovszky/consultation)! ## Contribution Join our [Discord](https://
+and help, [please book a free 30-min call with us](https://calendly.com/
+nowcasting/consultation)! ## Contribution Join our [Discord](https://
 discord.gg/EKJQgfuBpE) for live discussion! Submit an issue or reach out to us
 on info at dream-faster.ai for any inquiries. ## Licence & Usage Fold-wrappers
 is under the MIT Licence, but `fold` is not. [Read more](https://dream-
 faster.github.io/fold/product/license/)
```

### Comparing `fold_wrappers-0.1.0/pyproject.toml` & `fold_wrappers-0.1.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = "hatchling.build"
 requires = ["hatchling"]
  
 [project]
 name = "fold-wrappers"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Mark Aron Szulyovszky", email="mark@dreamfaster.ai" },
   { name="Daniel Szemerey", email="daniel@dreamfaster.ai" },
 ]
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "Programming Language :: Python",
@@ -73,14 +73,17 @@
 neuralforecast = [
   "neuralforecast>=1.4",
   "torch<2.0.0",
 ]
 lightgbm = [
   "lightgbm"
 ]
+arch = [
+  "arch>=4.19.0"
+]
 
 [tool.hatch.envs.quality]
 dependencies = [
   ".[quality]",
 ]
 detached = true
 
@@ -128,15 +131,15 @@
 pythonpath = [
   "src"
 ]
 testpaths = ["tests"]
 
 # bumpver command: ``bumpver update --patch``
 [tool.bumpver]
-current_version = "0.1.0"
+current_version = "0.1.1"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "chore(Release): Bump version from {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `fold_wrappers-0.1.0/PKG-INFO` & `fold_wrappers-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fold-wrappers
-Version: 0.1.0
+Version: 0.1.1
 Summary: 3rd party model wrappers for fold.
 Project-URL: Documentation, https://dream-faster.github.io/fold-wrappers
 Project-URL: Issues, https://github.com/dream-faster/fold-wrappers/issues
 Project-URL: Source, https://github.com/dream-faster/fold-wrappers
 Author-email: Mark Aron Szulyovszky <mark@dreamfaster.ai>, Daniel Szemerey <daniel@dreamfaster.ai>
 License: MIT License
         
@@ -38,14 +38,16 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
 Requires-Dist: fold-core~=0.1
 Requires-Dist: numpy
+Provides-Extra: arch
+Requires-Dist: arch>=4.19.0; extra == 'arch'
 Provides-Extra: docs
 Requires-Dist: mkdocs-autorefs; extra == 'docs'
 Requires-Dist: mkdocs-include-markdown-plugin; extra == 'docs'
 Requires-Dist: mkdocs-material; extra == 'docs'
 Requires-Dist: mkdocstrings-python; extra == 'docs'
 Provides-Extra: lightgbm
 Requires-Dist: lightgbm; extra == 'lightgbm'
@@ -76,15 +78,15 @@
 <p align="center" style="display:flex; width:100%; align-items:center; justify-content:center;">
   <a style="margin:2px" href="https://github.com/dream-faster/fold-wrappers/actions/workflows/test-statsforecast.yaml"><img alt="Statsforecast Tests" src="https://github.com/dream-faster/fold-wrappers/actions/workflows/test-statsforecast.yaml/badge.svg"/></a>
   <a style="margin:2px" href="https://github.com/dream-faster/fold-wrappers/actions/workflows/test-statsmodels.yaml"><img alt="StatsModels Tests" src="https://github.com/dream-faster/fold-wrappers/actions/workflows/test-statsmodels.yaml/badge.svg"/></a>
   <a style="margin:2px" href="https://github.com/dream-faster/fold-wrappers/actions/workflows/test-xgboost.yaml"><img alt="XGBoost Tests" src="https://github.com/dream-faster/fold-wrappers/actions/workflows/test-xgboost.yaml/badge.svg"/></a>
   <a style="margin:2px" href="https://github.com/dream-faster/fold-wrappers/actions/workflows/test-sktime.yaml"><img alt="Sktime Tests" src="https://github.com/dream-faster/fold-wrappers/actions/workflows/test-sktime.yaml/badge.svg"/></a>
   <a style="margin:2px" href="https://github.com/dream-faster/fold-wrappers/actions/workflows/test-prophet.yaml"><img alt="Prophet Test" src="https://github.com/dream-faster/fold-wrappers/actions/workflows/test-prophet.yaml/badge.svg"/></a>
   <a style="margin:2px" href="https://discord.gg/EKJQgfuBpE"><img alt="Discord Community" src="https://img.shields.io/badge/Discord-%235865F2.svg?logo=discord&logoColor=white"></a>
-  <a style="margin:2px" href="https://calendly.com/mark-szulyovszky/consultation"><img alt="Calendly Booking" src="https://shields.io/badge/-Speak%20with%20us-orange?logo=minutemailer&logoColor=white"></a>
+  <a style="margin:2px" href="https://calendly.com/nowcasting/consultation"><img alt="Calendly Booking" src="https://shields.io/badge/-Speak%20with%20us-orange?logo=minutemailer&logoColor=white"></a>
 </p>
 
 <!-- PROJECT LOGO -->
 
 <br />
 <div align="center">
   <a href="https://dream-faster.github.io/fold/">
@@ -164,15 +166,15 @@
 ## Our Open-core Time Series Toolkit
 
 [![Krisi](https://raw.githubusercontent.com/dream-faster/fold/main/docs/images/overview_diagrams/dream_faster_suite_krisi.svg)](https://github.com/dream-faster/krisi)
 [![Fold](https://raw.githubusercontent.com/dream-faster/fold/main/docs/images/overview_diagrams/dream_faster_suite_fold.svg)](https://github.com/dream-faster/fold)
 [![Fold/Models](https://raw.githubusercontent.com/dream-faster/fold/main/docs/images/overview_diagrams/dream_faster_suite_fold_models.svg)](https://github.com/dream-faster/fold-models)
 [![Fold/Wrapper](https://raw.githubusercontent.com/dream-faster/fold/main/docs/images/overview_diagrams/dream_faster_suite_fold_wrappers.svg)](https://github.com/dream-faster/fold-wrappers)
 
-If you want to try them out, we'd love to hear about your use case and help, [please book a free 30-min call with us](https://calendly.com/mark-szulyovszky/consultation)!
+If you want to try them out, we'd love to hear about your use case and help, [please book a free 30-min call with us](https://calendly.com/nowcasting/consultation)!
 
 ## Contribution
 
 Join our [Discord](https://discord.gg/EKJQgfuBpE) for live discussion!
 
 Submit an issue or reach out to us on info at dream-faster.ai for any inquiries.
```

