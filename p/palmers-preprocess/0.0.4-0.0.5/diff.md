# Comparing `tmp/palmers_preprocess-0.0.4.tar.gz` & `tmp/palmers_preprocess-0.0.5.tar.gz`

## Comparing `palmers_preprocess-0.0.4.tar` & `palmers_preprocess-0.0.5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.4/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.4/src/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.4/src/palmers_preprocessing/__init__.py
--rw-r--r--   0        0        0     5181 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.4/src/palmers_preprocessing/clearml_data_handler.py
--rw-r--r--   0        0        0     6784 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.4/src/palmers_preprocessing/config.py
--rw-r--r--   0        0        0    43603 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.4/src/palmers_preprocessing/events_handler.py
--rw-r--r--   0        0        0     5165 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.4/src/palmers_preprocessing/lags_feature_handler.py
--rw-r--r--   0        0        0     7599 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.4/src/palmers_preprocessing/preprocessor.py
--rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.4/src/palmers_preprocessing/regular_data_handler.py
--rw-r--r--   0        0        0     7669 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.4/src/palmers_preprocessing/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.4/src/palmers_preprocessing/features/__init__.py
--rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.4/src/palmers_preprocessing/features/config.py
--rw-r--r--   0        0        0     8887 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.4/src/palmers_preprocessing/features/cumulative_features.py
--rw-r--r--   0        0        0     9093 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.4/src/palmers_preprocessing/features/event_features.py
--rw-r--r--   0        0        0     8418 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.4/src/palmers_preprocessing/features/future_features.py
--rw-r--r--   0        0        0     4108 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.4/src/palmers_preprocessing/features/lags_features.py
--rw-r--r--   0        0        0     5404 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.4/src/palmers_preprocessing/features/weather_features.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.4/tests/__init__.py
--rw-r--r--   0        0        0   719548 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.4/tests/config_batch_dict.py
--rw-r--r--   0        0        0     1987 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.4/tests/event_feature_test.py
--rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.4/tests/features_test.py
--rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.4/tests/lags_features_test.py
--rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.4/tests/preprocessor_test.py
--rw-r--r--   0        0        0    50890 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.4/tests/sanity_checks.py
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.4/tests/test_todelete.py
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.4/tests/weather_test.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.4/.gitignore
--rw-r--r--   0        0        0    11558 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.4/LICENSE
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.4/README.md
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.5/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.5/src/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.5/src/palmers_preprocessing/__init__.py
+-rw-r--r--   0        0        0     5181 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.5/src/palmers_preprocessing/clearml_data_handler.py
+-rw-r--r--   0        0        0     6784 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.5/src/palmers_preprocessing/config.py
+-rw-r--r--   0        0        0    43620 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.5/src/palmers_preprocessing/events_handler.py
+-rw-r--r--   0        0        0     5216 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.5/src/palmers_preprocessing/lags_feature_handler.py
+-rw-r--r--   0        0        0     7599 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.5/src/palmers_preprocessing/preprocessor.py
+-rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.5/src/palmers_preprocessing/regular_data_handler.py
+-rw-r--r--   0        0        0     7669 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.5/src/palmers_preprocessing/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.5/src/palmers_preprocessing/features/__init__.py
+-rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.5/src/palmers_preprocessing/features/config.py
+-rw-r--r--   0        0        0     8887 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.5/src/palmers_preprocessing/features/cumulative_features.py
+-rw-r--r--   0        0        0     9093 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.5/src/palmers_preprocessing/features/event_features.py
+-rw-r--r--   0        0        0     8418 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.5/src/palmers_preprocessing/features/future_features.py
+-rw-r--r--   0        0        0     4108 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.5/src/palmers_preprocessing/features/lags_features.py
+-rw-r--r--   0        0        0     5404 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.5/src/palmers_preprocessing/features/weather_features.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.5/tests/__init__.py
+-rw-r--r--   0        0        0   719548 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.5/tests/config_batch_dict.py
+-rw-r--r--   0        0        0     1987 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.5/tests/event_feature_test.py
+-rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.5/tests/features_test.py
+-rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.5/tests/lags_features_test.py
+-rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.5/tests/preprocessor_test.py
+-rw-r--r--   0        0        0    50890 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.5/tests/sanity_checks.py
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.5/tests/test_todelete.py
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.5/tests/weather_test.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.5/.gitignore
+-rw-r--r--   0        0        0    11558 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.5/LICENSE
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.5/README.md
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.5/PKG-INFO
```

### Comparing `palmers_preprocess-0.0.4/requirements.txt` & `palmers_preprocess-0.0.5/requirements.txt`

 * *Files identical despite different names*

### Comparing `palmers_preprocess-0.0.4/src/palmers_preprocessing/clearml_data_handler.py` & `palmers_preprocess-0.0.5/src/palmers_preprocessing/clearml_data_handler.py`

 * *Files identical despite different names*

### Comparing `palmers_preprocess-0.0.4/src/palmers_preprocessing/config.py` & `palmers_preprocess-0.0.5/src/palmers_preprocessing/config.py`

 * *Files identical despite different names*

### Comparing `palmers_preprocess-0.0.4/src/palmers_preprocessing/events_handler.py` & `palmers_preprocess-0.0.5/src/palmers_preprocessing/events_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,15 +85,15 @@
             target_col:     name of target column
             df_sales:      pandas DataFrame
 
         Returns:   aggregate by target_col pandas DataFrame
 
         """
         df_sales[target_col] = df_sales[target_col].astype(np.float64)
-        return df_sales.groupby(['date'])[target_col].sum().reset_index()
+        return df_sales.groupby(['date'])[target_col].sum(numeric_only=True).reset_index()
 
     @classmethod
     def filter_data_by_date(cls, df_sales: pd.DataFrame, date_col: str, start_date: str) -> pd.DataFrame:
         """
         Filter data by date
         Args:
             df_sales:      pandas DataFrame
```

### Comparing `palmers_preprocess-0.0.4/src/palmers_preprocessing/lags_feature_handler.py` & `palmers_preprocess-0.0.5/src/palmers_preprocessing/lags_feature_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         self.lags_back = lags_back
         self.windows = windows
         self.diff_lags = diff_lags
         self.ewms = ewms
 
 
     def sum_agg_per_sku_date_store(self, data):
-        data = data.groupby([self.date_name, self.store_name, self.sku_name]).sum()[self.sales_name].reset_index()
+        data = data.groupby([self.date_name, self.store_name, self.sku_name]).sum(numeric_only=True)[self.sales_name].reset_index()
         data[self.sku_name] = data[self.sku_name].astype('category')
         data[self.store_name] = data[self.store_name].astype('category')
         return data
 
     def add_sku_store_id_col(self, df):
         ''' Add a column with the sku and store id.
 
@@ -86,26 +86,26 @@
 
 
     def return_df_of_store_sales_with_lags_rolling_diff_ewm(self, data):
         df_of_store_sales = pd.DataFrame()
         i = 0
         for store in data["store"].unique():
             i += 1
-            store_data = data[data["store"] == store].groupby("date").sum()
+            store_data = data[data["store"] == store].groupby("date").sum(numeric_only=True)
             store_data['store'] = store
             store_data = LagsRollingAverageDiffsEWMsFeaturesGenerator.add_lags_and_rolling_averages_and_diffs_and_ewms(self, store_data[['sales']], self.store_name)
             store_data['store'] = store
             df_of_store_sales = pd.concat([store_data.reset_index().rename(columns={"index": "date"})])
         return df_of_store_sales
 
     def return_df_of_sku_sales_with_lags_rolling_diff_ewm(self, data):
         df_of_sku_sales = pd.DataFrame()
         i = 0
         for sku in data["sku"].unique():
             i += 1
-            sku_data = data[data["sku"] == sku].groupby("date").sum()
+            sku_data = data[data["sku"] == sku].groupby("date").sum(numeric_only=True)
             sku_data['sku'] = sku
             sku_data = LagsRollingAverageDiffsEWMsFeaturesGenerator.add_lags_and_rolling_averages_and_diffs_and_ewms(self, sku_data[['sales']], self.sku_name)
             sku_data['sku'] = sku
             df_of_sku_sales = pd.concat([sku_data.reset_index().rename(columns={"index": "date"})])
 
         return df_of_sku_sales
```

### Comparing `palmers_preprocess-0.0.4/src/palmers_preprocessing/preprocessor.py` & `palmers_preprocess-0.0.5/src/palmers_preprocessing/preprocessor.py`

 * *Files identical despite different names*

### Comparing `palmers_preprocess-0.0.4/src/palmers_preprocessing/regular_data_handler.py` & `palmers_preprocess-0.0.5/src/palmers_preprocessing/regular_data_handler.py`

 * *Files identical despite different names*

### Comparing `palmers_preprocess-0.0.4/src/palmers_preprocessing/utils.py` & `palmers_preprocess-0.0.5/src/palmers_preprocessing/utils.py`

 * *Files identical despite different names*

### Comparing `palmers_preprocess-0.0.4/src/palmers_preprocessing/features/config.py` & `palmers_preprocess-0.0.5/src/palmers_preprocessing/features/config.py`

 * *Files identical despite different names*

### Comparing `palmers_preprocess-0.0.4/src/palmers_preprocessing/features/cumulative_features.py` & `palmers_preprocess-0.0.5/src/palmers_preprocessing/features/cumulative_features.py`

 * *Files identical despite different names*

### Comparing `palmers_preprocess-0.0.4/src/palmers_preprocessing/features/event_features.py` & `palmers_preprocess-0.0.5/src/palmers_preprocessing/features/event_features.py`

 * *Files identical despite different names*

### Comparing `palmers_preprocess-0.0.4/src/palmers_preprocessing/features/future_features.py` & `palmers_preprocess-0.0.5/src/palmers_preprocessing/features/future_features.py`

 * *Files identical despite different names*

### Comparing `palmers_preprocess-0.0.4/src/palmers_preprocessing/features/lags_features.py` & `palmers_preprocess-0.0.5/src/palmers_preprocessing/features/lags_features.py`

 * *Files identical despite different names*

### Comparing `palmers_preprocess-0.0.4/src/palmers_preprocessing/features/weather_features.py` & `palmers_preprocess-0.0.5/src/palmers_preprocessing/features/weather_features.py`

 * *Files identical despite different names*

### Comparing `palmers_preprocess-0.0.4/tests/config_batch_dict.py` & `palmers_preprocess-0.0.5/tests/config_batch_dict.py`

 * *Files identical despite different names*

### Comparing `palmers_preprocess-0.0.4/tests/event_feature_test.py` & `palmers_preprocess-0.0.5/tests/event_feature_test.py`

 * *Files identical despite different names*

### Comparing `palmers_preprocess-0.0.4/tests/features_test.py` & `palmers_preprocess-0.0.5/tests/features_test.py`

 * *Files identical despite different names*

### Comparing `palmers_preprocess-0.0.4/tests/lags_features_test.py` & `palmers_preprocess-0.0.5/tests/lags_features_test.py`

 * *Files identical despite different names*

### Comparing `palmers_preprocess-0.0.4/tests/preprocessor_test.py` & `palmers_preprocess-0.0.5/tests/preprocessor_test.py`

 * *Files identical despite different names*

### Comparing `palmers_preprocess-0.0.4/tests/sanity_checks.py` & `palmers_preprocess-0.0.5/tests/sanity_checks.py`

 * *Files identical despite different names*

### Comparing `palmers_preprocess-0.0.4/tests/weather_test.py` & `palmers_preprocess-0.0.5/tests/weather_test.py`

 * *Files identical despite different names*

### Comparing `palmers_preprocess-0.0.4/LICENSE` & `palmers_preprocess-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `palmers_preprocess-0.0.4/pyproject.toml` & `palmers_preprocess-0.0.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "palmers_preprocess"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Roy ", email="roy@sdatta.ai" },
   { name="Assaf", email="assafm@sdatta.ai" },
   { name="Guy", email="assafm@sdatta.ai" },
   { name="Oran", email="assafm@sdatta.ai" },
   { name="Yotam", email="assafm@sdatta.ai" },
 ]
```

### Comparing `palmers_preprocess-0.0.4/PKG-INFO` & `palmers_preprocess-0.0.5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: palmers_preprocess
-Version: 0.0.4
+Version: 0.0.5
 Summary: A package to preprocess data for Palmer's project
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Author-email: Roy  <roy@sdatta.ai>, Assaf <assafm@sdatta.ai>, Guy <assafm@sdatta.ai>, Oran <assafm@sdatta.ai>, Yotam <assafm@sdatta.ai>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

