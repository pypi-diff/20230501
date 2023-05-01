# Comparing `tmp/palmers_preprocess-0.0.6.tar.gz` & `tmp/palmers_preprocess-0.0.7.tar.gz`

## Comparing `palmers_preprocess-0.0.6.tar` & `palmers_preprocess-0.0.7.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.6/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.6/src/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.6/src/palmers_preprocessing/__init__.py
--rw-r--r--   0        0        0     5181 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.6/src/palmers_preprocessing/clearml_data_handler.py
--rw-r--r--   0        0        0     6784 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.6/src/palmers_preprocessing/config.py
--rw-r--r--   0        0        0    43620 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.6/src/palmers_preprocessing/events_handler.py
--rw-r--r--   0        0        0     5196 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.6/src/palmers_preprocessing/lags_feature_handler.py
--rw-r--r--   0        0        0     7475 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.6/src/palmers_preprocessing/preprocessor.py
--rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.6/src/palmers_preprocessing/regular_data_handler.py
--rw-r--r--   0        0        0     7669 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.6/src/palmers_preprocessing/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.6/src/palmers_preprocessing/features/__init__.py
--rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.6/src/palmers_preprocessing/features/config.py
--rw-r--r--   0        0        0     8887 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.6/src/palmers_preprocessing/features/cumulative_features.py
--rw-r--r--   0        0        0     9093 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.6/src/palmers_preprocessing/features/event_features.py
--rw-r--r--   0        0        0     8418 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.6/src/palmers_preprocessing/features/future_features.py
--rw-r--r--   0        0        0     4108 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.6/src/palmers_preprocessing/features/lags_features.py
--rw-r--r--   0        0        0     5404 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.6/src/palmers_preprocessing/features/weather_features.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.6/src/palmers_preprocessing/tests/__init__.py
--rw-r--r--   0        0        0   719548 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.6/src/palmers_preprocessing/tests/config_batch_dict.py
--rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.6/src/palmers_preprocessing/tests/event_feature_test.py
--rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.6/src/palmers_preprocessing/tests/features_test.py
--rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.6/src/palmers_preprocessing/tests/lags_features_test.py
--rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.6/src/palmers_preprocessing/tests/preprocessor_test.py
--rw-r--r--   0        0        0    50890 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.6/src/palmers_preprocessing/tests/sanity_checks.py
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.6/src/palmers_preprocessing/tests/test_todelete.py
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.6/src/palmers_preprocessing/tests/weather_test.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.6/.gitignore
--rw-r--r--   0        0        0    11558 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.6/LICENSE
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.6/README.md
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.6/pyproject.toml
--rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.7/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.7/src/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.7/src/palmers_preprocessing/__init__.py
+-rw-r--r--   0        0        0     5181 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.7/src/palmers_preprocessing/clearml_data_handler.py
+-rw-r--r--   0        0        0     6784 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.7/src/palmers_preprocessing/config.py
+-rw-r--r--   0        0        0    43620 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.7/src/palmers_preprocessing/events_handler.py
+-rw-r--r--   0        0        0     5196 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.7/src/palmers_preprocessing/lags_feature_handler.py
+-rw-r--r--   0        0        0     7475 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.7/src/palmers_preprocessing/preprocessor.py
+-rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.7/src/palmers_preprocessing/regular_data_handler.py
+-rw-r--r--   0        0        0     7669 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.7/src/palmers_preprocessing/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.7/src/palmers_preprocessing/features/__init__.py
+-rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.7/src/palmers_preprocessing/features/config.py
+-rw-r--r--   0        0        0     8923 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.7/src/palmers_preprocessing/features/cumulative_features.py
+-rw-r--r--   0        0        0     9093 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.7/src/palmers_preprocessing/features/event_features.py
+-rw-r--r--   0        0        0     8418 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.7/src/palmers_preprocessing/features/future_features.py
+-rw-r--r--   0        0        0     4142 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.7/src/palmers_preprocessing/features/lags_features.py
+-rw-r--r--   0        0        0     5404 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.7/src/palmers_preprocessing/features/weather_features.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.7/src/palmers_preprocessing/tests/__init__.py
+-rw-r--r--   0        0        0   719548 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.7/src/palmers_preprocessing/tests/config_batch_dict.py
+-rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.7/src/palmers_preprocessing/tests/event_feature_test.py
+-rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.7/src/palmers_preprocessing/tests/features_test.py
+-rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.7/src/palmers_preprocessing/tests/lags_features_test.py
+-rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.7/src/palmers_preprocessing/tests/preprocessor_test.py
+-rw-r--r--   0        0        0    50890 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.7/src/palmers_preprocessing/tests/sanity_checks.py
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.7/src/palmers_preprocessing/tests/test_todelete.py
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.7/src/palmers_preprocessing/tests/weather_test.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.7/.gitignore
+-rw-r--r--   0        0        0    11558 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.7/LICENSE
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.7/README.md
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.7/PKG-INFO
```

### Comparing `palmers_preprocess-0.0.6/requirements.txt` & `palmers_preprocess-0.0.7/requirements.txt`

 * *Files identical despite different names*

### Comparing `palmers_preprocess-0.0.6/src/palmers_preprocessing/clearml_data_handler.py` & `palmers_preprocess-0.0.7/src/palmers_preprocessing/clearml_data_handler.py`

 * *Files identical despite different names*

### Comparing `palmers_preprocess-0.0.6/src/palmers_preprocessing/config.py` & `palmers_preprocess-0.0.7/src/palmers_preprocessing/config.py`

 * *Files identical despite different names*

### Comparing `palmers_preprocess-0.0.6/src/palmers_preprocessing/events_handler.py` & `palmers_preprocess-0.0.7/src/palmers_preprocessing/events_handler.py`

 * *Files identical despite different names*

### Comparing `palmers_preprocess-0.0.6/src/palmers_preprocessing/lags_feature_handler.py` & `palmers_preprocess-0.0.7/src/palmers_preprocessing/lags_feature_handler.py`

 * *Files identical despite different names*

### Comparing `palmers_preprocess-0.0.6/src/palmers_preprocessing/preprocessor.py` & `palmers_preprocess-0.0.7/src/palmers_preprocessing/preprocessor.py`

 * *Files identical despite different names*

### Comparing `palmers_preprocess-0.0.6/src/palmers_preprocessing/regular_data_handler.py` & `palmers_preprocess-0.0.7/src/palmers_preprocessing/regular_data_handler.py`

 * *Files identical despite different names*

### Comparing `palmers_preprocess-0.0.6/src/palmers_preprocessing/utils.py` & `palmers_preprocess-0.0.7/src/palmers_preprocessing/utils.py`

 * *Files identical despite different names*

### Comparing `palmers_preprocess-0.0.6/src/palmers_preprocessing/features/config.py` & `palmers_preprocess-0.0.7/src/palmers_preprocessing/features/config.py`

 * *Files identical despite different names*

### Comparing `palmers_preprocess-0.0.6/src/palmers_preprocessing/features/cumulative_features.py` & `palmers_preprocess-0.0.7/src/palmers_preprocessing/features/cumulative_features.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,21 +14,22 @@
     @classmethod
     def groupby_sum_sku_store(cls, df: pd.DataFrame, target_col: str, sku_store_col: List[str],
                               date_col: str) -> pd.DataFrame:
 
         df[target_col] = df[target_col].astype(np.float64)
         return df.groupby(sku_store_col + [date_col])[target_col].sum().reset_index()
 
+
     @classmethod
     def add_cumulative_sum_column_respect_time(cls, df: pd.DataFrame, target_col: str, sku_store_col: List[str],
                                                list_freq: List[str], date_col: str) -> pd.DataFrame:
         df[date_col] = pd.to_datetime(df[date_col])
         sku_store_col_name = '_'.join(sku_store_col)
         for freq in list_freq:
-            df_grouped = df.groupby(sku_store_col + [pd.Grouper(key=date_col, freq=freq)])[target_col].sum().reset_index()
+            df_grouped = df.groupby(sku_store_col + [pd.Grouper(key=date_col, freq=freq)])[target_col].sum(numeric_only=True).reset_index()
 
             df_grouped[f"sales_cumulative_{sku_store_col_name}_{freq}"] = df_grouped.groupby(sku_store_col)[
                 target_col].apply(lambda x: np.cumsum(x.shift(1).fillna(0)))
 
             df = df.merge(df_grouped.drop(columns=[target_col]), on=sku_store_col + [date_col], how='left').fillna(0)
             df = df.drop_duplicates(subset=sku_store_col + [date_col], keep='last')
         return df
@@ -36,15 +37,15 @@
     @classmethod
     def add_expected_value_column_respect_time(cls, df: pd.DataFrame, target_col: str, sku_store_col: List[str],
                                                list_freq: List[str], date_col: str) -> pd.DataFrame:
         sku_store_col_name = '_'.join(sku_store_col)
         df_expected = pd.DataFrame()
         df[target_col] = df[target_col].astype(np.float32)
         for freq in list_freq:
-            df_temp = df.groupby(sku_store_col + [pd.Grouper(key=date_col, freq=freq)])[target_col].sum().reset_index()
+            df_temp = df.groupby(sku_store_col + [pd.Grouper(key=date_col, freq=freq)])[target_col].sum(numeric_only=True).reset_index()
             df_temp[f"sales_expected_{sku_store_col_name}_{freq}"] = df_temp.groupby(sku_store_col)[
                 target_col].transform(
                 lambda x: x.mean()).shift(1).fillna(0)
             df_temp[f"sales_expected_{sku_store_col_name}_{freq}"] = df_temp[
                 f"sales_expected_{sku_store_col_name}_{freq}"].replace(
                 [np.inf, -np.inf], 0)
             df_expected = pd.concat(
```

### Comparing `palmers_preprocess-0.0.6/src/palmers_preprocessing/features/event_features.py` & `palmers_preprocess-0.0.7/src/palmers_preprocessing/features/event_features.py`

 * *Files identical despite different names*

### Comparing `palmers_preprocess-0.0.6/src/palmers_preprocessing/features/future_features.py` & `palmers_preprocess-0.0.7/src/palmers_preprocessing/features/future_features.py`

 * *Files identical despite different names*

### Comparing `palmers_preprocess-0.0.6/src/palmers_preprocessing/features/lags_features.py` & `palmers_preprocess-0.0.7/src/palmers_preprocessing/features/lags_features.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     def __init__(self):
         super().__init__()
 
     def create_all_stores_lags(self, store_data_df, predict_date):
         """
         This function assumes that store_data_df is (regular_data_df ) filtered to include only rows from a specific store
         """
-        store_df = store_data_df.groupby(date_col_str).sum().reset_index()[[date_col_str, sales_col_str]]
+        store_df = store_data_df.groupby(date_col_str).sum(numeric_only=True).reset_index()[[date_col_str, sales_col_str]]
         store_df = store_df.set_index(date_col_str)
 
         store_df = self.add_lags_and_rolling_averages_and_diffs_and_ewms(df=store_df[[sales_col_str]], base_column_name=store_col_str)
 
 
         store_df = store_df.drop(columns=[sales_col_str]).reset_index()
         store_df = store_df[store_df[date_col_str] == pd.to_datetime(predict_date)]
@@ -60,15 +60,15 @@
 
     def create_all_sku_lags(self, regular_data_df, predict_date):
         """
             This function assumes that regular_data_df is not filtered and accept include only rows from a specific sku
         """
         all_sku_lags = pd.DataFrame()
         for sku in regular_data_df[sku_col_str].unique():
-            sku_data = regular_data_df[regular_data_df[sku_col_str] == sku].groupby(date_col_str).sum().reset_index()[
+            sku_data = regular_data_df[regular_data_df[sku_col_str] == sku].groupby(date_col_str).sum(numeric_only=True).reset_index()[
                 [date_col_str, sales_col_str]]
             sku_data = sku_data.set_index(date_col_str)
 
             sku_data = self.add_lags_and_rolling_averages_and_diffs_and_ewms(sku_data[[sales_col_str]], sku_col_str)
 
             sku_data = sku_data.drop(columns=[sales_col_str]).reset_index()
             sku_data[sku_col_str] = np.int64(sku)
```

### Comparing `palmers_preprocess-0.0.6/src/palmers_preprocessing/features/weather_features.py` & `palmers_preprocess-0.0.7/src/palmers_preprocessing/features/weather_features.py`

 * *Files identical despite different names*

### Comparing `palmers_preprocess-0.0.6/src/palmers_preprocessing/tests/config_batch_dict.py` & `palmers_preprocess-0.0.7/src/palmers_preprocessing/tests/config_batch_dict.py`

 * *Files identical despite different names*

### Comparing `palmers_preprocess-0.0.6/src/palmers_preprocessing/tests/event_feature_test.py` & `palmers_preprocess-0.0.7/src/palmers_preprocessing/tests/event_feature_test.py`

 * *Files identical despite different names*

### Comparing `palmers_preprocess-0.0.6/src/palmers_preprocessing/tests/features_test.py` & `palmers_preprocess-0.0.7/src/palmers_preprocessing/tests/features_test.py`

 * *Files identical despite different names*

### Comparing `palmers_preprocess-0.0.6/src/palmers_preprocessing/tests/lags_features_test.py` & `palmers_preprocess-0.0.7/src/palmers_preprocessing/tests/lags_features_test.py`

 * *Files identical despite different names*

### Comparing `palmers_preprocess-0.0.6/src/palmers_preprocessing/tests/preprocessor_test.py` & `palmers_preprocess-0.0.7/src/palmers_preprocessing/tests/preprocessor_test.py`

 * *Files identical despite different names*

### Comparing `palmers_preprocess-0.0.6/src/palmers_preprocessing/tests/sanity_checks.py` & `palmers_preprocess-0.0.7/src/palmers_preprocessing/tests/sanity_checks.py`

 * *Files identical despite different names*

### Comparing `palmers_preprocess-0.0.6/src/palmers_preprocessing/tests/weather_test.py` & `palmers_preprocess-0.0.7/src/palmers_preprocessing/tests/weather_test.py`

 * *Files identical despite different names*

### Comparing `palmers_preprocess-0.0.6/LICENSE` & `palmers_preprocess-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `palmers_preprocess-0.0.6/pyproject.toml` & `palmers_preprocess-0.0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "palmers_preprocess"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Roy ", email="roy@sdatta.ai" },
   { name="Assaf", email="assafm@sdatta.ai" },
   { name="Guy", email="assafm@sdatta.ai" },
   { name="Oran", email="assafm@sdatta.ai" },
   { name="Yotam", email="assafm@sdatta.ai" },
 ]
```

### Comparing `palmers_preprocess-0.0.6/PKG-INFO` & `palmers_preprocess-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: palmers_preprocess
-Version: 0.0.6
+Version: 0.0.7
 Summary: A package to preprocess data for Palmer's project
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Author-email: Roy  <roy@sdatta.ai>, Assaf <assafm@sdatta.ai>, Guy <assafm@sdatta.ai>, Oran <assafm@sdatta.ai>, Yotam <assafm@sdatta.ai>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

