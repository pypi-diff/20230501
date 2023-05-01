# Comparing `tmp/dbt_lineage_viewer-0.4.tar.gz` & `tmp/dbt_lineage_viewer-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt_lineage_viewer-0.4.tar", last modified: Mon May  1 09:28:17 2023, max compression
+gzip compressed data, was "dbt_lineage_viewer-0.5.tar", last modified: Mon May  1 18:17:58 2023, max compression
```

## Comparing `dbt_lineage_viewer-0.4.tar` & `dbt_lineage_viewer-0.5.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 yang      (1000) yang      (1000)        0 2023-05-01 09:28:17.469778 dbt_lineage_viewer-0.4/
--rw-r--r--   0 yang      (1000) yang      (1000)     1453 2023-05-01 09:28:17.469778 dbt_lineage_viewer-0.4/PKG-INFO
--rw-r--r--   0 yang      (1000) yang      (1000)     1211 2023-05-01 08:59:16.000000 dbt_lineage_viewer-0.4/README.md
-drwxr-xr-x   0 yang      (1000) yang      (1000)        0 2023-05-01 09:28:17.469778 dbt_lineage_viewer-0.4/dbt_lineage_viewer/
--rw-r--r--   0 yang      (1000) yang      (1000)       23 2023-05-01 09:25:49.000000 dbt_lineage_viewer-0.4/dbt_lineage_viewer/__init__.py
--rw-r--r--   0 yang      (1000) yang      (1000)     2345 2023-05-01 09:26:18.000000 dbt_lineage_viewer-0.4/dbt_lineage_viewer/main.py
--rw-r--r--   0 yang      (1000) yang      (1000)     1452 2023-05-01 09:24:52.000000 dbt_lineage_viewer-0.4/dbt_lineage_viewer/mermaid.py
--rw-r--r--   0 yang      (1000) yang      (1000)     3667 2023-05-01 09:24:55.000000 dbt_lineage_viewer-0.4/dbt_lineage_viewer/model.py
-drwxr-xr-x   0 yang      (1000) yang      (1000)        0 2023-05-01 09:28:17.469778 dbt_lineage_viewer-0.4/dbt_lineage_viewer.egg-info/
--rw-r--r--   0 yang      (1000) yang      (1000)     1453 2023-05-01 09:28:17.000000 dbt_lineage_viewer-0.4/dbt_lineage_viewer.egg-info/PKG-INFO
--rw-r--r--   0 yang      (1000) yang      (1000)      388 2023-05-01 09:28:17.000000 dbt_lineage_viewer-0.4/dbt_lineage_viewer.egg-info/SOURCES.txt
--rw-r--r--   0 yang      (1000) yang      (1000)        1 2023-05-01 09:28:17.000000 dbt_lineage_viewer-0.4/dbt_lineage_viewer.egg-info/dependency_links.txt
--rw-r--r--   0 yang      (1000) yang      (1000)       63 2023-05-01 09:28:17.000000 dbt_lineage_viewer-0.4/dbt_lineage_viewer.egg-info/entry_points.txt
--rw-r--r--   0 yang      (1000) yang      (1000)        6 2023-05-01 09:28:17.000000 dbt_lineage_viewer-0.4/dbt_lineage_viewer.egg-info/requires.txt
--rw-r--r--   0 yang      (1000) yang      (1000)       19 2023-05-01 09:28:17.000000 dbt_lineage_viewer-0.4/dbt_lineage_viewer.egg-info/top_level.txt
--rw-r--r--   0 yang      (1000) yang      (1000)       38 2023-05-01 09:28:17.469778 dbt_lineage_viewer-0.4/setup.cfg
--rw-r--r--   0 yang      (1000) yang      (1000)      675 2023-05-01 09:27:59.000000 dbt_lineage_viewer-0.4/setup.py
+drwxr-xr-x   0 yang      (1000) yang      (1000)        0 2023-05-01 18:17:58.973424 dbt_lineage_viewer-0.5/
+-rw-r--r--   0 yang      (1000) yang      (1000)     1453 2023-05-01 18:17:58.973424 dbt_lineage_viewer-0.5/PKG-INFO
+-rw-r--r--   0 yang      (1000) yang      (1000)     1211 2023-05-01 08:59:16.000000 dbt_lineage_viewer-0.5/README.md
+drwxr-xr-x   0 yang      (1000) yang      (1000)        0 2023-05-01 18:17:58.973424 dbt_lineage_viewer-0.5/dbt_lineage_viewer/
+-rw-r--r--   0 yang      (1000) yang      (1000)       23 2023-05-01 09:25:49.000000 dbt_lineage_viewer-0.5/dbt_lineage_viewer/__init__.py
+-rw-r--r--   0 yang      (1000) yang      (1000)     2903 2023-05-01 18:16:57.000000 dbt_lineage_viewer-0.5/dbt_lineage_viewer/main.py
+-rw-r--r--   0 yang      (1000) yang      (1000)     1452 2023-05-01 09:24:52.000000 dbt_lineage_viewer-0.5/dbt_lineage_viewer/mermaid.py
+-rw-r--r--   0 yang      (1000) yang      (1000)     3670 2023-05-01 16:40:21.000000 dbt_lineage_viewer-0.5/dbt_lineage_viewer/model.py
+-rw-r--r--   0 yang      (1000) yang      (1000)      237 2023-05-01 16:49:00.000000 dbt_lineage_viewer-0.5/dbt_lineage_viewer/utils.py
+drwxr-xr-x   0 yang      (1000) yang      (1000)        0 2023-05-01 18:17:58.973424 dbt_lineage_viewer-0.5/dbt_lineage_viewer.egg-info/
+-rw-r--r--   0 yang      (1000) yang      (1000)     1453 2023-05-01 18:17:58.000000 dbt_lineage_viewer-0.5/dbt_lineage_viewer.egg-info/PKG-INFO
+-rw-r--r--   0 yang      (1000) yang      (1000)      416 2023-05-01 18:17:58.000000 dbt_lineage_viewer-0.5/dbt_lineage_viewer.egg-info/SOURCES.txt
+-rw-r--r--   0 yang      (1000) yang      (1000)        1 2023-05-01 18:17:58.000000 dbt_lineage_viewer-0.5/dbt_lineage_viewer.egg-info/dependency_links.txt
+-rw-r--r--   0 yang      (1000) yang      (1000)       63 2023-05-01 18:17:58.000000 dbt_lineage_viewer-0.5/dbt_lineage_viewer.egg-info/entry_points.txt
+-rw-r--r--   0 yang      (1000) yang      (1000)        6 2023-05-01 18:17:58.000000 dbt_lineage_viewer-0.5/dbt_lineage_viewer.egg-info/requires.txt
+-rw-r--r--   0 yang      (1000) yang      (1000)       19 2023-05-01 18:17:58.000000 dbt_lineage_viewer-0.5/dbt_lineage_viewer.egg-info/top_level.txt
+-rw-r--r--   0 yang      (1000) yang      (1000)       38 2023-05-01 18:17:58.973424 dbt_lineage_viewer-0.5/setup.cfg
+-rw-r--r--   0 yang      (1000) yang      (1000)      675 2023-05-01 18:17:24.000000 dbt_lineage_viewer-0.5/setup.py
```

### Comparing `dbt_lineage_viewer-0.4/PKG-INFO` & `dbt_lineage_viewer-0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt_lineage_viewer
-Version: 0.4
+Version: 0.5
 Summary: A DBT lineage viewer
 Home-page: https://github.com/ydai713/dbt-lineage-viewer
 Author: Yang Dai
 Author-email: yang.dai2020@gmail.com
 Description-Content-Type: text/markdown
 
 # DBT Dependency Viewer
```

### Comparing `dbt_lineage_viewer-0.4/README.md` & `dbt_lineage_viewer-0.5/README.md`

 * *Files identical despite different names*

### Comparing `dbt_lineage_viewer-0.4/dbt_lineage_viewer/main.py` & `dbt_lineage_viewer-0.5/dbt_lineage_viewer/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,63 +9,78 @@
 from .model import generate_downstream_tree
 from .model import generate_upstream_tree
 from .model import get_all_models
 
 from .mermaid import export_diagram_to_html
 from .mermaid import generate_mermaid_code
 
+from .utils import generate_local_file_url
+
 import click
 
 
 @click.command()
 @click.argument("model_name")
 @click.option("--max-depth", default=2, help="Maximum depth of dependencies.")
 @click.option("--output", default="test.html", help="Output HTML file path.")
 @click.option("--model-dir-name", default="models", help="Model folder name")
 @click.option("--data-dir-name", default="data", help="Data folder name")
 @click.option("--snapshot-dir-name", default="snapshots", help="Snapshots folder name")
+@click.option("--upstream-only", is_flag=True, help="Show upstream models only.")
+@click.option("--downstream-only", is_flag=True, help="Show downstream models only.")
 def main(
     model_name: str,
     max_depth: int,
     output: str,
     model_dir_name: str,
     data_dir_name: str,
-    snapshot_dir_name
+    snapshot_dir_name,
+    upstream_only: bool,
+    downstream_only: bool
 
 ):
+    if upstream_only and downstream_only:
+        print("Cannot use --upstream-only and --downstream-only together.")
+        exit(1)
+
     try:
         project_root = find_dbt_project_root()
     except FileNotFoundError as error:
         print(error)
         exit(1)
 
     # Time consuming
     all_models = get_all_models(
         project_root, model_dir_name, data_dir_name, snapshot_dir_name
     )
 
+    if not all_models.get(model_name):
+        print(f"Error: Could not find model {model_name}")
+        exit(1)
+
     # Traverse downstream models (slower with bigget max_depth)
     downstream_models = generate_downstream_tree(
         model_name, all_models, max_depth=max_depth
-    )
+    ) if not upstream_only else {}
     downstream_tree = { model_name: downstream_models }
 
     # Traverse upstream models (fast, max_depth has little effect)
     upstream_models = generate_upstream_tree(
         model_name, all_models, max_depth=max_depth
-    )
+    ) if not downstream_only else {}
     upstream_tree = { model_name: upstream_models }
 
     # Convert dependency tree to mermaid code
     downstream_chart = generate_mermaid_code(downstream_tree, downstream=True)
     upstream_chart = generate_mermaid_code(upstream_tree, downstream=False)
 
     mermaid_code = f"""
         flowchart LR
         {downstream_chart}
         {upstream_chart}
     """
 
     # Wrap mermaid code with html and output it so can be displayed
     # in local browser
+    output = generate_local_file_url(output)
     export_diagram_to_html(output, mermaid_code)
-    print(f"You can now open {output} with your browser to view dependencies")
+    print(output)
```

### Comparing `dbt_lineage_viewer-0.4/dbt_lineage_viewer/mermaid.py` & `dbt_lineage_viewer-0.5/dbt_lineage_viewer/mermaid.py`

 * *Files identical despite different names*

### Comparing `dbt_lineage_viewer-0.4/dbt_lineage_viewer/model.py` & `dbt_lineage_viewer-0.5/dbt_lineage_viewer/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,14 +114,14 @@
                 parents[model_name] = generate_upstream_tree(
                     model_name,
                     all_models,
                     current_depth=current_depth + 1,
                     max_depth=max_depth
                 )
             except KeyError:
-                print("warning: you might have a dynamic dependency")
+                print(f"Warning: {model_name} is dynamically generated")
         elif model_type == "source":
             parents[model_name] = {}
 
     return parents
```

### Comparing `dbt_lineage_viewer-0.4/dbt_lineage_viewer.egg-info/PKG-INFO` & `dbt_lineage_viewer-0.5/dbt_lineage_viewer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-lineage-viewer
-Version: 0.4
+Version: 0.5
 Summary: A DBT lineage viewer
 Home-page: https://github.com/ydai713/dbt-lineage-viewer
 Author: Yang Dai
 Author-email: yang.dai2020@gmail.com
 Description-Content-Type: text/markdown
 
 # DBT Dependency Viewer
```

### Comparing `dbt_lineage_viewer-0.4/setup.py` & `dbt_lineage_viewer-0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="dbt_lineage_viewer",
-    version="0.4",
+    version="0.5",
     author="Yang Dai",
     author_email="yang.dai2020@gmail.com",
     description="A DBT lineage viewer",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ydai713/dbt-lineage-viewer",
     packages=find_packages(),
```

