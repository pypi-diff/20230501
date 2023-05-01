# Comparing `tmp/dbt_lineage_viewer-0.7.tar.gz` & `tmp/dbt_lineage_viewer-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt_lineage_viewer-0.7.tar", last modified: Mon May  1 18:29:32 2023, max compression
+gzip compressed data, was "dbt_lineage_viewer-0.8.tar", last modified: Mon May  1 19:37:09 2023, max compression
```

## Comparing `dbt_lineage_viewer-0.7.tar` & `dbt_lineage_viewer-0.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 yang      (1000) yang      (1000)        0 2023-05-01 18:29:32.438627 dbt_lineage_viewer-0.7/
--rw-r--r--   0 yang      (1000) yang      (1000)     1453 2023-05-01 18:29:32.438627 dbt_lineage_viewer-0.7/PKG-INFO
--rw-r--r--   0 yang      (1000) yang      (1000)     1211 2023-05-01 08:59:16.000000 dbt_lineage_viewer-0.7/README.md
-drwxr-xr-x   0 yang      (1000) yang      (1000)        0 2023-05-01 18:29:32.438627 dbt_lineage_viewer-0.7/dbt_lineage_viewer/
--rw-r--r--   0 yang      (1000) yang      (1000)       23 2023-05-01 09:25:49.000000 dbt_lineage_viewer-0.7/dbt_lineage_viewer/__init__.py
--rw-r--r--   0 yang      (1000) yang      (1000)     2903 2023-05-01 18:29:11.000000 dbt_lineage_viewer-0.7/dbt_lineage_viewer/main.py
--rw-r--r--   0 yang      (1000) yang      (1000)     1452 2023-05-01 09:24:52.000000 dbt_lineage_viewer-0.7/dbt_lineage_viewer/mermaid.py
--rw-r--r--   0 yang      (1000) yang      (1000)     3650 2023-05-01 18:26:05.000000 dbt_lineage_viewer-0.7/dbt_lineage_viewer/model.py
--rw-r--r--   0 yang      (1000) yang      (1000)      237 2023-05-01 16:49:00.000000 dbt_lineage_viewer-0.7/dbt_lineage_viewer/utils.py
-drwxr-xr-x   0 yang      (1000) yang      (1000)        0 2023-05-01 18:29:32.438627 dbt_lineage_viewer-0.7/dbt_lineage_viewer.egg-info/
--rw-r--r--   0 yang      (1000) yang      (1000)     1453 2023-05-01 18:29:32.000000 dbt_lineage_viewer-0.7/dbt_lineage_viewer.egg-info/PKG-INFO
--rw-r--r--   0 yang      (1000) yang      (1000)      416 2023-05-01 18:29:32.000000 dbt_lineage_viewer-0.7/dbt_lineage_viewer.egg-info/SOURCES.txt
--rw-r--r--   0 yang      (1000) yang      (1000)        1 2023-05-01 18:29:32.000000 dbt_lineage_viewer-0.7/dbt_lineage_viewer.egg-info/dependency_links.txt
--rw-r--r--   0 yang      (1000) yang      (1000)       63 2023-05-01 18:29:32.000000 dbt_lineage_viewer-0.7/dbt_lineage_viewer.egg-info/entry_points.txt
--rw-r--r--   0 yang      (1000) yang      (1000)        6 2023-05-01 18:29:32.000000 dbt_lineage_viewer-0.7/dbt_lineage_viewer.egg-info/requires.txt
--rw-r--r--   0 yang      (1000) yang      (1000)       19 2023-05-01 18:29:32.000000 dbt_lineage_viewer-0.7/dbt_lineage_viewer.egg-info/top_level.txt
--rw-r--r--   0 yang      (1000) yang      (1000)       38 2023-05-01 18:29:32.438627 dbt_lineage_viewer-0.7/setup.cfg
--rw-r--r--   0 yang      (1000) yang      (1000)      675 2023-05-01 18:29:21.000000 dbt_lineage_viewer-0.7/setup.py
+drwxr-xr-x   0 yang      (1000) yang      (1000)        0 2023-05-01 19:37:09.749722 dbt_lineage_viewer-0.8/
+-rw-r--r--   0 yang      (1000) yang      (1000)     1453 2023-05-01 19:37:09.749722 dbt_lineage_viewer-0.8/PKG-INFO
+-rw-r--r--   0 yang      (1000) yang      (1000)     1211 2023-05-01 08:59:16.000000 dbt_lineage_viewer-0.8/README.md
+drwxr-xr-x   0 yang      (1000) yang      (1000)        0 2023-05-01 19:37:09.749722 dbt_lineage_viewer-0.8/dbt_lineage_viewer/
+-rw-r--r--   0 yang      (1000) yang      (1000)       23 2023-05-01 09:25:49.000000 dbt_lineage_viewer-0.8/dbt_lineage_viewer/__init__.py
+-rw-r--r--   0 yang      (1000) yang      (1000)     2903 2023-05-01 18:29:11.000000 dbt_lineage_viewer-0.8/dbt_lineage_viewer/main.py
+-rw-r--r--   0 yang      (1000) yang      (1000)     1452 2023-05-01 09:24:52.000000 dbt_lineage_viewer-0.8/dbt_lineage_viewer/mermaid.py
+-rw-r--r--   0 yang      (1000) yang      (1000)     3630 2023-05-01 19:35:46.000000 dbt_lineage_viewer-0.8/dbt_lineage_viewer/model.py
+-rw-r--r--   0 yang      (1000) yang      (1000)      237 2023-05-01 16:49:00.000000 dbt_lineage_viewer-0.8/dbt_lineage_viewer/utils.py
+drwxr-xr-x   0 yang      (1000) yang      (1000)        0 2023-05-01 19:37:09.749722 dbt_lineage_viewer-0.8/dbt_lineage_viewer.egg-info/
+-rw-r--r--   0 yang      (1000) yang      (1000)     1453 2023-05-01 19:37:09.000000 dbt_lineage_viewer-0.8/dbt_lineage_viewer.egg-info/PKG-INFO
+-rw-r--r--   0 yang      (1000) yang      (1000)      416 2023-05-01 19:37:09.000000 dbt_lineage_viewer-0.8/dbt_lineage_viewer.egg-info/SOURCES.txt
+-rw-r--r--   0 yang      (1000) yang      (1000)        1 2023-05-01 19:37:09.000000 dbt_lineage_viewer-0.8/dbt_lineage_viewer.egg-info/dependency_links.txt
+-rw-r--r--   0 yang      (1000) yang      (1000)       63 2023-05-01 19:37:09.000000 dbt_lineage_viewer-0.8/dbt_lineage_viewer.egg-info/entry_points.txt
+-rw-r--r--   0 yang      (1000) yang      (1000)        6 2023-05-01 19:37:09.000000 dbt_lineage_viewer-0.8/dbt_lineage_viewer.egg-info/requires.txt
+-rw-r--r--   0 yang      (1000) yang      (1000)       19 2023-05-01 19:37:09.000000 dbt_lineage_viewer-0.8/dbt_lineage_viewer.egg-info/top_level.txt
+-rw-r--r--   0 yang      (1000) yang      (1000)       38 2023-05-01 19:37:09.749722 dbt_lineage_viewer-0.8/setup.cfg
+-rw-r--r--   0 yang      (1000) yang      (1000)      675 2023-05-01 19:36:52.000000 dbt_lineage_viewer-0.8/setup.py
```

### Comparing `dbt_lineage_viewer-0.7/PKG-INFO` & `dbt_lineage_viewer-0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt_lineage_viewer
-Version: 0.7
+Version: 0.8
 Summary: A DBT lineage viewer
 Home-page: https://github.com/ydai713/dbt-lineage-viewer
 Author: Yang Dai
 Author-email: yang.dai2020@gmail.com
 Description-Content-Type: text/markdown
 
 # DBT Dependency Viewer
```

### Comparing `dbt_lineage_viewer-0.7/README.md` & `dbt_lineage_viewer-0.8/README.md`

 * *Files identical despite different names*

### Comparing `dbt_lineage_viewer-0.7/dbt_lineage_viewer/main.py` & `dbt_lineage_viewer-0.8/dbt_lineage_viewer/main.py`

 * *Files identical despite different names*

### Comparing `dbt_lineage_viewer-0.7/dbt_lineage_viewer/mermaid.py` & `dbt_lineage_viewer-0.8/dbt_lineage_viewer/mermaid.py`

 * *Files identical despite different names*

### Comparing `dbt_lineage_viewer-0.7/dbt_lineage_viewer/model.py` & `dbt_lineage_viewer-0.8/dbt_lineage_viewer/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,19 +72,19 @@
     return models
 
 
 def generate_downstream_tree(
     parent_model_name: str,
     all_models: Dict[str, str],
     current_depth: int = 0,
-    max_depth: Optional[int] = None
+    max_depth: int = 0
 ) -> Dict[str, Dict]:
     children = {}
 
-    if max_depth is not None and current_depth >= max_depth:
+    if max_depth != 0 and current_depth >= max_depth:
         return children
 
     for model_name, model_content in all_models.items():
         if is_downstream_model(parent_model_name, model_content):
             children[model_name] = generate_downstream_tree(
                 model_name,
                 all_models,
```

### Comparing `dbt_lineage_viewer-0.7/dbt_lineage_viewer.egg-info/PKG-INFO` & `dbt_lineage_viewer-0.8/dbt_lineage_viewer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-lineage-viewer
-Version: 0.7
+Version: 0.8
 Summary: A DBT lineage viewer
 Home-page: https://github.com/ydai713/dbt-lineage-viewer
 Author: Yang Dai
 Author-email: yang.dai2020@gmail.com
 Description-Content-Type: text/markdown
 
 # DBT Dependency Viewer
```

### Comparing `dbt_lineage_viewer-0.7/setup.py` & `dbt_lineage_viewer-0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="dbt_lineage_viewer",
-    version="0.7",
+    version="0.8",
     author="Yang Dai",
     author_email="yang.dai2020@gmail.com",
     description="A DBT lineage viewer",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ydai713/dbt-lineage-viewer",
     packages=find_packages(),
```

