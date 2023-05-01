# Comparing `tmp/forust-0.2.2.tar.gz` & `tmp/forust-0.2.3.tar.gz`

## Comparing `forust-0.2.2.tar` & `forust-0.2.3.tar`

### file list

```diff
@@ -1,41 +1,42 @@
--rw-r--r--   0        0        0      696 1970-01-01 00:00:00.000000 forust-0.2.2/local_dependencies/forust-ml/Cargo.toml
--rw-r--r--   0      501       20     5608 2023-04-23 21:34:32.000000 forust-0.2.2/local_dependencies/forust-ml/.github/workflows/CI.yml
--rw-r--r--   0      501       20      262 2023-04-23 21:34:32.000000 forust-0.2.2/local_dependencies/forust-ml/.gitignore
--rw-r--r--   0      501       20      320 2023-04-23 21:34:32.000000 forust-0.2.2/local_dependencies/forust-ml/.pre-commit-config.yaml
--rw-r--r--   0      501       20    11341 2023-04-23 21:34:32.000000 forust-0.2.2/local_dependencies/forust-ml/LICENSE
--rw-r--r--   0      501       20    10881 2023-04-23 21:34:32.000000 forust-0.2.2/local_dependencies/forust-ml/README.md
--rw-r--r--   0      501       20     3857 2023-04-23 21:34:32.000000 forust-0.2.2/local_dependencies/forust-ml/benches/forust_benchmarks.rs
--rw-r--r--   0      501       20   397862 2023-04-23 21:38:22.000000 forust-0.2.2/local_dependencies/forust-ml/dist/forust-0.2.2-cp311-cp311-macosx_10_7_x86_64.whl
--rw-r--r--   0      501       20   746003 2023-04-23 21:37:25.000000 forust-0.2.2/local_dependencies/forust-ml/dist/forust-0.2.2.tar.gz
--rw-r--r--   0      501       20    16121 2023-04-23 21:34:32.000000 forust-0.2.2/local_dependencies/forust-ml/resources/pdp_plot_age.png
--rw-r--r--   0      501       20    10758 2023-04-23 21:34:32.000000 forust-0.2.2/local_dependencies/forust-ml/resources/pdp_plot_age_mono.png
--rw-r--r--   0      501       20    57018 2023-04-23 21:34:32.000000 forust-0.2.2/local_dependencies/forust-ml/resources/titanic.csv
--rw-r--r--   0      501       20   655700 2023-04-23 21:34:32.000000 forust-0.2.2/local_dependencies/forust-ml/resources/tree-image-crop.png
--rw-r--r--   0      501       20     2556 2023-04-23 21:34:32.000000 forust-0.2.2/local_dependencies/forust-ml/rs-example.md
--rw-r--r--   0      501       20     1179 2023-04-23 21:34:32.000000 forust-0.2.2/local_dependencies/forust-ml/scripts/make_resources.py
--rw-r--r--   0      501       20       53 2023-04-23 21:34:32.000000 forust-0.2.2/local_dependencies/forust-ml/scripts/run-python-tests.ps1
--rw-r--r--   0      501       20       53 2023-04-23 21:34:32.000000 forust-0.2.2/local_dependencies/forust-ml/scripts/run-python-tests.sh
--rw-r--r--   0      501       20     5456 2023-04-23 21:34:32.000000 forust-0.2.2/local_dependencies/forust-ml/src/binning.rs
--rw-r--r--   0      501       20      248 2023-04-23 21:34:32.000000 forust-0.2.2/local_dependencies/forust-ml/src/constraints.rs
--rw-r--r--   0      501       20     8384 2023-04-23 21:34:32.000000 forust-0.2.2/local_dependencies/forust-ml/src/data.rs
--rw-r--r--   0      501       20      473 2023-04-23 21:34:32.000000 forust-0.2.2/local_dependencies/forust-ml/src/errors.rs
--rw-r--r--   0      501       20    19236 2023-04-23 21:34:32.000000 forust-0.2.2/local_dependencies/forust-ml/src/gradientbooster.rs
--rw-r--r--   0      501       20     8639 2023-04-23 21:34:32.000000 forust-0.2.2/local_dependencies/forust-ml/src/histogram.rs
--rw-r--r--   0      501       20      318 2023-04-23 21:34:32.000000 forust-0.2.2/local_dependencies/forust-ml/src/lib.rs
--rw-r--r--   0      501       20     5901 2023-04-23 21:34:32.000000 forust-0.2.2/local_dependencies/forust-ml/src/node.rs
--rw-r--r--   0      501       20     4125 2023-04-23 21:34:32.000000 forust-0.2.2/local_dependencies/forust-ml/src/objective.rs
--rw-r--r--   0      501       20     3146 2023-04-23 21:34:32.000000 forust-0.2.2/local_dependencies/forust-ml/src/partial_dependence.rs
--rw-r--r--   0      501       20    27105 2023-04-23 21:34:32.000000 forust-0.2.2/local_dependencies/forust-ml/src/splitter.rs
--rw-r--r--   0      501       20    14132 2023-04-23 21:34:32.000000 forust-0.2.2/local_dependencies/forust-ml/src/tree.rs
--rw-r--r--   0      501       20    28561 2023-04-23 21:34:32.000000 forust-0.2.2/local_dependencies/forust-ml/src/utils.rs
--rw-r--r--   0        0        0      391 1970-01-01 00:00:00.000000 forust-0.2.2/Cargo.toml
--rw-r--r--   0      501       20      685 2023-04-23 21:34:32.000000 forust-0.2.2/.gitignore
--rw-r--r--   0      501       20    10881 2023-04-23 21:35:16.000000 forust-0.2.2/README.md
--rw-r--r--   0      501       20    15483 2023-04-23 21:34:32.000000 forust-0.2.2/forust/__init__.py
--rw-r--r--   0      501       20      785 2023-04-23 21:34:32.000000 forust-0.2.2/pyproject.toml
--rw-r--r--   0      501       20     7353 2023-04-23 21:34:32.000000 forust-0.2.2/scratch.py
--rw-r--r--   0      501       20     8439 2023-04-23 21:34:32.000000 forust-0.2.2/src/lib.rs
--rw-r--r--   0      501       20     7940 2023-04-23 21:34:32.000000 forust-0.2.2/tests/test_booster.py
--rw-r--r--   0      501       20    11341 2023-04-23 21:35:16.000000 forust-0.2.2/LICENSE
--rw-r--r--   0      501       20    10881 2023-04-23 21:35:16.000000 forust-0.2.2/README.md
--rw-r--r--   0        0        0    11665 1970-01-01 00:00:00.000000 forust-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0      745 1970-01-01 00:00:00.000000 forust-0.2.3/local_dependencies/forust-ml/Cargo.toml
+-rw-r--r--   0     1001      123     5608 2023-05-01 02:04:47.000000 forust-0.2.3/local_dependencies/forust-ml/.github/workflows/CI.yml
+-rw-r--r--   0     1001      123      262 2023-05-01 02:04:47.000000 forust-0.2.3/local_dependencies/forust-ml/.gitignore
+-rw-r--r--   0     1001      123      320 2023-05-01 02:04:47.000000 forust-0.2.3/local_dependencies/forust-ml/.pre-commit-config.yaml
+-rw-r--r--   0     1001      123    11341 2023-05-01 02:04:47.000000 forust-0.2.3/local_dependencies/forust-ml/LICENSE
+-rw-r--r--   0     1001      123    11318 2023-05-01 02:04:47.000000 forust-0.2.3/local_dependencies/forust-ml/README.md
+-rw-r--r--   0     1001      123     4100 2023-05-01 02:04:47.000000 forust-0.2.3/local_dependencies/forust-ml/benches/forust_benchmarks.rs
+-rw-r--r--   0     1001      123   456826 2023-05-01 02:09:09.000000 forust-0.2.3/local_dependencies/forust-ml/dist/forust-0.2.3-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl
+-rw-r--r--   0     1001      123   749549 2023-05-01 02:08:24.000000 forust-0.2.3/local_dependencies/forust-ml/dist/forust-0.2.3.tar.gz
+-rw-r--r--   0     1001      123    16121 2023-05-01 02:04:47.000000 forust-0.2.3/local_dependencies/forust-ml/resources/pdp_plot_age.png
+-rw-r--r--   0     1001      123    10758 2023-05-01 02:04:47.000000 forust-0.2.3/local_dependencies/forust-ml/resources/pdp_plot_age_mono.png
+-rw-r--r--   0     1001      123    57018 2023-05-01 02:04:47.000000 forust-0.2.3/local_dependencies/forust-ml/resources/titanic.csv
+-rw-r--r--   0     1001      123   655700 2023-05-01 02:04:47.000000 forust-0.2.3/local_dependencies/forust-ml/resources/tree-image-crop.png
+-rw-r--r--   0     1001      123     2556 2023-05-01 02:04:47.000000 forust-0.2.3/local_dependencies/forust-ml/rs-example.md
+-rwxr-xr-x   0     1001      123     1137 2023-05-01 02:09:18.000000 forust-0.2.3/local_dependencies/forust-ml/run-maturin-action.sh
+-rw-r--r--   0     1001      123     1179 2023-05-01 02:04:47.000000 forust-0.2.3/local_dependencies/forust-ml/scripts/make_resources.py
+-rw-r--r--   0     1001      123       53 2023-05-01 02:04:47.000000 forust-0.2.3/local_dependencies/forust-ml/scripts/run-python-tests.ps1
+-rw-r--r--   0     1001      123       53 2023-05-01 02:04:47.000000 forust-0.2.3/local_dependencies/forust-ml/scripts/run-python-tests.sh
+-rw-r--r--   0     1001      123     5610 2023-05-01 02:04:47.000000 forust-0.2.3/local_dependencies/forust-ml/src/binning.rs
+-rw-r--r--   0     1001      123      248 2023-05-01 02:04:47.000000 forust-0.2.3/local_dependencies/forust-ml/src/constraints.rs
+-rw-r--r--   0     1001      123     8384 2023-05-01 02:04:47.000000 forust-0.2.3/local_dependencies/forust-ml/src/data.rs
+-rw-r--r--   0     1001      123      585 2023-05-01 02:04:47.000000 forust-0.2.3/local_dependencies/forust-ml/src/errors.rs
+-rw-r--r--   0     1001      123    23141 2023-05-01 02:04:47.000000 forust-0.2.3/local_dependencies/forust-ml/src/gradientbooster.rs
+-rw-r--r--   0     1001      123     9052 2023-05-01 02:04:47.000000 forust-0.2.3/local_dependencies/forust-ml/src/histogram.rs
+-rw-r--r--   0     1001      123      318 2023-05-01 02:04:47.000000 forust-0.2.3/local_dependencies/forust-ml/src/lib.rs
+-rw-r--r--   0     1001      123     5958 2023-05-01 02:04:47.000000 forust-0.2.3/local_dependencies/forust-ml/src/node.rs
+-rw-r--r--   0     1001      123     4125 2023-05-01 02:04:47.000000 forust-0.2.3/local_dependencies/forust-ml/src/objective.rs
+-rw-r--r--   0     1001      123     3542 2023-05-01 02:04:47.000000 forust-0.2.3/local_dependencies/forust-ml/src/partial_dependence.rs
+-rw-r--r--   0     1001      123    27131 2023-05-01 02:04:47.000000 forust-0.2.3/local_dependencies/forust-ml/src/splitter.rs
+-rw-r--r--   0     1001      123    17335 2023-05-01 02:04:47.000000 forust-0.2.3/local_dependencies/forust-ml/src/tree.rs
+-rw-r--r--   0     1001      123    28906 2023-05-01 02:04:47.000000 forust-0.2.3/local_dependencies/forust-ml/src/utils.rs
+-rw-r--r--   0        0        0      391 1970-01-01 00:00:00.000000 forust-0.2.3/Cargo.toml
+-rw-r--r--   0     1001      123      685 2023-05-01 02:04:47.000000 forust-0.2.3/.gitignore
+-rw-r--r--   0     1001      123    11318 2023-05-01 02:05:18.000000 forust-0.2.3/README.md
+-rw-r--r--   0     1001      123    17331 2023-05-01 02:04:47.000000 forust-0.2.3/forust/__init__.py
+-rw-r--r--   0     1001      123      785 2023-05-01 02:04:47.000000 forust-0.2.3/pyproject.toml
+-rw-r--r--   0     1001      123     7353 2023-05-01 02:04:47.000000 forust-0.2.3/scratch.py
+-rw-r--r--   0     1001      123     9225 2023-05-01 02:04:47.000000 forust-0.2.3/src/lib.rs
+-rw-r--r--   0     1001      123    11077 2023-05-01 02:04:47.000000 forust-0.2.3/tests/test_booster.py
+-rw-r--r--   0     1001      123    11341 2023-05-01 02:05:18.000000 forust-0.2.3/LICENSE
+-rw-r--r--   0     1001      123    11318 2023-05-01 02:05:18.000000 forust-0.2.3/README.md
+-rw-r--r--   0        0        0    12102 1970-01-01 00:00:00.000000 forust-0.2.3/PKG-INFO
```

### Comparing `forust-0.2.2/local_dependencies/forust-ml/Cargo.toml` & `forust-0.2.3/local_dependencies/forust-ml/Cargo.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 [package]
 name = "forust-ml"
-version = "0.2.2"
+version = "0.2.3"
 edition = "2021"
 authors = ["James Inlow <james.d.inlow@gmail.com>"]
 homepage = "https://github.com/jinlow/forust"
 description = "A lightweight gradient boosting implementation in Rust."
 license-file = "LICENSE"
 readme = "README.md"
 repository = "https://github.com/jinlow/forust"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
+[profile.release]
+lto = 'fat'
+codegen-units = 1
 
 [dependencies]
 rayon = "1.7"
 thiserror = "1.0"
-serde_json = {version = "1.0", features = ["float_roundtrip"] }
+serde_json = { version = "1.0", features = ["float_roundtrip"] }
 serde = { version = "1.0", features = ["derive"] }
+rand = "0.8.5"
 
 [dev-dependencies]
 criterion = "0.4"
-rand = "0.8.5"
 
 [[bench]]
 name = "forust_benchmarks"
 harness = false
```

### Comparing `forust-0.2.2/local_dependencies/forust-ml/.github/workflows/CI.yml` & `forust-0.2.3/local_dependencies/forust-ml/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `forust-0.2.2/local_dependencies/forust-ml/LICENSE` & `forust-0.2.3/local_dependencies/forust-ml/LICENSE`

 * *Files identical despite different names*

### Comparing `forust-0.2.2/local_dependencies/forust-ml/README.md` & `forust-0.2.3/local_dependencies/forust-ml/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 The package can be installed directly from [pypi](https://pypi.org/project/forust/).
 ```shell
 pip install forust
 ```
 
 To use in a rust project add the following to your Cargo.toml file.
 ```toml
-forust-ml = "0.2.2"
+forust-ml = "0.2.3"
 ```
 
 ## Usage
 The `GradientBooster` class is currently the only public facing class in the package, and can be used to train gradient boosted decision tree ensembles with multiple objective functions.
 
 It can be initialized with the following arguments.
 
@@ -58,14 +58,19 @@
     a smaller number, will result in faster training time, while potentially sacrificing
     accuracy. If there are more bins, than unique values in a column, all unique values
     will be used. Defaults to 256.
  - `parallel` ***(bool, optional)***: Should multiple cores be used when training and predicting
     with this model? Defaults to `True`.
  - `allow_missing_splits` ***(bool, optional)***: Allow for splits to be made such that all missing values go down one branch, and all non-missing values go down the other, if this results in the greatest reduction of loss. If this is false, splits will only be made on non missing values. Defaults to `True`.
  - `monotone_constraints` ***(dict[Any, int], optional)***: Constraints that are used to enforce a specific relationship between the training features and the target variable. A dictionary should be provided where the keys are the feature index value if the model will be fit on a numpy array, or a feature name if it will be fit on a pandas Dataframe. The values of the dictionary should be an integer value of -1, 1, or 0 to specify the relationship that should be estimated between the respective feature and the target variable. Use a value of -1 to enforce a negative relationship, 1 a positive relationship, and 0 will enforce no specific relationship at all. Features not included in the mapping will not have any constraint applied. If `None` is passed no constraints will be enforced on any variable.  Defaults to `None`.
+ - `subsample` ***(float, optional)***: Percent of records to randomly sample at each iteration when
+      training a tree. Defaults to 1.0, meaning all data is used for training.
+ - `seed` ***(integer, optional)***: Integer value used to seed any randomness used in the
+      algorithm. Defaults to 0.
+ - `missing` ***(float, optional)***: Value to consider missing, when training and predicting with the booster. Defaults to `np.nan`.
 
 ### Training and Predicting
 
 Once, the booster has been initialized, it can be fit on a provided dataset, and performance field. After fitting, the model can be used to predict on a dataset.
 In the case of this example, the predictions are the log odds of a given record being 1.
 
 ```python
```

#### html2text {}

```diff
@@ -13,15 +13,15 @@
 understand the XGBoost algorithm, additionally to have a fun project to work on
 in rust, and because I wanted to be able to experiment with adding new features
 to the algorithm in a smaller simpler codebase. All of the rust code for the
 package can be found in the [src](src/) directory, while all of the python
 wrapper code is in the [py-forust](py-forust/) directory. ## Installation The
 package can be installed directly from [pypi](https://pypi.org/project/forust/
 ). ```shell pip install forust ``` To use in a rust project add the following
-to your Cargo.toml file. ```toml forust-ml = "0.2.2" ``` ## Usage The
+to your Cargo.toml file. ```toml forust-ml = "0.2.3" ``` ## Usage The
 `GradientBooster` class is currently the only public facing class in the
 package, and can be used to train gradient boosted decision tree ensembles with
 multiple objective functions. It can be initialized with the following
 arguments. - `objective_type` ***(str, optional)***: The name of objective
 function used to optimize. Valid options include "LogLoss" to use logistic loss
 as the objective function (binary classification), or "SquaredLoss" to use
 Squared Error as the objective function (continuous regression). Defaults to
@@ -56,42 +56,48 @@
 index value if the model will be fit on a numpy array, or a feature name if it
 will be fit on a pandas Dataframe. The values of the dictionary should be an
 integer value of -1, 1, or 0 to specify the relationship that should be
 estimated between the respective feature and the target variable. Use a value
 of -1 to enforce a negative relationship, 1 a positive relationship, and 0 will
 enforce no specific relationship at all. Features not included in the mapping
 will not have any constraint applied. If `None` is passed no constraints will
-be enforced on any variable. Defaults to `None`. ### Training and Predicting
-Once, the booster has been initialized, it can be fit on a provided dataset,
-and performance field. After fitting, the model can be used to predict on a
-dataset. In the case of this example, the predictions are the log odds of a
-given record being 1. ```python # Small example dataset from seaborn import
-load_dataset df = load_dataset("titanic") X = df.select_dtypes("number").drop
-(columns=["survived"]) y = df["survived"] # Initialize a booster with defaults.
-from forust import GradientBooster model = GradientBooster
-(objective_type="LogLoss") model.fit(X, y) # Predict on data model.predict
-(X.head()) # array([-1.94919663, 2.25863229, 0.32963671, 2.48732194, -
-3.00371813]) # predict contributions model.predict_contributions(X.head()) #
-array([[-0.63014213, 0.33880048, -0.16520798, -0.07798772, -0.85083578, # -
-1.07720813], # [ 1.05406709, 0.08825999, 0.21662544, -0.12083538, 0.35209258, #
--1.07720813], ``` The `fit` method accepts the following arguments. - `X` ***
-(FrameLike)***: Either a pandas DataFrame, or a 2 dimensional numpy array, with
-numeric data. - `y` ***(ArrayLike)***: Either a pandas Series, or a 1
-dimensional numpy array. If "LogLoss" was the objective type specified, then
-this should only contain 1 or 0 values, where 1 is the positive class being
-predicted. If "SquaredLoss" is the objective type, then any continuous variable
-can be provided. - `sample_weight` ***(Optional[ArrayLike], optional)***:
-Instance weights to use when training the model. If None is passed, a weight of
-1 will be used for every record. Defaults to None. The predict method accepts
-the following arguments. - `X` ***(FrameLike)***: Either a pandas DataFrame, or
-a 2 dimensional numpy array, with numeric data. - `parallel` ***(Optional
-[bool], optional)***: Optionally specify if the predict function should run in
-parallel on multiple threads. If `None` is passed, the `parallel` attribute of
-the booster will be used. Defaults to `None`. The `predict_contributions`
-method will predict with the fitted booster on new data, returning the feature
+be enforced on any variable. Defaults to `None`. - `subsample` ***(float,
+optional)***: Percent of records to randomly sample at each iteration when
+training a tree. Defaults to 1.0, meaning all data is used for training. -
+`seed` ***(integer, optional)***: Integer value used to seed any randomness
+used in the algorithm. Defaults to 0. - `missing` ***(float, optional)***:
+Value to consider missing, when training and predicting with the booster.
+Defaults to `np.nan`. ### Training and Predicting Once, the booster has been
+initialized, it can be fit on a provided dataset, and performance field. After
+fitting, the model can be used to predict on a dataset. In the case of this
+example, the predictions are the log odds of a given record being 1. ```python
+# Small example dataset from seaborn import load_dataset df = load_dataset
+("titanic") X = df.select_dtypes("number").drop(columns=["survived"]) y = df
+["survived"] # Initialize a booster with defaults. from forust import
+GradientBooster model = GradientBooster(objective_type="LogLoss") model.fit(X,
+y) # Predict on data model.predict(X.head()) # array([-1.94919663, 2.25863229,
+0.32963671, 2.48732194, -3.00371813]) # predict contributions
+model.predict_contributions(X.head()) # array([[-0.63014213, 0.33880048, -
+0.16520798, -0.07798772, -0.85083578, # -1.07720813], # [ 1.05406709,
+0.08825999, 0.21662544, -0.12083538, 0.35209258, # -1.07720813], ``` The `fit`
+method accepts the following arguments. - `X` ***(FrameLike)***: Either a
+pandas DataFrame, or a 2 dimensional numpy array, with numeric data. - `y` ***
+(ArrayLike)***: Either a pandas Series, or a 1 dimensional numpy array. If
+"LogLoss" was the objective type specified, then this should only contain 1 or
+0 values, where 1 is the positive class being predicted. If "SquaredLoss" is
+the objective type, then any continuous variable can be provided. -
+`sample_weight` ***(Optional[ArrayLike], optional)***: Instance weights to use
+when training the model. If None is passed, a weight of 1 will be used for
+every record. Defaults to None. The predict method accepts the following
+arguments. - `X` ***(FrameLike)***: Either a pandas DataFrame, or a 2
+dimensional numpy array, with numeric data. - `parallel` ***(Optional[bool],
+optional)***: Optionally specify if the predict function should run in parallel
+on multiple threads. If `None` is passed, the `parallel` attribute of the
+booster will be used. Defaults to `None`. The `predict_contributions` method
+will predict with the fitted booster on new data, returning the feature
 contribution matrix. The last column is the bias term. - `X` ***(FrameLike)***:
 Either a pandas DataFrame, or a 2 dimensional numpy array, with numeric data. -
 `parallel` ***(Optional[bool], optional)***: Optionally specify if the predict
 function should run in parallel on multiple threads. If `None` is passed, the
 `parallel` attribute of the booster will be used. Defaults to `None`. ###
 Inspecting the Model Once the booster has been fit, each individual tree
 structure can be retrieved in text form, using the `text_dump` method. This
```

### Comparing `forust-0.2.2/local_dependencies/forust-ml/benches/forust_benchmarks.rs` & `forust-0.2.3/local_dependencies/forust-ml/benches/forust_benchmarks.rs`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 use forust_ml::constraints::ConstraintMap;
 use forust_ml::data::Matrix;
 use forust_ml::gradientbooster::GradientBooster;
 use forust_ml::objective::{LogLoss, ObjectiveFunction};
 use forust_ml::splitter::MissingImputerSplitter;
 use forust_ml::tree::Tree;
 use forust_ml::utils::{fast_f64_sum, fast_sum, naive_sum};
+use rand::rngs::StdRng;
+use rand::SeedableRng;
 use std::fs;
 use std::time::Duration;
 
 pub fn tree_benchmarks(c: &mut Criterion) {
     let file = fs::read_to_string("resources/contiguous_no_missing_100k_samp_seed0.csv")
         .expect("Something went wrong reading the file");
     let data_vec: Vec<f64> = file.lines().map(|x| x.parse::<f64>().unwrap()).collect();
@@ -42,48 +44,52 @@
         min_leaf_weight: 1.0,
         learning_rate: 0.3,
         allow_missing_splits: true,
         constraints_map: ConstraintMap::new(),
     };
     let mut tree = Tree::new();
 
-    let bindata = bin_matrix(&data, &w, 300).unwrap();
+    let bindata = bin_matrix(&data, &w, 300, f64::NAN).unwrap();
     let bdata = Matrix::new(&bindata.binned_data, data.rows, data.cols);
-
+    let mut rng = StdRng::seed_from_u64(0);
     tree.fit(
         &bdata,
         &bindata.cuts,
         &g,
         &h,
         &splitter,
         usize::MAX,
         5,
         true,
+        1.,
+        &mut rng,
     );
     println!("{}", tree.nodes.len());
     c.bench_function("Train Tree", |b| {
         b.iter(|| {
             let mut train_tree: Tree = Tree::new();
             train_tree.fit(
                 black_box(&bdata),
                 black_box(&bindata.cuts),
                 black_box(&g),
                 black_box(&h),
                 black_box(&splitter),
                 black_box(usize::MAX),
                 black_box(10),
                 black_box(false),
+                black_box(1.0),
+                black_box(&mut rng),
             );
         })
     });
     c.bench_function("Tree Predict (Single Threaded)", |b| {
-        b.iter(|| tree.predict(black_box(&data), black_box(false)))
+        b.iter(|| tree.predict(black_box(&data), black_box(false), black_box(&f64::NAN)))
     });
     c.bench_function("Tree Predict (Multi Threaded)", |b| {
-        b.iter(|| tree.predict(black_box(&data), black_box(true)))
+        b.iter(|| tree.predict(black_box(&data), black_box(true), black_box(&f64::NAN)))
     });
 
     // Gradient Booster
     // Bench building
     let mut booster_train = c.benchmark_group("train-booster");
     booster_train.warm_up_time(Duration::from_secs(10));
     booster_train.sample_size(50);
```

### Comparing `forust-0.2.2/local_dependencies/forust-ml/resources/pdp_plot_age.png` & `forust-0.2.3/local_dependencies/forust-ml/resources/pdp_plot_age.png`

 * *Files identical despite different names*

### Comparing `forust-0.2.2/local_dependencies/forust-ml/resources/pdp_plot_age_mono.png` & `forust-0.2.3/local_dependencies/forust-ml/resources/pdp_plot_age_mono.png`

 * *Files identical despite different names*

### Comparing `forust-0.2.2/local_dependencies/forust-ml/resources/titanic.csv` & `forust-0.2.3/local_dependencies/forust-ml/resources/titanic.csv`

 * *Files identical despite different names*

### Comparing `forust-0.2.2/local_dependencies/forust-ml/resources/tree-image-crop.png` & `forust-0.2.3/local_dependencies/forust-ml/resources/tree-image-crop.png`

 * *Files identical despite different names*

### Comparing `forust-0.2.2/local_dependencies/forust-ml/rs-example.md` & `forust-0.2.3/local_dependencies/forust-ml/rs-example.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ## A Complete Rust Example
 
 To run this example, add the following code to your `Cargo.toml` file.
 ```toml
 [dependencies]
-forust-ml = "0.2.2"
+forust-ml = "0.2.3"
 polars = "0.24"
 reqwest = { version = "0.11", features = ["blocking"] }
 ```
 
 The following is a runable example using `polars` for data processing. The actual data manipulation can be performed with any tool, the only vital part, is the data be in column major format.
 ```rust
 use forust_ml::{GradientBooster, Matrix};
```

### Comparing `forust-0.2.2/local_dependencies/forust-ml/scripts/make_resources.py` & `forust-0.2.3/local_dependencies/forust-ml/scripts/make_resources.py`

 * *Files identical despite different names*

### Comparing `forust-0.2.2/local_dependencies/forust-ml/src/binning.rs` & `forust-0.2.3/local_dependencies/forust-ml/src/binning.rs`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 use crate::data::{FloatData, JaggedMatrix, Matrix};
 use crate::errors::ForustError;
-use crate::utils::{map_bin, percentiles};
+use crate::utils::{is_missing, map_bin, percentiles};
 
 /// If there are fewer unique values than their are
 /// percentiles, just return the unique values of the
 /// vectors.
 ///
 /// * `v` - A numeric slice to calculate percentiles for.
 /// * `sample_weight` - Instance weights for each row in the data.
@@ -65,42 +65,46 @@
 }
 
 /// Bin a numeric matrix.
 ///
 /// * `data` - A numeric matrix, of data to be binned.
 /// * `sample_weight` - Instance weights for each row of the data.
 /// * `nbins` - The number of bins each column should be binned into.
-pub fn bin_matrix<T: FloatData<T>>(
-    data: &Matrix<T>,
-    sample_weight: &[T],
+/// * `missing` - Float value to consider as missing.
+pub fn bin_matrix(
+    data: &Matrix<f64>,
+    sample_weight: &[f64],
     nbins: u16,
-) -> Result<BinnedData<T>, ForustError> {
+    missing: f64,
+) -> Result<BinnedData<f64>, ForustError> {
     let mut pcts = Vec::new();
-    let nbins_ = T::from_u16(nbins);
+    let nbins_ = f64::from_u16(nbins);
     for i in 0..nbins {
-        let v = T::from_u16(i) / nbins_;
+        let v = f64::from_u16(i) / nbins_;
         pcts.push(v);
     }
 
     // First we need to generate the bins for each of the columns.
     // We will loop through all of the columns, and generate the cuts.
     let mut cuts = JaggedMatrix::new();
     let mut nunique = Vec::new();
     for i in 0..data.cols {
-        let (no_miss, w): (Vec<T>, Vec<T>) = data
+        let (no_miss, w): (Vec<f64>, Vec<f64>) = data
             .get_col(i)
             .iter()
             .zip(sample_weight.iter())
-            .filter(|(v, _)| !v.is_nan())
+            // It is unrecoverable if they have provided missing values in
+            // the data other than the specificized missing.
+            .filter(|(v, _)| !is_missing(v, &missing))
             .unzip();
         assert_eq!(no_miss.len(), w.len());
         let mut col_cuts = percentiles_or_value(&no_miss, &w, &pcts);
-        col_cuts.push(T::MAX);
+        col_cuts.push(f64::MAX);
         col_cuts.dedup();
-        if col_cuts.len() < 3 {
+        if col_cuts.len() < 2 {
             return Err(ForustError::NoVariance(i));
         }
         // There will be one less bins, then there are cuts.
         // The first value will be for missing.
         nunique.push(col_cuts.len());
         let l = col_cuts.len();
         cuts.data.extend(col_cuts);
@@ -129,15 +133,15 @@
     #[test]
     fn test_bin_data() {
         let file = fs::read_to_string("resources/contiguous_no_missing.csv")
             .expect("Something went wrong reading the file");
         let data_vec: Vec<f64> = file.lines().map(|x| x.parse::<f64>().unwrap()).collect();
         let data = Matrix::new(&data_vec, 891, 5);
         let sample_weight = vec![1.; data.rows];
-        let b = bin_matrix(&data, &sample_weight, 50).unwrap();
+        let b = bin_matrix(&data, &sample_weight, 50, f64::NAN).unwrap();
         let bdata = Matrix::new(&b.binned_data, data.rows, data.cols);
         for column in 0..data.cols {
             let mut b_compare = 1;
             for cuts in b.cuts.get_col(column).windows(2) {
                 let c1 = cuts[0];
                 let c2 = cuts[1];
                 let mut n_v = 0;
@@ -146,14 +150,13 @@
                     if *bin == b_compare {
                         n_b += 1;
                     }
                     if (c1 <= *value) && (*value < c2) {
                         n_v += 1;
                     }
                 }
-                // println!("Column: {}, Bin: {}, {} {}", column, b_compare, n_v, n_b);
                 assert_eq!(n_v, n_b);
                 b_compare += 1;
             }
         }
     }
 }
```

### Comparing `forust-0.2.2/local_dependencies/forust-ml/src/data.rs` & `forust-0.2.3/local_dependencies/forust-ml/src/data.rs`

 * *Files identical despite different names*

### Comparing `forust-0.2.2/local_dependencies/forust-ml/src/gradientbooster.rs` & `forust-0.2.3/local_dependencies/forust-ml/src/gradientbooster.rs`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 use crate::binning::bin_matrix;
 use crate::constraints::ConstraintMap;
 use crate::data::Matrix;
 use crate::errors::ForustError;
 use crate::objective::{gradient_hessian_callables, ObjectiveType};
 use crate::splitter::MissingImputerSplitter;
 use crate::tree::Tree;
+use rand::rngs::StdRng;
+use rand::SeedableRng;
 use rayon::prelude::*;
-use serde::{Deserialize, Serialize};
+use serde::{Deserialize, Deserializer, Serialize};
+use std::collections::HashMap;
 use std::fs;
-
 /// Gradient Booster object
 ///
 /// * `objective_type` - The name of objective function used to optimize.
 ///   Valid options include "LogLoss" to use logistic loss as the objective function,
 ///   or "SquaredLoss" to use Squared Error as the objective function.
 /// * `iterations` - Total number of trees to train in the ensemble.
 /// * `learning_rate` - Step size to use at each iteration. Each
@@ -48,15 +50,27 @@
     pub gamma: f32,
     pub min_leaf_weight: f32,
     pub base_score: f64,
     pub nbins: u16,
     pub parallel: bool,
     pub allow_missing_splits: bool,
     pub monotone_constraints: Option<ConstraintMap>,
+    pub subsample: f32,
+    pub seed: u64,
+    #[serde(deserialize_with = "parse_missing")]
+    pub missing: f64,
     pub trees: Vec<Tree>,
+    metadata: HashMap<String, String>,
+}
+
+fn parse_missing<'de, D>(d: D) -> Result<f64, D::Error>
+where
+    D: Deserializer<'de>,
+{
+    Deserialize::deserialize(d).map(|x: Option<_>| x.unwrap_or(f64::NAN))
 }
 
 impl Default for GradientBooster {
     fn default() -> Self {
         Self::new(
             ObjectiveType::LogLoss,
             10,
@@ -67,14 +81,17 @@
             0.,
             1.,
             0.5,
             256,
             true,
             true,
             None,
+            1.,
+            0,
+            f64::NAN,
         )
     }
 }
 
 impl GradientBooster {
     /// Gradient Booster object
     ///
@@ -98,14 +115,17 @@
     /// * `base_score` - The initial prediction value of the model.
     /// * `nbins` - Number of bins to calculate to partition the data. Setting this to
     ///   a smaller number, will result in faster training time, while potentially sacrificing
     ///   accuracy. If there are more bins, than unique values in a column, all unique values
     ///   will be used.
     /// * `monotone_constraints` - Constraints that are used to enforce a specific relationship
     ///   between the training features and the target variable.
+    /// * `subsample` - Percent of records to randomly sample at each iteration when training a tree.
+    /// * `seed` - Integer value used to seed any randomness used in the algorithm.
+    /// * `missing` - Value to consider missing.
     #[allow(clippy::too_many_arguments)]
     pub fn new(
         objective_type: ObjectiveType,
         iterations: usize,
         learning_rate: f32,
         max_depth: usize,
         max_leaves: usize,
@@ -113,14 +133,17 @@
         gamma: f32,
         min_leaf_weight: f32,
         base_score: f64,
         nbins: u16,
         parallel: bool,
         allow_missing_splits: bool,
         monotone_constraints: Option<ConstraintMap>,
+        subsample: f32,
+        seed: u64,
+        missing: f64,
     ) -> Self {
         GradientBooster {
             objective_type,
             iterations,
             learning_rate,
             max_depth,
             max_leaves,
@@ -128,15 +151,19 @@
             gamma,
             min_leaf_weight,
             base_score,
             nbins,
             parallel,
             allow_missing_splits,
             monotone_constraints,
+            subsample,
+            seed,
+            missing,
             trees: Vec::new(),
+            metadata: HashMap::new(),
         }
     }
 
     /// Fit the gradient booster on a provided dataset.
     ///
     /// * `data` -  Either a pandas DataFrame, or a 2 dimensional numpy array.
     /// * `y` - Either a pandas Series, or a 1 dimensional numpy array.
@@ -144,14 +171,15 @@
     /// training the model. If None is passed, a weight of 1 will be used for every record.
     pub fn fit(
         &mut self,
         data: &Matrix<f64>,
         y: &[f64],
         sample_weight: &[f64],
     ) -> Result<(), ForustError> {
+        let mut rng = StdRng::seed_from_u64(self.seed);
         let constraints_map = self
             .monotone_constraints
             .as_ref()
             .unwrap_or(&ConstraintMap::new())
             .to_owned();
         let splitter = MissingImputerSplitter {
             l2: self.l2,
@@ -165,31 +193,33 @@
         let (calc_grad, calc_hess) = gradient_hessian_callables(&self.objective_type);
         let mut grad = calc_grad(y, &yhat, sample_weight);
         let mut hess = calc_hess(y, &yhat, sample_weight);
 
         // Generate binned data
         // TODO
         // In scikit-learn, they sample 200_000 records for generating the bins.
-        // we could consier that, especially if this proved to be a large bottleneck...
-        let binned_data = bin_matrix(data, sample_weight, self.nbins)?;
+        // we could consider that, especially if this proved to be a large bottleneck...
+        let binned_data = bin_matrix(data, sample_weight, self.nbins, self.missing)?;
         let bdata = Matrix::new(&binned_data.binned_data, data.rows, data.cols);
 
         for _ in 0..self.iterations {
             let mut tree = Tree::new();
             tree.fit(
                 &bdata,
                 &binned_data.cuts,
                 &grad,
                 &hess,
                 &splitter,
                 self.max_leaves,
                 self.max_depth,
                 self.parallel,
+                self.subsample,
+                &mut rng,
             );
-            let preds = tree.predict(data, self.parallel);
+            let preds = tree.predict(data, self.parallel, &self.missing);
             yhat = yhat.iter().zip(preds).map(|(i, j)| *i + j).collect();
             self.trees.push(tree);
             grad = calc_grad(y, &yhat, sample_weight);
             hess = calc_hess(y, &yhat, sample_weight);
         }
         Ok(())
     }
@@ -205,15 +235,18 @@
 
     /// Generate predictions on data using the gradient booster.
     ///
     /// * `data` -  Either a pandas DataFrame, or a 2 dimensional numpy array.
     pub fn predict(&self, data: &Matrix<f64>, parallel: bool) -> Vec<f64> {
         let mut init_preds = vec![self.base_score; data.rows];
         self.trees.iter().for_each(|tree| {
-            for (p_, val) in init_preds.iter_mut().zip(tree.predict(data, parallel)) {
+            for (p_, val) in init_preds
+                .iter_mut()
+                .zip(tree.predict(data, parallel, &self.missing))
+            {
                 *p_ += val;
             }
         });
         init_preds
     }
 
     // pub fn predict(&self, data: &Matrix<f64>, parallel: bool) -> Vec<f64> {
@@ -272,25 +305,25 @@
         if parallel {
             data.index
                 .par_iter()
                 .zip(contribs.par_chunks_mut(data.cols + 1))
                 .for_each(|(row, c)| {
                     let r_ = data.get_row(*row);
                     self.trees.iter().zip(weights.iter()).for_each(|(t, w)| {
-                        t.predict_contributions_row(&r_, c, w);
+                        t.predict_contributions_row(&r_, c, w, &self.missing);
                     });
                 });
         } else {
             data.index
                 .iter()
                 .zip(contribs.chunks_mut(data.cols + 1))
                 .for_each(|(row, c)| {
                     let r_ = data.get_row(*row);
                     self.trees.iter().zip(weights.iter()).for_each(|(t, w)| {
-                        t.predict_contributions_row(&r_, c, w);
+                        t.predict_contributions_row(&r_, c, w, &self.missing);
                     });
                 });
         }
 
         contribs
     }
 
@@ -299,15 +332,15 @@
     ///
     /// * `feature` - The index of the feature.
     /// * `value` - The value for which to calculate the partial dependence.
     pub fn value_partial_dependence(&self, feature: usize, value: f64) -> f64 {
         let pd: f64 = self
             .trees
             .iter()
-            .map(|t| t.value_partial_dependence(feature, value))
+            .map(|t| t.value_partial_dependence(feature, value, &self.missing))
             .sum();
         pd + self.base_score
     }
 
     /// Save a booster as a json object to a file.
     ///
     /// * `path` - Path to save booster.
@@ -437,23 +470,87 @@
 
     /// Set the monotone_constraints on the booster.
     /// * `monotone_constraints` - The monotone constraints of the booster.
     pub fn set_monotone_constraints(mut self, monotone_constraints: Option<ConstraintMap>) -> Self {
         self.monotone_constraints = monotone_constraints;
         self
     }
+
+    /// Set the subsample on the booster.
+    /// * `subsample` - Percent of the data to randomly sample when training each tree.
+    pub fn set_subsample(mut self, subsample: f32) -> Self {
+        self.subsample = subsample;
+        self
+    }
+
+    /// Set the seed on the booster.
+    /// * `seed` - Integer value used to see any randomness used in the algorithm.
+    pub fn set_seed(mut self, seed: u64) -> Self {
+        self.seed = seed;
+        self
+    }
+
+    /// Set missing value of the booster
+    /// * `missing` - Float value to consider as missing.
+    pub fn set_missing(mut self, missing: f64) -> Self {
+        self.missing = missing;
+        self
+    }
+
+    /// Insert metadata
+    /// * `key` - String value for the metadata key.
+    /// * `value` - value to assign to the metadata key.
+    pub fn insert_metadata(&mut self, key: String, value: String) {
+        self.metadata.insert(key, value);
+    }
+
+    /// Get Metadata
+    /// * `key` - Get the associated value for the metadata key.
+    pub fn get_metadata(&self, key: &String) -> Option<String> {
+        self.metadata.get(key).cloned()
+    }
 }
 
 #[cfg(test)]
 mod tests {
     use super::*;
     use std::fs;
 
     #[test]
-    fn test_tree_fit() {
+    fn test_booster_fit_subsample() {
+        let file = fs::read_to_string("resources/contiguous_with_missing.csv")
+            .expect("Something went wrong reading the file");
+        let data_vec: Vec<f64> = file
+            .lines()
+            .map(|x| x.parse::<f64>().unwrap_or(f64::NAN))
+            .collect();
+        let file = fs::read_to_string("resources/performance.csv")
+            .expect("Something went wrong reading the file");
+        let y: Vec<f64> = file.lines().map(|x| x.parse::<f64>().unwrap()).collect();
+
+        let data = Matrix::new(&data_vec, 891, 5);
+        //let data = Matrix::new(data.get_col(1), 891, 1);
+        let mut booster = GradientBooster::default();
+        booster.iterations = 10;
+        booster.nbins = 300;
+        booster.max_depth = 3;
+        booster.subsample = 0.5;
+        let sample_weight = vec![1.; y.len()];
+        booster.fit(&data, &y, &sample_weight).unwrap();
+        let preds = booster.predict(&data, false);
+        let contribs = booster.predict_contributions(&data, false);
+        assert_eq!(contribs.len(), (data.cols + 1) * data.rows);
+        println!("{}", booster.trees[0]);
+        println!("{}", booster.trees[0].nodes.len());
+        println!("{}", booster.trees.last().unwrap().nodes.len());
+        println!("{:?}", &preds[0..10]);
+    }
+
+    #[test]
+    fn test_booster_fit() {
         let file = fs::read_to_string("resources/contiguous_with_missing.csv")
             .expect("Something went wrong reading the file");
         let data_vec: Vec<f64> = file
             .lines()
             .map(|x| x.parse::<f64>().unwrap_or(f64::NAN))
             .collect();
         let file = fs::read_to_string("resources/performance.csv")
@@ -498,9 +595,16 @@
         let sample_weight = vec![1.; y.len()];
         booster.fit(&data, &y, &sample_weight).unwrap();
         let preds = booster.predict(&data, true);
 
         booster.save_booster("resources/model64.json").unwrap();
         let booster2 = GradientBooster::load_booster("resources/model64.json").unwrap();
         assert_eq!(booster2.predict(&data, true)[0..10], preds[0..10]);
+
+        // Test with non-NAN missing.
+        booster.missing = 0.;
+        booster.save_booster("resources/modelmissing.json").unwrap();
+        let booster3 = GradientBooster::load_booster("resources/modelmissing.json").unwrap();
+        assert_eq!(booster3.missing, 0.);
+        assert_eq!(booster3.missing, booster.missing);
     }
 }
```

### Comparing `forust-0.2.2/local_dependencies/forust-ml/src/histogram.rs` & `forust-0.2.3/local_dependencies/forust-ml/src/histogram.rs`

 * *Files 3% similar despite different names*

```diff
@@ -81,15 +81,21 @@
     feature: &[u16],
     cuts: &[f64],
     sorted_grad: &[f32],
     sorted_hess: &[f32],
     index: &[usize],
 ) -> Vec<Bin<f32>> {
     let mut histogram: Vec<Bin<f64>> = Vec::with_capacity(cuts.len());
+    // The first value is missing, it seems to not matter that we are using
+    // Missing here, rather than the booster "missing" definition, because
+    // we just always assume the first bin of the histogram is missing.
     histogram.push(Bin::new_f64(f64::NAN));
+    // The last cut value is simply the maximum possible value, so we don't need it.
+    // This value is needed initially for binning, but we don't need to count it as
+    // a histogram bin.
     histogram.extend(cuts[..(cuts.len() - 1)].iter().map(|c| Bin::new_f64(*c)));
     index
         .iter()
         .zip(sorted_grad)
         .zip(sorted_hess)
         .for_each(|((i, g), h)| {
             if let Some(v) = histogram.get_mut(feature[*i] as usize) {
@@ -104,30 +110,30 @@
     pub fn new(
         data: &Matrix<u16>,
         cuts: &JaggedMatrix<f64>,
         grad: &[f32],
         hess: &[f32],
         index: &[usize],
         parallel: bool,
-        root_node: bool,
+        sort: bool,
     ) -> Self {
         let col_index: Vec<usize> = (0..data.cols).collect();
         // Sort gradients and hessians to reduce cache hits.
         // This made a really sizeable difference on larger datasets
         // Bringing training time down from nearly 6 minutes, to 2 minutes.
         // Sort gradients and hessians to reduce cache hits.
         // This made a really sizeable difference on larger datasets
         // Bringing training time down from nearly 6 minutes, to 2 minutes.
-        let sorted_grad = if root_node {
+        let sorted_grad = if !sort {
             grad.to_vec()
         } else {
             index.iter().map(|i| grad[*i]).collect::<Vec<f32>>()
         };
 
-        let sorted_hess = if root_node {
+        let sorted_hess = if !sort {
             hess.to_vec()
         } else {
             index.iter().map(|i| hess[*i]).collect::<Vec<f32>>()
         };
 
         let histograms = if parallel {
             col_index
@@ -225,15 +231,15 @@
     #[test]
     fn test_single_histogram() {
         let file = fs::read_to_string("resources/contiguous_no_missing.csv")
             .expect("Something went wrong reading the file");
         let data_vec: Vec<f64> = file.lines().map(|x| x.parse::<f64>().unwrap()).collect();
         let data = Matrix::new(&data_vec, 891, 5);
         let sample_weight = vec![1.; data.rows];
-        let b = bin_matrix(&data, &sample_weight, 10).unwrap();
+        let b = bin_matrix(&data, &sample_weight, 10, f64::NAN).unwrap();
         let bdata = Matrix::new(&b.binned_data, data.rows, data.cols);
         let y: Vec<f64> = file.lines().map(|x| x.parse::<f64>().unwrap()).collect();
         let yhat = vec![0.5; y.len()];
         let w = vec![1.; y.len()];
         let g = LogLoss::calc_grad(&y, &yhat, &w);
         let h = LogLoss::calc_hess(&y, &yhat, &w);
         let hist =
```

### Comparing `forust-0.2.2/local_dependencies/forust-ml/src/node.rs` & `forust-0.2.3/local_dependencies/forust-ml/src/node.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 use crate::data::FloatData;
 use crate::histogram::HistogramMatrix;
 use crate::splitter::{MissingInfo, NodeInfo, SplitInfo};
+use crate::utils::is_missing;
 use serde::{Deserialize, Serialize};
 use std::fmt::{self, Debug};
 
 #[derive(Debug, Deserialize, Serialize)]
 pub struct SplittableNode {
     pub num: usize,
     pub histograms: HistogramMatrix,
@@ -50,16 +51,16 @@
         self.split_value = split_node.split_value;
         self.split_feature = split_node.split_feature;
         self.split_gain = split_node.split_gain;
         self.left_child = split_node.left_child;
         self.right_child = split_node.right_child;
     }
     /// Get the path that should be traveled down, given a value.
-    pub fn get_child_idx(&self, v: &f64) -> usize {
-        if v.is_nan() {
+    pub fn get_child_idx(&self, v: &f64, missing: &f64) -> usize {
+        if is_missing(v, missing) {
             self.missing_node
         } else if v < &self.split_value {
             self.left_child
         } else {
             //  if v >= &self.split_value
             self.right_child
         }
```

### Comparing `forust-0.2.2/local_dependencies/forust-ml/src/objective.rs` & `forust-0.2.3/local_dependencies/forust-ml/src/objective.rs`

 * *Files identical despite different names*

### Comparing `forust-0.2.2/local_dependencies/forust-ml/src/partial_dependence.rs` & `forust-0.2.3/local_dependencies/forust-ml/src/partial_dependence.rs`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-use crate::tree::Tree;
+use crate::{tree::Tree, utils::is_missing};
 
 /// Partial Dependence Calculator
 // struct PDCalculator {
 //     partial_dependence: f32,
 //     base_score: f64,
 //     tree_prediction: f64,
 
@@ -14,49 +14,55 @@
 
 pub fn tree_partial_dependence(
     tree: &Tree,
     node_idx: usize,
     feature: usize,
     value: f64,
     proportion: f32,
+    missing: &f64,
 ) -> f64 {
     let n = &tree.nodes[node_idx];
     if n.is_leaf {
         f64::from(proportion * n.weight_value)
     } else if n.split_feature == feature {
-        let child = if value.is_nan() {
+        let child = if is_missing(&value, missing) {
             n.missing_node
         } else if value < n.split_value {
             n.left_child
         } else {
             n.right_child
         };
-        tree_partial_dependence(tree, child, feature, value, proportion)
+        tree_partial_dependence(tree, child, feature, value, proportion, missing)
     } else {
         let left_cover = get_node_cover(tree, n.left_child);
         let right_cover = get_node_cover(tree, n.right_child);
         let total_cover = left_cover + right_cover;
         tree_partial_dependence(
             tree,
             n.left_child,
             feature,
             value,
             proportion * (left_cover / total_cover),
+            missing,
         ) + tree_partial_dependence(
             tree,
             n.right_child,
             feature,
             value,
             proportion * (right_cover / total_cover),
+            missing,
         )
     }
 }
 
 #[cfg(test)]
 mod tests {
+    use rand::rngs::StdRng;
+    use rand::SeedableRng;
+
     use super::*;
     use crate::binning::bin_matrix;
     use crate::constraints::ConstraintMap;
     use crate::data::Matrix;
     use crate::objective::{LogLoss, ObjectiveFunction};
     use crate::splitter::MissingImputerSplitter;
     use crate::tree::Tree;
@@ -81,17 +87,29 @@
             min_leaf_weight: 1.0,
             learning_rate: 0.3,
             allow_missing_splits: true,
             constraints_map: ConstraintMap::new(),
         };
         let mut tree = Tree::new();
 
-        let b = bin_matrix(&data, &w, 300).unwrap();
+        let b = bin_matrix(&data, &w, 300, f64::NAN).unwrap();
         let bdata = Matrix::new(&b.binned_data, data.rows, data.cols);
 
-        tree.fit(&bdata, &b.cuts, &g, &h, &splitter, usize::MAX, 5, true);
-        let pdp1 = tree_partial_dependence(&tree, 0, 0, 1.0, 1.0);
-        let pdp2 = tree_partial_dependence(&tree, 0, 0, 2.0, 1.0);
-        let pdp3 = tree_partial_dependence(&tree, 0, 0, 3.0, 1.0);
+        let mut rng = StdRng::seed_from_u64(0);
+        tree.fit(
+            &bdata,
+            &b.cuts,
+            &g,
+            &h,
+            &splitter,
+            usize::MAX,
+            5,
+            true,
+            1.,
+            &mut rng,
+        );
+        let pdp1 = tree_partial_dependence(&tree, 0, 0, 1.0, 1.0, &f64::NAN);
+        let pdp2 = tree_partial_dependence(&tree, 0, 0, 2.0, 1.0, &f64::NAN);
+        let pdp3 = tree_partial_dependence(&tree, 0, 0, 3.0, 1.0, &f64::NAN);
         println!("{}, {}, {}", pdp1, pdp2, pdp3);
     }
 }
```

### Comparing `forust-0.2.2/local_dependencies/forust-ml/src/splitter.rs` & `forust-0.2.3/local_dependencies/forust-ml/src/splitter.rs`

 * *Files 0% similar despite different names*

```diff
@@ -585,27 +585,27 @@
             left_histograms = HistogramMatrix::new(
                 data,
                 cuts,
                 grad,
                 hess,
                 &index[node.start_idx..split_idx],
                 parallel,
-                false,
+                true,
             );
             right_histograms =
                 HistogramMatrix::from_parent_child(&node.histograms, &left_histograms);
         } else {
             right_histograms = HistogramMatrix::new(
                 data,
                 cuts,
                 grad,
                 hess,
                 &index[split_idx..node.stop_idx],
                 parallel,
-                false,
+                true,
             );
             left_histograms =
                 HistogramMatrix::from_parent_child(&node.histograms, &right_histograms);
         }
 
         node.update_children(left_idx, right_idx, &split_info);
 
@@ -656,18 +656,18 @@
         let data = Matrix::new(&d, 7, 1);
         let y = vec![0., 0., 0., 1., 1., 0., 1.];
         let yhat = vec![0.; 7];
         let w = vec![1.; y.len()];
         let grad = LogLoss::calc_grad(&y, &yhat, &w);
         let hess = LogLoss::calc_hess(&y, &yhat, &w);
 
-        let b = bin_matrix(&data, &w, 10).unwrap();
+        let b = bin_matrix(&data, &w, 10, f64::NAN).unwrap();
         let bdata = Matrix::new(&b.binned_data, data.rows, data.cols);
         let index = data.index.to_owned();
-        let hists = HistogramMatrix::new(&bdata, &b.cuts, &grad, &hess, &index, true, false);
+        let hists = HistogramMatrix::new(&bdata, &b.cuts, &grad, &hess, &index, true, true);
         let splitter = MissingImputerSplitter {
             l2: 0.0,
             gamma: 0.0,
             min_leaf_weight: 0.0,
             learning_rate: 1.0,
             allow_missing_splits: true,
             constraints_map: ConstraintMap::new(),
@@ -703,18 +703,18 @@
         let data = Matrix::new(&d, 7, 2);
         let y = vec![0., 0., 0., 1., 1., 0., 1.];
         let yhat = vec![0.; 7];
         let w = vec![1.; y.len()];
         let grad = LogLoss::calc_grad(&y, &yhat, &w);
         let hess = LogLoss::calc_hess(&y, &yhat, &w);
 
-        let b = bin_matrix(&data, &w, 10).unwrap();
+        let b = bin_matrix(&data, &w, 10, f64::NAN).unwrap();
         let bdata = Matrix::new(&b.binned_data, data.rows, data.cols);
         let index = data.index.to_owned();
-        let hists = HistogramMatrix::new(&bdata, &b.cuts, &grad, &hess, &index, true, false);
+        let hists = HistogramMatrix::new(&bdata, &b.cuts, &grad, &hess, &index, true, true);
         println!("{:?}", hists);
         let splitter = MissingImputerSplitter {
             l2: 0.0,
             gamma: 0.0,
             min_leaf_weight: 0.0,
             learning_rate: 1.0,
             allow_missing_splits: true,
@@ -770,15 +770,15 @@
         let hessian_sum = hess.iter().copied().sum();
         let root_gain = gain(&splitter.l2, gradient_sum, hessian_sum);
         let root_weight = weight(&splitter.l2, gradient_sum, hessian_sum);
         // let gain_given_weight = splitter.gain_given_weight(gradient_sum, hessian_sum, root_weight);
         // println!("gain: {}, weight: {}, gain from weight: {}", root_gain, root_weight, gain_given_weight);
         let data = Matrix::new(&data_vec, 891, 5);
 
-        let b = bin_matrix(&data, &w, 10).unwrap();
+        let b = bin_matrix(&data, &w, 10, f64::NAN).unwrap();
         let bdata = Matrix::new(&b.binned_data, data.rows, data.cols);
         let index = data.index.to_owned();
         let hists = HistogramMatrix::new(&bdata, &b.cuts, &grad, &hess, &index, true, false);
 
         let mut n = SplittableNode::new(
             0,
             // (0..(data.rows - 1)).collect(),
```

### Comparing `forust-0.2.2/local_dependencies/forust-ml/src/tree.rs` & `forust-0.2.3/local_dependencies/forust-ml/src/tree.rs`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 use crate::data::{JaggedMatrix, Matrix};
 use crate::histogram::HistogramMatrix;
 use crate::node::{Node, SplittableNode};
 use crate::partial_dependence::tree_partial_dependence;
 use crate::splitter::Splitter;
 use crate::utils::fast_f64_sum;
 use crate::utils::{gain, weight};
+use rand::rngs::StdRng;
+use rand::Rng;
 use rayon::prelude::*;
 use serde::{Deserialize, Serialize};
 use std::collections::VecDeque;
 use std::fmt::{self, Display};
 
 #[derive(Deserialize, Serialize)]
 pub struct Tree {
@@ -33,36 +35,63 @@
         cuts: &JaggedMatrix<f64>,
         grad: &[f32],
         hess: &[f32],
         splitter: &T,
         max_leaves: usize,
         max_depth: usize,
         parallel: bool,
+        subsample: f32,
+        rng: &mut StdRng,
     ) {
         // Recreating the index for each tree, ensures that the tree construction is faster
         // for the root node. This also ensures that sorting the records is always fast,
         // because we are starting from a nearly sorted array.
-        let mut index = data.index.to_owned();
+        let (mut index, gradient_sum, hessian_sum, sort) = if subsample == 1. {
+            // We don't need to sort, if we are not sampling. This is because
+            // the data is already sorted.
+            (
+                data.index.to_owned(),
+                fast_f64_sum(grad),
+                fast_f64_sum(hess),
+                false,
+            )
+        } else {
+            // Accumulate using f64 for numeric fidelity.
+            let mut gs: f64 = 0.;
+            let mut hs: f64 = 0.;
+            let mut index = Vec::new();
+            for ((i, g), h) in data
+                .index
+                .iter()
+                .zip(grad)
+                .zip(hess)
+                .filter(|_| rng.gen_range(0.0..1.0) < subsample)
+            {
+                index.push(*i);
+                gs += *g as f64;
+                hs += *h as f64;
+            }
+            (index, gs as f32, hs as f32, true)
+        };
+
         let mut n_nodes = 1;
-        let gradient_sum = fast_f64_sum(grad);
-        let hessian_sum = fast_f64_sum(hess);
         let root_gain = gain(&splitter.get_l2(), gradient_sum, hessian_sum);
         let root_weight = weight(&splitter.get_l2(), gradient_sum, hessian_sum);
         // Calculate the histograms for the root node.
-        let root_hists = HistogramMatrix::new(data, cuts, grad, hess, &index, parallel, true);
+        let root_hists = HistogramMatrix::new(data, cuts, grad, hess, &index, parallel, sort);
         let root_node = SplittableNode::new(
             0,
             root_hists,
             root_weight,
             root_gain,
             gradient_sum,
             hessian_sum,
             0,
             0,
-            data.rows,
+            index.len(),
             f32::NEG_INFINITY,
             f32::INFINITY,
         );
         // Add the first node to the tree nodes.
         self.nodes.push(root_node.as_node());
         let mut n_leaves = 1;
         let mut growable: VecDeque<SplittableNode> = VecDeque::new();
@@ -114,125 +143,134 @@
                 for n in new_nodes {
                     self.nodes.push(n.as_node());
                     growable.push_front(n)
                 }
             }
         }
     }
-    pub fn predict_contributions_row(&self, row: &[f64], contribs: &mut [f64], weights: &[f64]) {
+    pub fn predict_contributions_row(
+        &self,
+        row: &[f64],
+        contribs: &mut [f64],
+        weights: &[f64],
+        missing: &f64,
+    ) {
         // Add the bias term first...
         contribs[contribs.len() - 1] += weights[0];
         let mut node_idx = 0;
         loop {
             let node = &self.nodes[node_idx];
             if node.is_leaf {
                 break;
             }
             // Get change of weight given child's weight.
-            let child_idx = node.get_child_idx(&row[node.split_feature]);
+            let child_idx = node.get_child_idx(&row[node.split_feature], missing);
             let node_weight = weights[node_idx];
             let child_weight = weights[child_idx];
             let delta = child_weight - node_weight;
             contribs[node.split_feature] += delta;
             node_idx = child_idx
         }
     }
 
     fn predict_contributions_single_threaded(
         &self,
         data: &Matrix<f64>,
         contribs: &mut [f64],
         weights: &[f64],
+        missing: &f64,
     ) {
         // There needs to always be at least 2 trees
         data.index
             .iter()
             .zip(contribs.chunks_mut(data.cols + 1))
             .for_each(|(row, contribs)| {
-                self.predict_contributions_row(&data.get_row(*row), contribs, weights)
+                self.predict_contributions_row(&data.get_row(*row), contribs, weights, missing)
             })
     }
 
     fn predict_contributions_parallel(
         &self,
         data: &Matrix<f64>,
         contribs: &mut [f64],
         weights: &[f64],
+        missing: &f64,
     ) {
         // There needs to always be at least 2 trees
         data.index
             .par_iter()
             .zip(contribs.par_chunks_mut(data.cols + 1))
             .for_each(|(row, contribs)| {
-                self.predict_contributions_row(&data.get_row(*row), contribs, weights)
+                self.predict_contributions_row(&data.get_row(*row), contribs, weights, missing)
             })
     }
 
     pub fn predict_contributions(
         &self,
         data: &Matrix<f64>,
         contribs: &mut [f64],
         weights: &[f64],
         parallel: bool,
+        missing: &f64,
     ) {
         if parallel {
-            self.predict_contributions_parallel(data, contribs, weights)
+            self.predict_contributions_parallel(data, contribs, weights, missing)
         } else {
-            self.predict_contributions_single_threaded(data, contribs, weights)
+            self.predict_contributions_single_threaded(data, contribs, weights, missing)
         }
     }
 
-    fn predict_row(&self, data: &Matrix<f64>, row: usize) -> f64 {
+    fn predict_row(&self, data: &Matrix<f64>, row: usize, missing: &f64) -> f64 {
         let mut node_idx = 0;
         loop {
             let node = &self.nodes[node_idx];
             if node.is_leaf {
                 return node.weight_value as f64;
             } else {
-                node_idx = node.get_child_idx(data.get(row, node.split_feature));
+                node_idx = node.get_child_idx(data.get(row, node.split_feature), missing);
             }
         }
     }
 
-    pub fn predict_row_from_row_slice(&self, row: &[f64]) -> f64 {
+    pub fn predict_row_from_row_slice(&self, row: &[f64], missing: &f64) -> f64 {
         let mut node_idx = 0;
         loop {
             let node = &self.nodes[node_idx];
             if node.is_leaf {
                 return node.weight_value as f64;
             } else {
-                node_idx = node.get_child_idx(&row[node.split_feature]);
+                node_idx = node.get_child_idx(&row[node.split_feature], missing);
             }
         }
     }
 
-    fn predict_single_threaded(&self, data: &Matrix<f64>) -> Vec<f64> {
+    fn predict_single_threaded(&self, data: &Matrix<f64>, missing: &f64) -> Vec<f64> {
         data.index
             .iter()
-            .map(|i| self.predict_row(data, *i))
+            .map(|i| self.predict_row(data, *i, missing))
             .collect()
     }
 
-    fn predict_parallel(&self, data: &Matrix<f64>) -> Vec<f64> {
+    fn predict_parallel(&self, data: &Matrix<f64>, missing: &f64) -> Vec<f64> {
         data.index
             .par_iter()
-            .map(|i| self.predict_row(data, *i))
+            .map(|i| self.predict_row(data, *i, missing))
             .collect()
     }
 
-    pub fn predict(&self, data: &Matrix<f64>, parallel: bool) -> Vec<f64> {
+    pub fn predict(&self, data: &Matrix<f64>, parallel: bool, missing: &f64) -> Vec<f64> {
         if parallel {
-            self.predict_parallel(data)
+            self.predict_parallel(data, missing)
         } else {
-            self.predict_single_threaded(data)
+            self.predict_single_threaded(data, missing)
         }
     }
 
-    pub fn value_partial_dependence(&self, feature: usize, value: f64) -> f64 {
-        tree_partial_dependence(self, 0, feature, value, 1.0)
+    pub fn value_partial_dependence(&self, feature: usize, value: f64, missing: &f64) -> f64 {
+        tree_partial_dependence(self, 0, feature, value, 1.0, missing)
     }
     fn distribute_node_leaf_weights(&self, i: usize, weights: &mut [f64]) -> f64 {
         let node = &self.nodes[i];
         let mut w = node.weight_value as f64;
         if !node.is_leaf {
             let left_node = &self.nodes[node.left_child];
             let right_node = &self.nodes[node.right_child];
@@ -278,17 +316,19 @@
 mod tests {
     use super::*;
     use crate::binning::bin_matrix;
     use crate::constraints::{Constraint, ConstraintMap};
     use crate::objective::{LogLoss, ObjectiveFunction};
     use crate::splitter::MissingImputerSplitter;
     use crate::utils::precision_round;
+    use rand::rngs::StdRng;
+    use rand::SeedableRng;
     use std::fs;
     #[test]
-    fn test_tree_fit() {
+    fn test_tree_fit_with_subsample() {
         let file = fs::read_to_string("resources/contiguous_no_missing.csv")
             .expect("Something went wrong reading the file");
         let data_vec: Vec<f64> = file.lines().map(|x| x.parse::<f64>().unwrap()).collect();
         let file = fs::read_to_string("resources/performance.csv")
             .expect("Something went wrong reading the file");
         let y: Vec<f64> = file.lines().map(|x| x.parse::<f64>().unwrap()).collect();
         let yhat = vec![0.5; y.len()];
@@ -303,28 +343,80 @@
             min_leaf_weight: 1.0,
             learning_rate: 0.3,
             allow_missing_splits: true,
             constraints_map: ConstraintMap::new(),
         };
         let mut tree = Tree::new();
 
-        let b = bin_matrix(&data, &w, 300).unwrap();
+        let b = bin_matrix(&data, &w, 300, f64::NAN).unwrap();
         let bdata = Matrix::new(&b.binned_data, data.rows, data.cols);
+        let mut rng = StdRng::seed_from_u64(0);
+        tree.fit(
+            &bdata,
+            &b.cuts,
+            &g,
+            &h,
+            &splitter,
+            usize::MAX,
+            5,
+            true,
+            0.5,
+            &mut rng,
+        );
+    }
+
+    #[test]
+    fn test_tree_fit() {
+        let file = fs::read_to_string("resources/contiguous_no_missing.csv")
+            .expect("Something went wrong reading the file");
+        let data_vec: Vec<f64> = file.lines().map(|x| x.parse::<f64>().unwrap()).collect();
+        let file = fs::read_to_string("resources/performance.csv")
+            .expect("Something went wrong reading the file");
+        let y: Vec<f64> = file.lines().map(|x| x.parse::<f64>().unwrap()).collect();
+        let yhat = vec![0.5; y.len()];
+        let w = vec![1.; y.len()];
+        let g = LogLoss::calc_grad(&y, &yhat, &w);
+        let h = LogLoss::calc_hess(&y, &yhat, &w);
 
-        tree.fit(&bdata, &b.cuts, &g, &h, &splitter, usize::MAX, 5, true);
+        let data = Matrix::new(&data_vec, 891, 5);
+        let splitter = MissingImputerSplitter {
+            l2: 1.0,
+            gamma: 3.0,
+            min_leaf_weight: 1.0,
+            learning_rate: 0.3,
+            allow_missing_splits: true,
+            constraints_map: ConstraintMap::new(),
+        };
+        let mut tree = Tree::new();
+
+        let b = bin_matrix(&data, &w, 300, f64::NAN).unwrap();
+        let bdata = Matrix::new(&b.binned_data, data.rows, data.cols);
+        let mut rng = StdRng::seed_from_u64(0);
+        tree.fit(
+            &bdata,
+            &b.cuts,
+            &g,
+            &h,
+            &splitter,
+            usize::MAX,
+            5,
+            true,
+            1.,
+            &mut rng,
+        );
 
         // println!("{}", tree);
         // let preds = tree.predict(&data, false);
         // println!("{:?}", &preds[0..10]);
         assert_eq!(25, tree.nodes.len());
         // Test contributions prediction...
         let weights = tree.distribute_leaf_weights();
         let mut contribs = vec![0.; (data.cols + 1) * data.rows];
-        tree.predict_contributions(&data, &mut contribs, &weights, false);
-        let full_preds = tree.predict(&data, true);
+        tree.predict_contributions(&data, &mut contribs, &weights, false, &f64::NAN);
+        let full_preds = tree.predict(&data, true, &f64::NAN);
         assert_eq!(contribs.len(), (data.cols + 1) * data.rows);
 
         let contribs_preds: Vec<f64> = contribs
             .chunks(data.cols + 1)
             .map(|i| i.iter().sum())
             .collect();
         println!("{:?}", &contribs[0..10]);
@@ -344,48 +436,61 @@
         let file = fs::read_to_string("resources/performance.csv")
             .expect("Something went wrong reading the file");
         let y: Vec<f64> = file.lines().map(|x| x.parse::<f64>().unwrap()).collect();
         let yhat = vec![0.5; y.len()];
         let w = vec![1.; y.len()];
         let g = LogLoss::calc_grad(&y, &yhat, &w);
         let h = LogLoss::calc_hess(&y, &yhat, &w);
+        println!("GRADIENT -- {:?}", h);
 
         let data_ = Matrix::new(&data_vec, 891, 5);
         let data = Matrix::new(data_.get_col(1), 891, 1);
         let map = ConstraintMap::from([(0, Constraint::Negative)]);
         let splitter = MissingImputerSplitter {
             l2: 1.0,
             gamma: 0.0,
             min_leaf_weight: 1.0,
             learning_rate: 0.3,
             allow_missing_splits: true,
             constraints_map: map,
         };
         let mut tree = Tree::new();
 
-        let b = bin_matrix(&data, &w, 300).unwrap();
+        let b = bin_matrix(&data, &w, 300, f64::NAN).unwrap();
         let bdata = Matrix::new(&b.binned_data, data.rows, data.cols);
 
-        tree.fit(&bdata, &b.cuts, &g, &h, &splitter, usize::MAX, 5, true);
+        let mut rng = StdRng::seed_from_u64(0);
+        tree.fit(
+            &bdata,
+            &b.cuts,
+            &g,
+            &h,
+            &splitter,
+            usize::MAX,
+            5,
+            true,
+            1.,
+            &mut rng,
+        );
 
         // println!("{}", tree);
         let mut pred_data_vec = data.get_col(0).to_owned();
         pred_data_vec.sort_by(|a, b| a.partial_cmp(b).unwrap());
         pred_data_vec.dedup();
         let pred_data = Matrix::new(&pred_data_vec, pred_data_vec.len(), 1);
 
-        let preds = tree.predict(&pred_data, false);
+        let preds = tree.predict(&pred_data, false, &f64::NAN);
         let increasing = preds.windows(2).all(|a| a[0] >= a[1]);
         assert!(increasing);
 
         let weights = tree.distribute_leaf_weights();
 
         let mut contribs = vec![0.; (data.cols + 1) * data.rows];
-        tree.predict_contributions(&data, &mut contribs, &weights, false);
-        let full_preds = tree.predict(&data, true);
+        tree.predict_contributions(&data, &mut contribs, &weights, false, &f64::NAN);
+        let full_preds = tree.predict(&data, true, &f64::NAN);
         assert_eq!(contribs.len(), (data.cols + 1) * data.rows);
         let contribs_preds: Vec<f64> = contribs
             .chunks(data.cols + 1)
             .map(|i| i.iter().sum())
             .collect();
         assert_eq!(contribs_preds.len(), full_preds.len());
         for (i, j) in full_preds.iter().zip(contribs_preds) {
```

### Comparing `forust-0.2.2/local_dependencies/forust-ml/src/utils.rs` & `forust-0.2.3/local_dependencies/forust-ml/src/utils.rs`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,28 @@
 use crate::constraints::Constraint;
 use crate::data::FloatData;
 use std::cmp::Ordering;
 use std::collections::VecDeque;
 use std::convert::TryInto;
 
+/// Calculate if a value is missing.
+#[inline]
+pub fn is_missing(value: &f64, missing: &f64) -> bool {
+    if missing.is_nan() {
+        value.is_nan()
+    } else if value.is_nan() {
+        panic!(
+            "Missing value is {}, however NAN value found in data.",
+            missing
+        )
+    } else {
+        value == missing
+    }
+}
+
 /// Calculate the constraint weight given bounds
 /// and a constraint.
 #[inline]
 pub fn constrained_weight(
     l2: &f32,
     gradient_sum: f32,
     hessian_sum: f32,
```

### Comparing `forust-0.2.2/.gitignore` & `forust-0.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `forust-0.2.2/README.md` & `forust-0.2.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 The package can be installed directly from [pypi](https://pypi.org/project/forust/).
 ```shell
 pip install forust
 ```
 
 To use in a rust project add the following to your Cargo.toml file.
 ```toml
-forust-ml = "0.2.2"
+forust-ml = "0.2.3"
 ```
 
 ## Usage
 The `GradientBooster` class is currently the only public facing class in the package, and can be used to train gradient boosted decision tree ensembles with multiple objective functions.
 
 It can be initialized with the following arguments.
 
@@ -58,14 +58,19 @@
     a smaller number, will result in faster training time, while potentially sacrificing
     accuracy. If there are more bins, than unique values in a column, all unique values
     will be used. Defaults to 256.
  - `parallel` ***(bool, optional)***: Should multiple cores be used when training and predicting
     with this model? Defaults to `True`.
  - `allow_missing_splits` ***(bool, optional)***: Allow for splits to be made such that all missing values go down one branch, and all non-missing values go down the other, if this results in the greatest reduction of loss. If this is false, splits will only be made on non missing values. Defaults to `True`.
  - `monotone_constraints` ***(dict[Any, int], optional)***: Constraints that are used to enforce a specific relationship between the training features and the target variable. A dictionary should be provided where the keys are the feature index value if the model will be fit on a numpy array, or a feature name if it will be fit on a pandas Dataframe. The values of the dictionary should be an integer value of -1, 1, or 0 to specify the relationship that should be estimated between the respective feature and the target variable. Use a value of -1 to enforce a negative relationship, 1 a positive relationship, and 0 will enforce no specific relationship at all. Features not included in the mapping will not have any constraint applied. If `None` is passed no constraints will be enforced on any variable.  Defaults to `None`.
+ - `subsample` ***(float, optional)***: Percent of records to randomly sample at each iteration when
+      training a tree. Defaults to 1.0, meaning all data is used for training.
+ - `seed` ***(integer, optional)***: Integer value used to seed any randomness used in the
+      algorithm. Defaults to 0.
+ - `missing` ***(float, optional)***: Value to consider missing, when training and predicting with the booster. Defaults to `np.nan`.
 
 ### Training and Predicting
 
 Once, the booster has been initialized, it can be fit on a provided dataset, and performance field. After fitting, the model can be used to predict on a dataset.
 In the case of this example, the predictions are the log odds of a given record being 1.
 
 ```python
```

#### html2text {}

```diff
@@ -13,15 +13,15 @@
 understand the XGBoost algorithm, additionally to have a fun project to work on
 in rust, and because I wanted to be able to experiment with adding new features
 to the algorithm in a smaller simpler codebase. All of the rust code for the
 package can be found in the [src](src/) directory, while all of the python
 wrapper code is in the [py-forust](py-forust/) directory. ## Installation The
 package can be installed directly from [pypi](https://pypi.org/project/forust/
 ). ```shell pip install forust ``` To use in a rust project add the following
-to your Cargo.toml file. ```toml forust-ml = "0.2.2" ``` ## Usage The
+to your Cargo.toml file. ```toml forust-ml = "0.2.3" ``` ## Usage The
 `GradientBooster` class is currently the only public facing class in the
 package, and can be used to train gradient boosted decision tree ensembles with
 multiple objective functions. It can be initialized with the following
 arguments. - `objective_type` ***(str, optional)***: The name of objective
 function used to optimize. Valid options include "LogLoss" to use logistic loss
 as the objective function (binary classification), or "SquaredLoss" to use
 Squared Error as the objective function (continuous regression). Defaults to
@@ -56,42 +56,48 @@
 index value if the model will be fit on a numpy array, or a feature name if it
 will be fit on a pandas Dataframe. The values of the dictionary should be an
 integer value of -1, 1, or 0 to specify the relationship that should be
 estimated between the respective feature and the target variable. Use a value
 of -1 to enforce a negative relationship, 1 a positive relationship, and 0 will
 enforce no specific relationship at all. Features not included in the mapping
 will not have any constraint applied. If `None` is passed no constraints will
-be enforced on any variable. Defaults to `None`. ### Training and Predicting
-Once, the booster has been initialized, it can be fit on a provided dataset,
-and performance field. After fitting, the model can be used to predict on a
-dataset. In the case of this example, the predictions are the log odds of a
-given record being 1. ```python # Small example dataset from seaborn import
-load_dataset df = load_dataset("titanic") X = df.select_dtypes("number").drop
-(columns=["survived"]) y = df["survived"] # Initialize a booster with defaults.
-from forust import GradientBooster model = GradientBooster
-(objective_type="LogLoss") model.fit(X, y) # Predict on data model.predict
-(X.head()) # array([-1.94919663, 2.25863229, 0.32963671, 2.48732194, -
-3.00371813]) # predict contributions model.predict_contributions(X.head()) #
-array([[-0.63014213, 0.33880048, -0.16520798, -0.07798772, -0.85083578, # -
-1.07720813], # [ 1.05406709, 0.08825999, 0.21662544, -0.12083538, 0.35209258, #
--1.07720813], ``` The `fit` method accepts the following arguments. - `X` ***
-(FrameLike)***: Either a pandas DataFrame, or a 2 dimensional numpy array, with
-numeric data. - `y` ***(ArrayLike)***: Either a pandas Series, or a 1
-dimensional numpy array. If "LogLoss" was the objective type specified, then
-this should only contain 1 or 0 values, where 1 is the positive class being
-predicted. If "SquaredLoss" is the objective type, then any continuous variable
-can be provided. - `sample_weight` ***(Optional[ArrayLike], optional)***:
-Instance weights to use when training the model. If None is passed, a weight of
-1 will be used for every record. Defaults to None. The predict method accepts
-the following arguments. - `X` ***(FrameLike)***: Either a pandas DataFrame, or
-a 2 dimensional numpy array, with numeric data. - `parallel` ***(Optional
-[bool], optional)***: Optionally specify if the predict function should run in
-parallel on multiple threads. If `None` is passed, the `parallel` attribute of
-the booster will be used. Defaults to `None`. The `predict_contributions`
-method will predict with the fitted booster on new data, returning the feature
+be enforced on any variable. Defaults to `None`. - `subsample` ***(float,
+optional)***: Percent of records to randomly sample at each iteration when
+training a tree. Defaults to 1.0, meaning all data is used for training. -
+`seed` ***(integer, optional)***: Integer value used to seed any randomness
+used in the algorithm. Defaults to 0. - `missing` ***(float, optional)***:
+Value to consider missing, when training and predicting with the booster.
+Defaults to `np.nan`. ### Training and Predicting Once, the booster has been
+initialized, it can be fit on a provided dataset, and performance field. After
+fitting, the model can be used to predict on a dataset. In the case of this
+example, the predictions are the log odds of a given record being 1. ```python
+# Small example dataset from seaborn import load_dataset df = load_dataset
+("titanic") X = df.select_dtypes("number").drop(columns=["survived"]) y = df
+["survived"] # Initialize a booster with defaults. from forust import
+GradientBooster model = GradientBooster(objective_type="LogLoss") model.fit(X,
+y) # Predict on data model.predict(X.head()) # array([-1.94919663, 2.25863229,
+0.32963671, 2.48732194, -3.00371813]) # predict contributions
+model.predict_contributions(X.head()) # array([[-0.63014213, 0.33880048, -
+0.16520798, -0.07798772, -0.85083578, # -1.07720813], # [ 1.05406709,
+0.08825999, 0.21662544, -0.12083538, 0.35209258, # -1.07720813], ``` The `fit`
+method accepts the following arguments. - `X` ***(FrameLike)***: Either a
+pandas DataFrame, or a 2 dimensional numpy array, with numeric data. - `y` ***
+(ArrayLike)***: Either a pandas Series, or a 1 dimensional numpy array. If
+"LogLoss" was the objective type specified, then this should only contain 1 or
+0 values, where 1 is the positive class being predicted. If "SquaredLoss" is
+the objective type, then any continuous variable can be provided. -
+`sample_weight` ***(Optional[ArrayLike], optional)***: Instance weights to use
+when training the model. If None is passed, a weight of 1 will be used for
+every record. Defaults to None. The predict method accepts the following
+arguments. - `X` ***(FrameLike)***: Either a pandas DataFrame, or a 2
+dimensional numpy array, with numeric data. - `parallel` ***(Optional[bool],
+optional)***: Optionally specify if the predict function should run in parallel
+on multiple threads. If `None` is passed, the `parallel` attribute of the
+booster will be used. Defaults to `None`. The `predict_contributions` method
+will predict with the fitted booster on new data, returning the feature
 contribution matrix. The last column is the bias term. - `X` ***(FrameLike)***:
 Either a pandas DataFrame, or a 2 dimensional numpy array, with numeric data. -
 `parallel` ***(Optional[bool], optional)***: Optionally specify if the predict
 function should run in parallel on multiple threads. If `None` is passed, the
 `parallel` attribute of the booster will be used. Defaults to `None`. ###
 Inspecting the Model Once the booster has been fit, each individual tree
 structure can be retrieved in text form, using the `text_dump` method. This
```

### Comparing `forust-0.2.2/forust/__init__.py` & `forust-0.2.3/forust/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -67,14 +67,20 @@
 
     def json_dump(self) -> str:
         raise NotImplementedError()
 
     def get_params(self) -> dict[str, Any]:
         raise NotImplementedError()
 
+    def insert_metadata(self, key: str, value: str) -> None:
+        raise NotImplementedError()
+
+    def get_metadata(self, key: str) -> str:
+        raise NotImplementedError()
+
 
 class GradientBooster:
     def __init__(
         self,
         objective_type: str = "LogLoss",
         iterations: int = 100,
         learning_rate: float = 0.3,
@@ -84,14 +90,17 @@
         gamma: float = 0.0,
         min_leaf_weight: float = 1.0,
         base_score: float = 0.5,
         nbins: int = 256,
         parallel: bool = True,
         allow_missing_splits: bool = True,
         monotone_constraints: Union[dict[Any, int], None] = None,
+        subsample: float = 1.0,
+        seed: int = 0,
+        missing: float = np.nan,
     ):
         """Gradient Booster Class, used to generate gradient boosted decision tree ensembles.
 
         Args:
             objective_type (str, optional): The name of objective function used to optimize.
                 Valid options include "LogLoss" to use logistic loss as the objective function
                 (binary classification), or "SquaredLoss" to use Squared Error as the objective
@@ -128,14 +137,20 @@
                 a numpy array, or a feature name if it will be fit on a pandas Dataframe. The values of
                 the dictionary should be an integer value of -1, 1, or 0 to specify the relationship
                 that should be estimated between the respective feature and the target variable.
                 Use a value of -1 to enforce a negative relationship, 1 a positive relationship,
                 and 0 will enforce no specific relationship at all. Features not included in the
                 mapping will not have any constraint applied. If `None` is passed no constraints
                 will be enforced on any variable.  Defaults to `None`.
+            subsample (float, optional): Percent of records to randomly sample at each iteration when
+                training a tree. Defaults to 1.0, meaning all data is used to training.
+            seed (integer, optional): Integer value used to seed any randomness used in the
+                algorithm. Defaults to 0.
+            missing (float, optional): Value to consider missing, when training and predicting
+                with the booster. Defaults to `np.nan`.
 
         Raises:
             TypeError: Raised if an invalid dtype is passed.
         """
         booster = CrateGradientBooster(
             objective_type=objective_type,
             iterations=iterations,
@@ -146,14 +161,17 @@
             gamma=gamma,
             min_leaf_weight=min_leaf_weight,
             base_score=base_score,
             nbins=nbins,
             parallel=parallel,
             allow_missing_splits=allow_missing_splits,
             monotone_constraints={},
+            subsample=subsample,
+            seed=seed,
+            missing=missing,
         )
         monotone_constraints_ = (
             {} if monotone_constraints is None else monotone_constraints
         )
         self.booster = cast(BoosterType, booster)
         self.objective_type = objective_type
         self.iterations = iterations
@@ -164,14 +182,17 @@
         self.gamma = gamma
         self.min_leaf_weight = min_leaf_weight
         self.base_score = base_score
         self.nbins = nbins
         self.parallel = parallel
         self.allow_missing_splits = (allow_missing_splits,)
         self.monotone_constraints = monotone_constraints_
+        self.subsample = subsample
+        self.seed = seed
+        self.missing = missing
 
     def fit(
         self,
         X: FrameLike,
         y: ArrayLike,
         sample_weight: Union[ArrayLike, None] = None,
     ):
@@ -183,29 +204,37 @@
                 was the objective type specified, then this should only contain 1 or 0 values,
                 where 1 is the positive class being predicted. If "SquaredLoss" is the
                 objective type, then any continuous variable can be provided.
             sample_weight (Union[ArrayLike, None], optional): Instance weights to use when
                 training the model. If None is passed, a weight of 1 will be used for every record.
                 Defaults to None.
         """
-        X_ = X.to_numpy() if isinstance(X, pd.DataFrame) else X
+        if isinstance(X, pd.DataFrame):
+            X_ = X.to_numpy()
+            self.feature_names_in_ = X.columns.to_list()
+            self.insert_metadata("feature_names_in_", str(self.feature_names_in_))
+        else:
+            # Assume it's a numpy array.
+            X_ = X
         if not np.issubdtype(X_.dtype, "float64"):
             X_ = X_.astype(dtype="float64", copy=False)
 
         y_ = y.to_numpy() if isinstance(y, pd.Series) else y
+
         if not np.issubdtype(y_.dtype, "float64"):
             y_ = y_.astype(dtype="float64", copy=False)
 
         if sample_weight is None:
             sample_weight = np.ones(y_.shape, dtype="float64")
         sample_weight_ = (
             sample_weight.to_numpy()
             if isinstance(sample_weight, pd.Series)
             else sample_weight
         )
+
         if not np.issubdtype(sample_weight_.dtype, "float64"):
             sample_weight_ = sample_weight_.astype("float64", copy=False)
 
         # Convert the monotone constraints into the form needed
         # by the rust code.
         monotone_constraints_ = self._standardize_monotonicity_map(X)
         self.booster.monotone_constraints = monotone_constraints_
@@ -373,7 +402,27 @@
         X: Union[pd.DataFrame, np.ndarray],
     ) -> dict[int, Any]:
         if isinstance(X, np.ndarray):
             return self.monotone_constraints
         else:
             feature_map = {f: i for i, f in enumerate(X.columns)}
             return {feature_map[f]: v for f, v in self.monotone_constraints.items()}
+
+    def insert_metadata(self, key: str, value: str):
+        """Insert data into the models metadata, this will be saved on the booster object.
+
+        Args:
+            key (str): Key to give the inserted value in the metadata.
+            value (str): Value to assign the the key.
+        """
+        self.booster.insert_metadata(key=key, value=value)
+
+    def get_metadata(self, key: str) -> str:
+        """Get the value associated with a given key, on the boosters metadata.
+
+        Args:
+            key (str): Key of item in metadata.
+
+        Returns:
+            str: Value associated with the provided key in the boosters metadata.
+        """
+        return self.booster.get_metadata(key=key)
```

### Comparing `forust-0.2.2/pyproject.toml` & `forust-0.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `forust-0.2.2/scratch.py` & `forust-0.2.3/scratch.py`

 * *Files identical despite different names*

### Comparing `forust-0.2.2/src/lib.rs` & `forust-0.2.3/src/lib.rs`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 use forust_ml::constraints::{Constraint, ConstraintMap};
 use forust_ml::data::Matrix;
 use forust_ml::gradientbooster::GradientBooster as CrateGradientBooster;
 use forust_ml::objective::ObjectiveType;
 use forust_ml::utils::percentiles as crate_percentiles;
 use numpy::{IntoPyArray, PyArray1, PyReadonlyArray1};
-use pyo3::exceptions::PyValueError;
+use pyo3::exceptions::{PyKeyError, PyValueError};
 use pyo3::prelude::*;
 use pyo3::types::IntoPyDict;
 use pyo3::types::PyType;
 use std::collections::HashMap;
 
 fn int_map_to_constraint_map(int_map: HashMap<usize, i8>) -> PyResult<ConstraintMap> {
     let mut constraints: ConstraintMap = HashMap::new();
@@ -45,14 +45,17 @@
         gamma: f32,
         min_leaf_weight: f32,
         base_score: f64,
         nbins: u16,
         parallel: bool,
         allow_missing_splits: bool,
         monotone_constraints: HashMap<usize, i8>,
+        subsample: f32,
+        seed: u64,
+        missing: f64,
     ) -> PyResult<Self> {
         let constraints = int_map_to_constraint_map(monotone_constraints)?;
         let objective_ = match objective_type {
             "LogLoss" => Ok(ObjectiveType::LogLoss),
             "SquaredLoss" => Ok(ObjectiveType::SquaredLoss),
             _ => Err(PyValueError::new_err(format!("Not a valid objective type passed, expected one of 'LogLoss', 'SquaredLoss', but '{}' was provided.", objective_type))),
         }?;
@@ -66,14 +69,17 @@
             gamma,
             min_leaf_weight,
             base_score,
             nbins,
             parallel,
             allow_missing_splits,
             Some(constraints),
+            subsample,
+            seed,
+            missing,
         );
         Ok(GradientBooster { booster })
     }
 
     #[setter]
     fn set_monotone_constraints(&mut self, value: HashMap<usize, i8>) -> PyResult<()> {
         let map = int_map_to_constraint_map(value)?;
@@ -151,14 +157,28 @@
     pub fn json_dump(&self) -> PyResult<String> {
         match self.booster.json_dump() {
             Ok(m) => Ok(m),
             Err(e) => Err(PyValueError::new_err(e.to_string())),
         }
     }
 
+    pub fn insert_metadata(&mut self, key: String, value: String) -> PyResult<()> {
+        self.booster.insert_metadata(key, value);
+        Ok(())
+    }
+
+    pub fn get_metadata(&self, key: String) -> PyResult<String> {
+        match self.booster.get_metadata(&key) {
+            Some(m) => Ok(m),
+            None => Err(PyKeyError::new_err(
+                format!("No value associated with provided key {}", key).to_string(),
+            )),
+        }
+    }
+
     #[classmethod]
     pub fn load_booster(_: &PyType, path: String) -> PyResult<Self> {
         let booster = match CrateGradientBooster::load_booster(path.as_str()) {
             Ok(m) => Ok(m),
             Err(e) => Err(PyValueError::new_err(e.to_string())),
         }?;
         Ok(GradientBooster { booster })
@@ -209,14 +229,17 @@
             ("nbins", self.booster.nbins.to_object(py)),
             ("parallel", self.booster.parallel.to_object(py)),
             (
                 "allow_missing_splits",
                 self.booster.allow_missing_splits.to_object(py),
             ),
             ("monotone_constraints", constraints.to_object(py)),
+            ("subsample", self.booster.subsample.to_object(py)),
+            ("seed", self.booster.seed.to_object(py)),
+            ("missing", self.booster.missing.to_object(py)),
         ];
         let dict = key_vals.into_py_dict(py);
         Ok(dict.to_object(py))
     }
 }
 
 #[pyfunction]
```

### Comparing `forust-0.2.2/tests/test_booster.py` & `forust-0.2.3/tests/test_booster.py`

 * *Files 24% similar despite different names*

```diff
@@ -69,15 +69,15 @@
         learning_rate=0.3,
         max_depth=5,
         l2=1,
         min_leaf_weight=1,
         gamma=1,
         objective_type="LogLoss",
         nbins=500,
-        parallel=False,
+        parallel=True,
     )
     fmod.fit(X, y=y)
     fmod_preds = fmod.predict(X)
     assert np.allclose(fmod_preds, xmod_preds, atol=0.00001)
 
 
 def test_booster_to_xgboosts_with_missing_sl(X_y):
@@ -105,21 +105,125 @@
         learning_rate=0.3,
         max_depth=5,
         l2=1,
         min_leaf_weight=1,
         gamma=1,
         objective_type="SquaredLoss",
         nbins=500,
-        parallel=False,
+        parallel=True,
     )
     fmod.fit(X, y=y)
     fmod_preds = fmod.predict(X)
     assert np.allclose(fmod_preds, xmod_preds, atol=0.00001)
 
 
+def test_booster_with_new_missing(X_y):
+    X, y = X_y
+    X = X
+    fmod = GradientBooster(
+        iterations=100,
+        learning_rate=0.3,
+        max_depth=5,
+        l2=1,
+        min_leaf_weight=1,
+        gamma=1,
+        objective_type="LogLoss",
+        nbins=500,
+        parallel=True,
+    )
+    fmod.fit(X, y=y)
+    fmod_preds = fmod.predict(X)
+
+    Xm = X.copy().fillna(-9999)
+    fmod2 = GradientBooster(
+        iterations=100,
+        learning_rate=0.3,
+        max_depth=5,
+        l2=1,
+        min_leaf_weight=1,
+        gamma=1,
+        objective_type="LogLoss",
+        nbins=500,
+        parallel=True,
+        missing=-9999,
+    )
+    fmod2.fit(Xm, y=y)
+    fmod_preds2 = fmod2.predict(Xm)
+    assert np.allclose(fmod_preds, fmod_preds2, atol=0.00001)
+
+
+def test_booster_with_seed(X_y):
+    X, y = X_y
+    X = X
+    fmod1 = GradientBooster(
+        iterations=100,
+        learning_rate=0.3,
+        max_depth=5,
+        l2=1,
+        min_leaf_weight=1,
+        gamma=1,
+        objective_type="LogLoss",
+        nbins=500,
+        parallel=True,
+        subsample=0.5,
+        seed=0,
+    )
+    fmod1.fit(X, y=y)
+    fmod1_preds = fmod1.predict(X)
+
+    fmod2 = GradientBooster(
+        iterations=100,
+        learning_rate=0.3,
+        max_depth=5,
+        l2=1,
+        min_leaf_weight=1,
+        gamma=1,
+        objective_type="LogLoss",
+        nbins=500,
+        parallel=True,
+        subsample=0.5,
+        seed=0,
+    )
+    fmod2.fit(X, y=y)
+    fmod2_preds = fmod2.predict(X)
+    assert np.allclose(fmod2_preds, fmod1_preds, atol=0.0000001)
+
+    fmod3 = GradientBooster(
+        iterations=100,
+        learning_rate=0.3,
+        max_depth=5,
+        l2=1,
+        min_leaf_weight=1,
+        gamma=1,
+        objective_type="LogLoss",
+        nbins=500,
+        parallel=True,
+        subsample=0.5,
+        seed=1,
+    )
+    fmod3.fit(X, y=y)
+    fmod3_preds = fmod3.predict(X)
+    assert not np.allclose(fmod3_preds, fmod2_preds, atol=0.0000001)
+
+    fmod4 = GradientBooster(
+        iterations=100,
+        learning_rate=0.3,
+        max_depth=5,
+        l2=1,
+        min_leaf_weight=1,
+        gamma=1,
+        objective_type="LogLoss",
+        nbins=500,
+        parallel=True,
+    )
+    fmod4.fit(X, y=y)
+    fmod4_preds = fmod4.predict(X)
+    assert not np.allclose(fmod4_preds, fmod2_preds, atol=0.00001)
+
+
 def test_booster_to_xgboosts_weighted(X_y):
     X, y = X_y
     X = X.fillna(0)
     w = X["fare"].to_numpy() + 1
     xmod = XGBClassifier(
         n_estimators=100,
         learning_rate=0.3,
@@ -158,15 +262,15 @@
         learning_rate=0.3,
         max_depth=5,
         l2=1,
         min_leaf_weight=1,
         gamma=1,
         objective_type="SquaredLoss",
         nbins=500,
-        parallel=False,
+        parallel=True,
     )
     fmod.fit(X, y=y)
     fmod_preds = fmod.predict(X)
     fmod.save_booster(f64_model_path)
     fmod_loaded = GradientBooster.load_booster(f64_model_path)
     assert all(fmod_preds == fmod_loaded.predict(X))
 
@@ -179,15 +283,15 @@
         learning_rate=0.3,
         max_depth=5,
         l2=1,
         min_leaf_weight=1,
         gamma=1,
         objective_type="LogLoss",
         nbins=500,
-        parallel=False,
+        parallel=True,
     )
     fmod.fit(X, y=y)
     fmod_preds = fmod.predict(X)
     fmod.save_booster(f64_model_path)
     fmod_loaded = GradientBooster.load_booster(f64_model_path)
     assert all(fmod_preds == fmod_loaded.predict(X))
 
@@ -203,15 +307,15 @@
         learning_rate=0.3,
         max_depth=5,
         l2=1,
         min_leaf_weight=1,
         gamma=1,
         objective_type="SquaredLoss",
         nbins=500,
-        parallel=False,
+        parallel=True,
         monotone_constraints=mono_,
     )
     fmod.fit(X, y=y)
     fmod_preds = fmod.predict(X)
     fmod.save_booster(f64_model_path)
     fmod_loaded = GradientBooster.load_booster(f64_model_path)
     assert all(fmod_preds == fmod_loaded.predict(X))
@@ -225,15 +329,15 @@
         learning_rate=0.3,
         max_depth=5,
         l2=1,
         min_leaf_weight=1,
         gamma=1,
         objective_type="LogLoss",
         nbins=500,
-        parallel=False,
+        parallel=True,
         monotone_constraints=mono_,
     )
     fmod.fit(X, y=y)
     fmod_preds = fmod.predict(X)
     fmod.save_booster(f64_model_path)
     fmod_loaded = GradientBooster.load_booster(f64_model_path)
     assert all(fmod_preds == fmod_loaded.predict(X))
@@ -248,15 +352,15 @@
         learning_rate=0.3,
         max_depth=5,
         l2=1,
         min_leaf_weight=1,
         gamma=1,
         objective_type="SquaredLoss",
         nbins=500,
-        parallel=False,
+        parallel=True,
         monotone_constraints=mono_,
     )
     fmod.fit(X, y=y)
     for f, m in mono_.items():
         p_d = fmod.partial_dependence(X, feature=f)
         p_d = p_d[~np.isnan(p_d[:, 0])]
         if m < 0:
@@ -273,15 +377,15 @@
         learning_rate=0.3,
         max_depth=5,
         l2=1,
         min_leaf_weight=1,
         gamma=1,
         objective_type="LogLoss",
         nbins=500,
-        parallel=False,
+        parallel=True,
         base_score=0.5,
     )
     fmod.fit(X, y=y)
     fmod_preds = fmod.predict(X)
     fmod_contribs = fmod.predict_contributions(X)
     fmod_preds[~np.isclose(fmod_contribs.sum(1), fmod_preds, rtol=5)]
     fmod_contribs.sum(1)[~np.isclose(fmod_contribs.sum(1), fmod_preds, rtol=5)]
@@ -305,7 +409,36 @@
     xmod_preds = xmod.predict(X, output_margin=True)
     import xgboost as xgb
 
     xmod_contribs = xmod.get_booster().predict(
         xgb.DMatrix(X), approx_contribs=True, pred_contribs=True
     )
     assert np.allclose(fmod_contribs, xmod_contribs, atol=0.000001)
+
+
+def test_booster_metadata(X_y, tmp_path):
+    f64_model_path = tmp_path / "modelf64_sl.json"
+    X, y = X_y
+    X = X
+    fmod = GradientBooster(
+        iterations=100,
+        learning_rate=0.3,
+        max_depth=5,
+        l2=1,
+        min_leaf_weight=1,
+        gamma=1,
+        objective_type="SquaredLoss",
+        nbins=500,
+        parallel=True,
+    )
+    fmod.fit(X, y=y)
+    fmod_preds = fmod.predict(X)
+    fmod.save_booster(f64_model_path)
+    fmod.insert_metadata("test-info", "some-info")
+    assert fmod.get_metadata("test-info") == "some-info"
+    fmod.save_booster(f64_model_path)
+
+    loaded = GradientBooster.load_booster(f64_model_path)
+    assert loaded.get_metadata("test-info") == "some-info"
+
+    with pytest.raises(KeyError):
+        loaded.get_metadata("No-key")
```

### Comparing `forust-0.2.2/LICENSE` & `forust-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `forust-0.2.2/PKG-INFO` & `forust-0.2.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: forust
-Version: 0.2.2
+Version: 0.2.3
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: numpy>=1.21
 Requires-Dist: pandas>=1.3
 Requires-Dist: maturin; extra == 'dev'
 Requires-Dist: pytest; extra == 'dev'
@@ -43,15 +43,15 @@
 The package can be installed directly from [pypi](https://pypi.org/project/forust/).
 ```shell
 pip install forust
 ```
 
 To use in a rust project add the following to your Cargo.toml file.
 ```toml
-forust-ml = "0.2.2"
+forust-ml = "0.2.3"
 ```
 
 ## Usage
 The `GradientBooster` class is currently the only public facing class in the package, and can be used to train gradient boosted decision tree ensembles with multiple objective functions.
 
 It can be initialized with the following arguments.
 
@@ -79,14 +79,19 @@
     a smaller number, will result in faster training time, while potentially sacrificing
     accuracy. If there are more bins, than unique values in a column, all unique values
     will be used. Defaults to 256.
  - `parallel` ***(bool, optional)***: Should multiple cores be used when training and predicting
     with this model? Defaults to `True`.
  - `allow_missing_splits` ***(bool, optional)***: Allow for splits to be made such that all missing values go down one branch, and all non-missing values go down the other, if this results in the greatest reduction of loss. If this is false, splits will only be made on non missing values. Defaults to `True`.
  - `monotone_constraints` ***(dict[Any, int], optional)***: Constraints that are used to enforce a specific relationship between the training features and the target variable. A dictionary should be provided where the keys are the feature index value if the model will be fit on a numpy array, or a feature name if it will be fit on a pandas Dataframe. The values of the dictionary should be an integer value of -1, 1, or 0 to specify the relationship that should be estimated between the respective feature and the target variable. Use a value of -1 to enforce a negative relationship, 1 a positive relationship, and 0 will enforce no specific relationship at all. Features not included in the mapping will not have any constraint applied. If `None` is passed no constraints will be enforced on any variable.  Defaults to `None`.
+ - `subsample` ***(float, optional)***: Percent of records to randomly sample at each iteration when
+      training a tree. Defaults to 1.0, meaning all data is used for training.
+ - `seed` ***(integer, optional)***: Integer value used to seed any randomness used in the
+      algorithm. Defaults to 0.
+ - `missing` ***(float, optional)***: Value to consider missing, when training and predicting with the booster. Defaults to `np.nan`.
 
 ### Training and Predicting
 
 Once, the booster has been initialized, it can be fit on a provided dataset, and performance field. After fitting, the model can be used to predict on a dataset.
 In the case of this example, the predictions are the log odds of a given record being 1.
 
 ```python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: forust Version: 0.2.2 Classifier: Programming
+Metadata-Version: 2.1 Name: forust Version: 0.2.3 Classifier: Programming
 Language :: Rust Classifier: Programming Language :: Python :: Implementation
 :: CPython Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: numpy>=1.21 Requires-Dist: pandas>=1.3 Requires-Dist: maturin;
 extra == 'dev' Requires-Dist: pytest; extra == 'dev' Requires-Dist: seaborn;
 extra == 'dev' Requires-Dist: xgboost==1.6.1; extra == 'dev' Requires-Dist:
 scikit-learn; extra == 'dev' Provides-Extra: dev License-File: LICENSE Summary:
 A lightweight gradient boosting implementation in Rust. Keywords:
@@ -24,15 +24,15 @@
 understand the XGBoost algorithm, additionally to have a fun project to work on
 in rust, and because I wanted to be able to experiment with adding new features
 to the algorithm in a smaller simpler codebase. All of the rust code for the
 package can be found in the [src](src/) directory, while all of the python
 wrapper code is in the [py-forust](py-forust/) directory. ## Installation The
 package can be installed directly from [pypi](https://pypi.org/project/forust/
 ). ```shell pip install forust ``` To use in a rust project add the following
-to your Cargo.toml file. ```toml forust-ml = "0.2.2" ``` ## Usage The
+to your Cargo.toml file. ```toml forust-ml = "0.2.3" ``` ## Usage The
 `GradientBooster` class is currently the only public facing class in the
 package, and can be used to train gradient boosted decision tree ensembles with
 multiple objective functions. It can be initialized with the following
 arguments. - `objective_type` ***(str, optional)***: The name of objective
 function used to optimize. Valid options include "LogLoss" to use logistic loss
 as the objective function (binary classification), or "SquaredLoss" to use
 Squared Error as the objective function (continuous regression). Defaults to
@@ -67,42 +67,48 @@
 index value if the model will be fit on a numpy array, or a feature name if it
 will be fit on a pandas Dataframe. The values of the dictionary should be an
 integer value of -1, 1, or 0 to specify the relationship that should be
 estimated between the respective feature and the target variable. Use a value
 of -1 to enforce a negative relationship, 1 a positive relationship, and 0 will
 enforce no specific relationship at all. Features not included in the mapping
 will not have any constraint applied. If `None` is passed no constraints will
-be enforced on any variable. Defaults to `None`. ### Training and Predicting
-Once, the booster has been initialized, it can be fit on a provided dataset,
-and performance field. After fitting, the model can be used to predict on a
-dataset. In the case of this example, the predictions are the log odds of a
-given record being 1. ```python # Small example dataset from seaborn import
-load_dataset df = load_dataset("titanic") X = df.select_dtypes("number").drop
-(columns=["survived"]) y = df["survived"] # Initialize a booster with defaults.
-from forust import GradientBooster model = GradientBooster
-(objective_type="LogLoss") model.fit(X, y) # Predict on data model.predict
-(X.head()) # array([-1.94919663, 2.25863229, 0.32963671, 2.48732194, -
-3.00371813]) # predict contributions model.predict_contributions(X.head()) #
-array([[-0.63014213, 0.33880048, -0.16520798, -0.07798772, -0.85083578, # -
-1.07720813], # [ 1.05406709, 0.08825999, 0.21662544, -0.12083538, 0.35209258, #
--1.07720813], ``` The `fit` method accepts the following arguments. - `X` ***
-(FrameLike)***: Either a pandas DataFrame, or a 2 dimensional numpy array, with
-numeric data. - `y` ***(ArrayLike)***: Either a pandas Series, or a 1
-dimensional numpy array. If "LogLoss" was the objective type specified, then
-this should only contain 1 or 0 values, where 1 is the positive class being
-predicted. If "SquaredLoss" is the objective type, then any continuous variable
-can be provided. - `sample_weight` ***(Optional[ArrayLike], optional)***:
-Instance weights to use when training the model. If None is passed, a weight of
-1 will be used for every record. Defaults to None. The predict method accepts
-the following arguments. - `X` ***(FrameLike)***: Either a pandas DataFrame, or
-a 2 dimensional numpy array, with numeric data. - `parallel` ***(Optional
-[bool], optional)***: Optionally specify if the predict function should run in
-parallel on multiple threads. If `None` is passed, the `parallel` attribute of
-the booster will be used. Defaults to `None`. The `predict_contributions`
-method will predict with the fitted booster on new data, returning the feature
+be enforced on any variable. Defaults to `None`. - `subsample` ***(float,
+optional)***: Percent of records to randomly sample at each iteration when
+training a tree. Defaults to 1.0, meaning all data is used for training. -
+`seed` ***(integer, optional)***: Integer value used to seed any randomness
+used in the algorithm. Defaults to 0. - `missing` ***(float, optional)***:
+Value to consider missing, when training and predicting with the booster.
+Defaults to `np.nan`. ### Training and Predicting Once, the booster has been
+initialized, it can be fit on a provided dataset, and performance field. After
+fitting, the model can be used to predict on a dataset. In the case of this
+example, the predictions are the log odds of a given record being 1. ```python
+# Small example dataset from seaborn import load_dataset df = load_dataset
+("titanic") X = df.select_dtypes("number").drop(columns=["survived"]) y = df
+["survived"] # Initialize a booster with defaults. from forust import
+GradientBooster model = GradientBooster(objective_type="LogLoss") model.fit(X,
+y) # Predict on data model.predict(X.head()) # array([-1.94919663, 2.25863229,
+0.32963671, 2.48732194, -3.00371813]) # predict contributions
+model.predict_contributions(X.head()) # array([[-0.63014213, 0.33880048, -
+0.16520798, -0.07798772, -0.85083578, # -1.07720813], # [ 1.05406709,
+0.08825999, 0.21662544, -0.12083538, 0.35209258, # -1.07720813], ``` The `fit`
+method accepts the following arguments. - `X` ***(FrameLike)***: Either a
+pandas DataFrame, or a 2 dimensional numpy array, with numeric data. - `y` ***
+(ArrayLike)***: Either a pandas Series, or a 1 dimensional numpy array. If
+"LogLoss" was the objective type specified, then this should only contain 1 or
+0 values, where 1 is the positive class being predicted. If "SquaredLoss" is
+the objective type, then any continuous variable can be provided. -
+`sample_weight` ***(Optional[ArrayLike], optional)***: Instance weights to use
+when training the model. If None is passed, a weight of 1 will be used for
+every record. Defaults to None. The predict method accepts the following
+arguments. - `X` ***(FrameLike)***: Either a pandas DataFrame, or a 2
+dimensional numpy array, with numeric data. - `parallel` ***(Optional[bool],
+optional)***: Optionally specify if the predict function should run in parallel
+on multiple threads. If `None` is passed, the `parallel` attribute of the
+booster will be used. Defaults to `None`. The `predict_contributions` method
+will predict with the fitted booster on new data, returning the feature
 contribution matrix. The last column is the bias term. - `X` ***(FrameLike)***:
 Either a pandas DataFrame, or a 2 dimensional numpy array, with numeric data. -
 `parallel` ***(Optional[bool], optional)***: Optionally specify if the predict
 function should run in parallel on multiple threads. If `None` is passed, the
 `parallel` attribute of the booster will be used. Defaults to `None`. ###
 Inspecting the Model Once the booster has been fit, each individual tree
 structure can be retrieved in text form, using the `text_dump` method. This
```

