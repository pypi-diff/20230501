# Comparing `tmp/pheno-utils-0.1.9.tar.gz` & `tmp/pheno-utils-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pheno-utils-0.1.9.tar", last modified: Wed Apr 26 20:36:55 2023, max compression
+gzip compressed data, was "pheno-utils-0.2.0.tar", last modified: Mon May  1 18:49:32 2023, max compression
```

## Comparing `pheno-utils-0.1.9.tar` & `pheno-utils-0.2.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 alondmnt   (501) staff       (20)        0 2023-04-26 20:36:55.770380 pheno-utils-0.1.9/
--rw-r--r--   0 alondmnt   (501) staff       (20)    11357 2023-04-06 20:07:34.000000 pheno-utils-0.1.9/LICENSE
--rw-r--r--   0 alondmnt   (501) staff       (20)      111 2023-04-06 20:07:42.000000 pheno-utils-0.1.9/MANIFEST.in
--rw-r--r--   0 alondmnt   (501) staff       (20)     1479 2023-04-26 20:36:55.769989 pheno-utils-0.1.9/PKG-INFO
--rw-r--r--   0 alondmnt   (501) staff       (20)      446 2023-04-06 20:07:47.000000 pheno-utils-0.1.9/README.md
-drwxr-xr-x   0 alondmnt   (501) staff       (20)        0 2023-04-26 20:36:55.765544 pheno-utils-0.1.9/pheno_utils/
--rw-r--r--   0 alondmnt   (501) staff       (20)      355 2023-04-26 20:32:17.000000 pheno-utils-0.1.9/pheno_utils/__init__.py
--rw-r--r--   0 alondmnt   (501) staff       (20)    16451 2023-04-26 20:32:17.000000 pheno-utils-0.1.9/pheno_utils/_modidx.py
--rw-r--r--   0 alondmnt   (501) staff       (20)    16963 2023-04-26 20:32:17.000000 pheno-utils-0.1.9/pheno_utils/age_reference_plots.py
--rw-r--r--   0 alondmnt   (501) staff       (20)     5300 2023-04-26 20:32:17.000000 pheno-utils-0.1.9/pheno_utils/basic_analysis.py
--rw-r--r--   0 alondmnt   (501) staff       (20)     2789 2023-04-26 20:32:17.000000 pheno-utils-0.1.9/pheno_utils/basic_plots.py
--rw-r--r--   0 alondmnt   (501) staff       (20)     2517 2023-04-26 20:32:17.000000 pheno-utils-0.1.9/pheno_utils/blandaltman_plots.py
--rw-r--r--   0 alondmnt   (501) staff       (20)     7865 2023-04-26 20:32:17.000000 pheno-utils-0.1.9/pheno_utils/cgm_plots.py
--rw-r--r--   0 alondmnt   (501) staff       (20)     3599 2023-04-26 20:32:17.000000 pheno-utils-0.1.9/pheno_utils/config.py
--rw-r--r--   0 alondmnt   (501) staff       (20)    17193 2023-04-26 20:32:17.000000 pheno-utils-0.1.9/pheno_utils/data_loader.py
--rw-r--r--   0 alondmnt   (501) staff       (20)     2825 2023-04-26 20:32:17.000000 pheno-utils-0.1.9/pheno_utils/dates_plots.py
--rw-r--r--   0 alondmnt   (501) staff       (20)     2113 2023-04-26 20:32:17.000000 pheno-utils-0.1.9/pheno_utils/ecg_analysis.py
--rw-r--r--   0 alondmnt   (501) staff       (20)     7306 2023-04-26 20:32:17.000000 pheno-utils-0.1.9/pheno_utils/meta_loader.py
--rw-r--r--   0 alondmnt   (501) staff       (20)    13210 2023-04-26 20:32:17.000000 pheno-utils-0.1.9/pheno_utils/sleep_plots.py
--rw-r--r--   0 alondmnt   (501) staff       (20)     1225 2023-04-26 20:32:17.000000 pheno-utils-0.1.9/pheno_utils/subset_loader.py
-drwxr-xr-x   0 alondmnt   (501) staff       (20)        0 2023-04-26 20:36:55.769322 pheno-utils-0.1.9/pheno_utils.egg-info/
--rw-r--r--   0 alondmnt   (501) staff       (20)     1479 2023-04-26 20:36:55.000000 pheno-utils-0.1.9/pheno_utils.egg-info/PKG-INFO
--rw-r--r--   0 alondmnt   (501) staff       (20)      681 2023-04-26 20:36:55.000000 pheno-utils-0.1.9/pheno_utils.egg-info/SOURCES.txt
--rw-r--r--   0 alondmnt   (501) staff       (20)        1 2023-04-26 20:36:55.000000 pheno-utils-0.1.9/pheno_utils.egg-info/dependency_links.txt
--rw-r--r--   0 alondmnt   (501) staff       (20)       65 2023-04-26 20:36:55.000000 pheno-utils-0.1.9/pheno_utils.egg-info/entry_points.txt
--rw-r--r--   0 alondmnt   (501) staff       (20)        1 2023-04-06 08:56:36.000000 pheno-utils-0.1.9/pheno_utils.egg-info/not-zip-safe
--rw-r--r--   0 alondmnt   (501) staff       (20)      143 2023-04-26 20:36:55.000000 pheno-utils-0.1.9/pheno_utils.egg-info/requires.txt
--rw-r--r--   0 alondmnt   (501) staff       (20)       12 2023-04-26 20:36:55.000000 pheno-utils-0.1.9/pheno_utils.egg-info/top_level.txt
--rw-r--r--   0 alondmnt   (501) staff       (20)     1086 2023-04-26 20:20:39.000000 pheno-utils-0.1.9/settings.ini
--rw-r--r--   0 alondmnt   (501) staff       (20)       38 2023-04-26 20:36:55.770561 pheno-utils-0.1.9/setup.cfg
--rw-r--r--   0 alondmnt   (501) staff       (20)     2560 2023-04-06 20:07:57.000000 pheno-utils-0.1.9/setup.py
+drwxr-xr-x   0 alondmnt   (501) staff       (20)        0 2023-05-01 18:49:32.461170 pheno-utils-0.2.0/
+-rw-r--r--   0 alondmnt   (501) staff       (20)    11357 2023-04-06 20:07:34.000000 pheno-utils-0.2.0/LICENSE
+-rw-r--r--   0 alondmnt   (501) staff       (20)      111 2023-04-06 20:07:42.000000 pheno-utils-0.2.0/MANIFEST.in
+-rw-r--r--   0 alondmnt   (501) staff       (20)     1553 2023-05-01 18:49:32.458503 pheno-utils-0.2.0/PKG-INFO
+-rw-r--r--   0 alondmnt   (501) staff       (20)      504 2023-05-01 07:16:03.000000 pheno-utils-0.2.0/README.md
+drwxr-xr-x   0 alondmnt   (501) staff       (20)        0 2023-05-01 18:49:32.449280 pheno-utils-0.2.0/pheno_utils/
+-rw-r--r--   0 alondmnt   (501) staff       (20)      355 2023-05-01 18:46:41.000000 pheno-utils-0.2.0/pheno_utils/__init__.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)    16451 2023-05-01 18:46:41.000000 pheno-utils-0.2.0/pheno_utils/_modidx.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)    16963 2023-05-01 18:46:41.000000 pheno-utils-0.2.0/pheno_utils/age_reference_plots.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)     5300 2023-05-01 18:46:41.000000 pheno-utils-0.2.0/pheno_utils/basic_analysis.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)     2789 2023-05-01 18:46:41.000000 pheno-utils-0.2.0/pheno_utils/basic_plots.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)     2517 2023-05-01 18:46:41.000000 pheno-utils-0.2.0/pheno_utils/blandaltman_plots.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)     7865 2023-05-01 18:46:41.000000 pheno-utils-0.2.0/pheno_utils/cgm_plots.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)     3599 2023-05-01 18:46:41.000000 pheno-utils-0.2.0/pheno_utils/config.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)    17656 2023-05-01 18:46:41.000000 pheno-utils-0.2.0/pheno_utils/data_loader.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)     2825 2023-05-01 18:46:41.000000 pheno-utils-0.2.0/pheno_utils/dates_plots.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)     2113 2023-05-01 18:46:41.000000 pheno-utils-0.2.0/pheno_utils/ecg_analysis.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)     7691 2023-05-01 18:46:41.000000 pheno-utils-0.2.0/pheno_utils/meta_loader.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)    13210 2023-05-01 18:46:41.000000 pheno-utils-0.2.0/pheno_utils/sleep_plots.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)     1586 2023-05-01 18:46:41.000000 pheno-utils-0.2.0/pheno_utils/subset_loader.py
+drwxr-xr-x   0 alondmnt   (501) staff       (20)        0 2023-05-01 18:49:32.456084 pheno-utils-0.2.0/pheno_utils.egg-info/
+-rw-r--r--   0 alondmnt   (501) staff       (20)     1553 2023-05-01 18:49:32.000000 pheno-utils-0.2.0/pheno_utils.egg-info/PKG-INFO
+-rw-r--r--   0 alondmnt   (501) staff       (20)      681 2023-05-01 18:49:32.000000 pheno-utils-0.2.0/pheno_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 alondmnt   (501) staff       (20)        1 2023-05-01 18:49:32.000000 pheno-utils-0.2.0/pheno_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 alondmnt   (501) staff       (20)       65 2023-05-01 18:49:32.000000 pheno-utils-0.2.0/pheno_utils.egg-info/entry_points.txt
+-rw-r--r--   0 alondmnt   (501) staff       (20)        1 2023-04-06 08:56:36.000000 pheno-utils-0.2.0/pheno_utils.egg-info/not-zip-safe
+-rw-r--r--   0 alondmnt   (501) staff       (20)      143 2023-05-01 18:49:32.000000 pheno-utils-0.2.0/pheno_utils.egg-info/requires.txt
+-rw-r--r--   0 alondmnt   (501) staff       (20)       12 2023-05-01 18:49:32.000000 pheno-utils-0.2.0/pheno_utils.egg-info/top_level.txt
+-rw-r--r--   0 alondmnt   (501) staff       (20)     1085 2023-05-01 18:46:30.000000 pheno-utils-0.2.0/settings.ini
+-rw-r--r--   0 alondmnt   (501) staff       (20)       38 2023-05-01 18:49:32.461742 pheno-utils-0.2.0/setup.cfg
+-rw-r--r--   0 alondmnt   (501) staff       (20)     2560 2023-04-06 20:07:57.000000 pheno-utils-0.2.0/setup.py
```

### Comparing `pheno-utils-0.1.9/LICENSE` & `pheno-utils-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.1.9/PKG-INFO` & `pheno-utils-0.2.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pheno-utils
-Version: 0.1.9
+Version: 0.2.0
 Summary: Pheno data utils - viz, loaders, mergers
 Home-page: https://github.com/hrossman/pheno-utils
 Author: hrossman
 Author-email: hagairossman@gmail.com
 License: Apache Software License 2.0
 Description: pheno-utils
         ================
@@ -26,21 +26,23 @@
         Examples:
         
         ``` python
         data = generate_synthetic_data(n=1000)
         hist_ecdf_plots(data=data, col="val1")
         ```
         
-            NameError: name 'hist_ecdf_plots' is not defined
+        ![](index_files/figure-commonmark/cell-2-output-1.png)
         
         ``` python
         age_refplots = GenderAgeRefPlot(data, "val1")
         age_refplots.plot()
         ```
         
+        ![](index_files/figure-commonmark/cell-3-output-1.png)
+        
 Keywords: nbdev jupyter notebook python
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `pheno-utils-0.1.9/pheno_utils/_modidx.py` & `pheno-utils-0.2.0/pheno_utils/_modidx.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.1.9/pheno_utils/age_reference_plots.py` & `pheno-utils-0.2.0/pheno_utils/age_reference_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.1.9/pheno_utils/basic_analysis.py` & `pheno-utils-0.2.0/pheno_utils/basic_analysis.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.1.9/pheno_utils/basic_plots.py` & `pheno-utils-0.2.0/pheno_utils/basic_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.1.9/pheno_utils/blandaltman_plots.py` & `pheno-utils-0.2.0/pheno_utils/blandaltman_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.1.9/pheno_utils/cgm_plots.py` & `pheno-utils-0.2.0/pheno_utils/cgm_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.1.9/pheno_utils/config.py` & `pheno-utils-0.2.0/pheno_utils/config.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.1.9/pheno_utils/data_loader.py` & `pheno-utils-0.2.0/pheno_utils/data_loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -273,18 +273,32 @@
 
         self.fields += ['age', 'sex']
         ind = self.dfs['age_sex'].isnull().any(axis=1)
         if not ind.any():  # no missing values
             return
 
         # fill in missing values by computing age from birth date
-        date_cols = np.array(['collection_date', 'collection_timestamp', 'sequencing_date'])
-        date = date_cols[np.isin(date_cols, align_df.columns)][0]  # prefer first match
+        try:
+            date_cols = np.array(['collection_date', 'collection_timestamp', 'sequencing_date'])
+            date = date_cols[np.isin(date_cols, align_df.columns)][0]  # prefer first match
+        except Exception as e:
+            if self.errors == 'raise':
+                raise(e)
+            elif self.errors == 'warn':
+                warnings.warn(f'No date field found')
+            return
 
-        ind &= align_df[date].notnull()
+        try:
+            ind &= align_df[date].notnull()
+        except Exception as e:
+            if self.errors == 'raise':
+                raise(e)
+            if self.errors == 'warn':
+                warnings.warn(f'Error checking date field: {e}')
+            return
         if not ind.any():
             return
 
         age_df = pd.read_parquet(age_path.replace('events', 'population'))
 
         # trying a workaround for a pandas deprecation warning
         age_sex = self.dfs['age_sex']
```

### Comparing `pheno-utils-0.1.9/pheno_utils/dates_plots.py` & `pheno-utils-0.2.0/pheno_utils/dates_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.1.9/pheno_utils/ecg_analysis.py` & `pheno-utils-0.2.0/pheno_utils/ecg_analysis.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.1.9/pheno_utils/meta_loader.py` & `pheno-utils-0.2.0/pheno_utils/meta_loader.py`

 * *Files 5% similar despite different names*

```diff
@@ -67,22 +67,32 @@
             fields (Union[str,List[str]]): Fields to return
             flexible (bool, optional): Whether to use fuzzy matching to find fields. Defaults to None, which uses the DataLoader's flexible_field_search attribute.
             prop (str, optional): The property to use for searching. Defaults to 'tabular_field_name'.
 
         Returns:
             pd.DataFrame: Dataframe containing the fields from the respective datasets.
         """
+        found_fields = self.get(fields, flexible, prop)
+        found_fields.columns = found_fields.columns.str.split('/').str[1]
+        dup_fields = found_fields.columns.value_counts()\
+            .to_frame('count').query('count > 1').index
+
         loaded_fields = []
-        for ds, f in self.get(fields, flexible, prop).T.groupby('dataset'):
-            df = PhenoLoader(ds, base_path=self.base_path, cohort=self.cohort, **self.kwargs)\
-                [f.index.str.replace(f'{ds}/', '').tolist()]
-            if len(loaded_fields):
-                loaded_fields = loaded_fields.join(df, how='outer')
-            else:
+        for ds, f in found_fields.T.groupby('dataset'):
+            df = PhenoLoader(ds, base_path=self.base_path, cohort=self.cohort,
+                             age_sex_dataset=None, **self.kwargs)\
+                [f.index.tolist()]
+            # rename duplicate fields
+            df = df.rename(columns=pd.Series(dup_fields + f'_{ds}', index=dup_fields))
+
+            if not len(loaded_fields):
                 loaded_fields = df
+                continue
+
+            loaded_fields = loaded_fields.join(df, how='outer')
 
         return loaded_fields
 
     def get(self, fields: Union[str,List[str]], flexible: bool=None, prop='tabular_field_name') -> pd.DataFrame:
         """
         Return metadata for the specified fields from all tables.
 
@@ -132,16 +142,16 @@
         """
         Return string representation of object
 
         Returns:
             str: String representation of object
         """
         ds_list = str(list(self.dicts.keys())).replace(',', '\n')
-        return f'MetaLoader for: {self.dataset_path}' +\
-            f'with \n{len(self.fields)} fields\n{len(self.dicts)} datasets:\n{ds_list}'
+        return f'MetaLoader for: {self.dataset_path}\n' + \
+            f'with {len(self.fields)} fields\n{len(self.dicts)} datasets:\n{ds_list}'
 
     def __getitem__(self, fields: Union[str,List[str]]):
         """
         Return data for the specified fields from all tables
 
         Args:
             fields (Union[str, List[str]]): Fields to return
```

### Comparing `pheno-utils-0.1.9/pheno_utils/sleep_plots.py` & `pheno-utils-0.2.0/pheno_utils/sleep_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.1.9/pheno_utils.egg-info/PKG-INFO` & `pheno-utils-0.2.0/pheno_utils.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pheno-utils
-Version: 0.1.9
+Version: 0.2.0
 Summary: Pheno data utils - viz, loaders, mergers
 Home-page: https://github.com/hrossman/pheno-utils
 Author: hrossman
 Author-email: hagairossman@gmail.com
 License: Apache Software License 2.0
 Description: pheno-utils
         ================
@@ -26,21 +26,23 @@
         Examples:
         
         ``` python
         data = generate_synthetic_data(n=1000)
         hist_ecdf_plots(data=data, col="val1")
         ```
         
-            NameError: name 'hist_ecdf_plots' is not defined
+        ![](index_files/figure-commonmark/cell-2-output-1.png)
         
         ``` python
         age_refplots = GenderAgeRefPlot(data, "val1")
         age_refplots.plot()
         ```
         
+        ![](index_files/figure-commonmark/cell-3-output-1.png)
+        
 Keywords: nbdev jupyter notebook python
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `pheno-utils-0.1.9/pheno_utils.egg-info/SOURCES.txt` & `pheno-utils-0.2.0/pheno_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.1.9/setup.py` & `pheno-utils-0.2.0/setup.py`

 * *Files identical despite different names*

