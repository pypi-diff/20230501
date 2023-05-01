# Comparing `tmp/lib310_lite-0.0.4.tar.gz` & `tmp/lib310_lite-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib310_lite-0.0.4.tar", max compression
+gzip compressed data, was "lib310_lite-0.0.5.tar", max compression
```

## Comparing `lib310_lite-0.0.4.tar` & `lib310_lite-0.0.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      249 2023-03-08 14:56:22.920616 lib310_lite-0.0.4/lib310_lite/__init__.py
--rw-r--r--   0        0        0      141 2023-03-07 16:27:34.184530 lib310_lite-0.0.4/lib310_lite/bigquery/_functions.py
--rw-r--r--   0        0        0     7467 2023-03-08 14:56:22.918017 lib310_lite-0.0.4/lib310_lite/bigquery/client.py
--rw-r--r--   0        0        0      872 2023-03-07 16:14:03.813101 lib310_lite-0.0.4/lib310_lite/bigquery/constants.py
--rw-r--r--   0        0        0       35 2023-03-07 10:52:53.179251 lib310_lite-0.0.4/lib310_lite/fucntion.py
--rw-r--r--   0        0        0     9324 2023-04-24 18:53:59.229007 lib310_lite-0.0.4/lib310_lite/mldl/mldl.py
--rw-r--r--   0        0        0      769 2023-04-24 19:01:38.262738 lib310_lite-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      877 1970-01-01 00:00:00.000000 lib310_lite-0.0.4/setup.py
--rw-r--r--   0        0        0      848 1970-01-01 00:00:00.000000 lib310_lite-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      249 2023-03-08 14:56:22.920616 lib310_lite-0.0.5/lib310_lite/__init__.py
+-rw-r--r--   0        0        0      141 2023-03-07 16:27:34.184530 lib310_lite-0.0.5/lib310_lite/bigquery/_functions.py
+-rw-r--r--   0        0        0     7467 2023-03-08 14:56:22.918017 lib310_lite-0.0.5/lib310_lite/bigquery/client.py
+-rw-r--r--   0        0        0      872 2023-03-07 16:14:03.813101 lib310_lite-0.0.5/lib310_lite/bigquery/constants.py
+-rw-r--r--   0        0        0       35 2023-03-07 10:52:53.179251 lib310_lite-0.0.5/lib310_lite/fucntion.py
+-rw-r--r--   0        0        0     9952 2023-05-01 20:32:25.307400 lib310_lite-0.0.5/lib310_lite/mldl/mldl.py
+-rw-r--r--   0        0        0      769 2023-05-01 20:14:07.640872 lib310_lite-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      877 1970-01-01 00:00:00.000000 lib310_lite-0.0.5/setup.py
+-rw-r--r--   0        0        0      848 1970-01-01 00:00:00.000000 lib310_lite-0.0.5/PKG-INFO
```

### Comparing `lib310_lite-0.0.4/lib310_lite/bigquery/client.py` & `lib310_lite-0.0.5/lib310_lite/bigquery/client.py`

 * *Files identical despite different names*

### Comparing `lib310_lite-0.0.4/lib310_lite/bigquery/constants.py` & `lib310_lite-0.0.5/lib310_lite/bigquery/constants.py`

 * *Files identical despite different names*

### Comparing `lib310_lite-0.0.4/lib310_lite/mldl/mldl.py` & `lib310_lite-0.0.5/lib310_lite/mldl/mldl.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,29 +16,32 @@
 
     __TRAIN = 'TRAIN'
     __TEST = 'TEST'
     __MAIN = 'MAIN'
     __INTERACTION = 'INTERACTION'
     __DB_NAME = 'A310'
     __TOKEN_NAMES = 'token_names'
-    __PARTS = {__INTERACTION: 1, __TOKEN_NAMES: 1}
+    __PROTEIN_NAMES = 'protein_names'
+    __TAXONOMIES = 'taxonomies'
+    __ORGANISMS = 'organisms'
+    __PARTS = {__INTERACTION: 1, __TOKEN_NAMES: 1, __PROTEIN_NAMES: 1, __TAXONOMIES: 1, __ORGANISMS: 0}
 
     def __init__(self, mongo_url: str, cache_size: int = 50, num_threads: int = 10, random_seed: int = time.time()):
         random.seed(random_seed)
         self.client = MongoClient(mongo_url)
         self.bq_client = BigQueryClient()
         self.db = self.client[MLDL.__DB_NAME]
 
         self.collections = {
             MLDL.__TRAIN: {
-                MLDL.__MAIN: self.db['seq_lang5'],
+                MLDL.__MAIN: self.db['seq_lang5_copy'],
                 MLDL.__INTERACTION: self.db['interactions_lang5_train'],
             },
             MLDL.__TEST: {
-                MLDL.__MAIN: self.db['seq_lang5'],
+                MLDL.__MAIN: self.db['seq_lang5_copy'],
                 MLDL.__INTERACTION: self.db['interactions_lang5_test'],
             }
         }
 
         # this is the pool of samples row_id
         self.sample_cache = []
         # this is the maximum number of requests we fetch sooner from the database
@@ -191,18 +194,27 @@
         :param stage: stage of the data
         :param parts: parts of the data
         :return: dataframe of main data
         """
         if parts is None:
             parts = MLDL.__PARTS
         token_names = 0
-        if parts[MLDL.__TOKEN_NAMES] and parts[MLDL.__TOKEN_NAMES] == 1:
+        if not parts[MLDL.__TOKEN_NAMES] or parts[MLDL.__TOKEN_NAMES] == 1:
             token_names = 1
+        protein_names = 0
+        if not parts[MLDL.__PROTEIN_NAMES] or parts[MLDL.__PROTEIN_NAMES] == 1:
+            protein_names = 1
+        taxonomies = 0
+        if not parts[MLDL.__TAXONOMIES] or parts[MLDL.__TAXONOMIES] == 1:
+            taxonomies = 1
+        organisms = 0
+        if not parts[MLDL.__ORGANISMS] or parts[MLDL.__ORGANISMS] == 1:
+            organisms = 1
         cursor = col.find({'row_id': {'$in': index_list}, 'stage': stage}, {'_id': 0, 'row_id': 1, 'sequence': 1,
-                                                                            'token_ids': 1, 'token_names': token_names})
+                                                                            'token_ids': 1, 'token_names': token_names, 'protein_names': protein_names, 'taxonomies': taxonomies, 'organisms': organisms})
         return pd.DataFrame(list(cursor))
 
     def fetch_sample_interaction(self, index_list: list, col):
         """
         This function is used to fetch the interaction data from the database
         :param index_list: list of row_ids
         :param col: interaction collection
```

### Comparing `lib310_lite-0.0.4/pyproject.toml` & `lib310_lite-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lib310_lite"
-version = "0.0.4"
+version = "0.0.5"
 description = "lib310 Lite Python Package"
 authors = ["310 <info@310.ai>"]
 maintainers = ["Saman Fekri <saman@310.ai>"]
 keywords = ["biology", "AI", "genomics", "bioinforma", "machine learning", "GAN"]
 packages = [
     { include = "lib310_lite" }
 ]
```

### Comparing `lib310_lite-0.0.4/setup.py` & `lib310_lite-0.0.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,15 +17,15 @@
  'google-cloud-bigquery>=3.2.0',
  'google-cloud>=0.34.0',
  'numpy<1.23.0',
  'pymongo>=4.0.0']
 
 setup_kwargs = {
     'name': 'lib310-lite',
-    'version': '0.0.4',
+    'version': '0.0.5',
     'description': 'lib310 Lite Python Package',
     'long_description': 'None',
     'author': '310',
     'author_email': 'info@310.ai',
     'maintainer': 'Saman Fekri',
     'maintainer_email': 'saman@310.ai',
     'url': 'None',
```

### Comparing `lib310_lite-0.0.4/PKG-INFO` & `lib310_lite-0.0.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib310-lite
-Version: 0.0.4
+Version: 0.0.5
 Summary: lib310 Lite Python Package
 Keywords: biology,AI,genomics,bioinforma,machine learning,GAN
 Author: 310
 Author-email: info@310.ai
 Maintainer: Saman Fekri
 Maintainer-email: saman@310.ai
 Requires-Python: >=3.8
```

