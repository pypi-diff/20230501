# Comparing `tmp/dbt_lineage_viewer-0.6.tar.gz` & `tmp/dbt_lineage_viewer-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt_lineage_viewer-0.6.tar", last modified: Mon May  1 18:26:56 2023, max compression
+gzip compressed data, was "dbt_lineage_viewer-0.7.tar", last modified: Mon May  1 18:29:32 2023, max compression
```

## Comparing `dbt_lineage_viewer-0.6.tar` & `dbt_lineage_viewer-0.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 yang      (1000) yang      (1000)        0 2023-05-01 18:26:56.174421 dbt_lineage_viewer-0.6/
--rw-r--r--   0 yang      (1000) yang      (1000)     1453 2023-05-01 18:26:56.174421 dbt_lineage_viewer-0.6/PKG-INFO
--rw-r--r--   0 yang      (1000) yang      (1000)     1211 2023-05-01 08:59:16.000000 dbt_lineage_viewer-0.6/README.md
-drwxr-xr-x   0 yang      (1000) yang      (1000)        0 2023-05-01 18:26:56.174421 dbt_lineage_viewer-0.6/dbt_lineage_viewer/
--rw-r--r--   0 yang      (1000) yang      (1000)       23 2023-05-01 09:25:49.000000 dbt_lineage_viewer-0.6/dbt_lineage_viewer/__init__.py
--rw-r--r--   0 yang      (1000) yang      (1000)     2903 2023-05-01 18:26:11.000000 dbt_lineage_viewer-0.6/dbt_lineage_viewer/main.py
--rw-r--r--   0 yang      (1000) yang      (1000)     1452 2023-05-01 09:24:52.000000 dbt_lineage_viewer-0.6/dbt_lineage_viewer/mermaid.py
--rw-r--r--   0 yang      (1000) yang      (1000)     3650 2023-05-01 18:26:05.000000 dbt_lineage_viewer-0.6/dbt_lineage_viewer/model.py
--rw-r--r--   0 yang      (1000) yang      (1000)      237 2023-05-01 16:49:00.000000 dbt_lineage_viewer-0.6/dbt_lineage_viewer/utils.py
-drwxr-xr-x   0 yang      (1000) yang      (1000)        0 2023-05-01 18:26:56.174421 dbt_lineage_viewer-0.6/dbt_lineage_viewer.egg-info/
--rw-r--r--   0 yang      (1000) yang      (1000)     1453 2023-05-01 18:26:56.000000 dbt_lineage_viewer-0.6/dbt_lineage_viewer.egg-info/PKG-INFO
--rw-r--r--   0 yang      (1000) yang      (1000)      416 2023-05-01 18:26:56.000000 dbt_lineage_viewer-0.6/dbt_lineage_viewer.egg-info/SOURCES.txt
--rw-r--r--   0 yang      (1000) yang      (1000)        1 2023-05-01 18:26:56.000000 dbt_lineage_viewer-0.6/dbt_lineage_viewer.egg-info/dependency_links.txt
--rw-r--r--   0 yang      (1000) yang      (1000)       63 2023-05-01 18:26:56.000000 dbt_lineage_viewer-0.6/dbt_lineage_viewer.egg-info/entry_points.txt
--rw-r--r--   0 yang      (1000) yang      (1000)        6 2023-05-01 18:26:56.000000 dbt_lineage_viewer-0.6/dbt_lineage_viewer.egg-info/requires.txt
--rw-r--r--   0 yang      (1000) yang      (1000)       19 2023-05-01 18:26:56.000000 dbt_lineage_viewer-0.6/dbt_lineage_viewer.egg-info/top_level.txt
--rw-r--r--   0 yang      (1000) yang      (1000)       38 2023-05-01 18:26:56.174421 dbt_lineage_viewer-0.6/setup.cfg
--rw-r--r--   0 yang      (1000) yang      (1000)      675 2023-05-01 18:26:41.000000 dbt_lineage_viewer-0.6/setup.py
+drwxr-xr-x   0 yang      (1000) yang      (1000)        0 2023-05-01 18:29:32.438627 dbt_lineage_viewer-0.7/
+-rw-r--r--   0 yang      (1000) yang      (1000)     1453 2023-05-01 18:29:32.438627 dbt_lineage_viewer-0.7/PKG-INFO
+-rw-r--r--   0 yang      (1000) yang      (1000)     1211 2023-05-01 08:59:16.000000 dbt_lineage_viewer-0.7/README.md
+drwxr-xr-x   0 yang      (1000) yang      (1000)        0 2023-05-01 18:29:32.438627 dbt_lineage_viewer-0.7/dbt_lineage_viewer/
+-rw-r--r--   0 yang      (1000) yang      (1000)       23 2023-05-01 09:25:49.000000 dbt_lineage_viewer-0.7/dbt_lineage_viewer/__init__.py
+-rw-r--r--   0 yang      (1000) yang      (1000)     2903 2023-05-01 18:29:11.000000 dbt_lineage_viewer-0.7/dbt_lineage_viewer/main.py
+-rw-r--r--   0 yang      (1000) yang      (1000)     1452 2023-05-01 09:24:52.000000 dbt_lineage_viewer-0.7/dbt_lineage_viewer/mermaid.py
+-rw-r--r--   0 yang      (1000) yang      (1000)     3650 2023-05-01 18:26:05.000000 dbt_lineage_viewer-0.7/dbt_lineage_viewer/model.py
+-rw-r--r--   0 yang      (1000) yang      (1000)      237 2023-05-01 16:49:00.000000 dbt_lineage_viewer-0.7/dbt_lineage_viewer/utils.py
+drwxr-xr-x   0 yang      (1000) yang      (1000)        0 2023-05-01 18:29:32.438627 dbt_lineage_viewer-0.7/dbt_lineage_viewer.egg-info/
+-rw-r--r--   0 yang      (1000) yang      (1000)     1453 2023-05-01 18:29:32.000000 dbt_lineage_viewer-0.7/dbt_lineage_viewer.egg-info/PKG-INFO
+-rw-r--r--   0 yang      (1000) yang      (1000)      416 2023-05-01 18:29:32.000000 dbt_lineage_viewer-0.7/dbt_lineage_viewer.egg-info/SOURCES.txt
+-rw-r--r--   0 yang      (1000) yang      (1000)        1 2023-05-01 18:29:32.000000 dbt_lineage_viewer-0.7/dbt_lineage_viewer.egg-info/dependency_links.txt
+-rw-r--r--   0 yang      (1000) yang      (1000)       63 2023-05-01 18:29:32.000000 dbt_lineage_viewer-0.7/dbt_lineage_viewer.egg-info/entry_points.txt
+-rw-r--r--   0 yang      (1000) yang      (1000)        6 2023-05-01 18:29:32.000000 dbt_lineage_viewer-0.7/dbt_lineage_viewer.egg-info/requires.txt
+-rw-r--r--   0 yang      (1000) yang      (1000)       19 2023-05-01 18:29:32.000000 dbt_lineage_viewer-0.7/dbt_lineage_viewer.egg-info/top_level.txt
+-rw-r--r--   0 yang      (1000) yang      (1000)       38 2023-05-01 18:29:32.438627 dbt_lineage_viewer-0.7/setup.cfg
+-rw-r--r--   0 yang      (1000) yang      (1000)      675 2023-05-01 18:29:21.000000 dbt_lineage_viewer-0.7/setup.py
```

### Comparing `dbt_lineage_viewer-0.6/PKG-INFO` & `dbt_lineage_viewer-0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt_lineage_viewer
-Version: 0.6
+Version: 0.7
 Summary: A DBT lineage viewer
 Home-page: https://github.com/ydai713/dbt-lineage-viewer
 Author: Yang Dai
 Author-email: yang.dai2020@gmail.com
 Description-Content-Type: text/markdown
 
 # DBT Dependency Viewer
```

### Comparing `dbt_lineage_viewer-0.6/README.md` & `dbt_lineage_viewer-0.7/README.md`

 * *Files identical despite different names*

### Comparing `dbt_lineage_viewer-0.6/dbt_lineage_viewer/main.py` & `dbt_lineage_viewer-0.7/dbt_lineage_viewer/main.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -77,10 +77,10 @@
         flowchart LR
         {downstream_chart}
         {upstream_chart}
     """
 
     # Wrap mermaid code with html and output it so can be displayed
     # in local browser
-    output = generate_local_file_url(output)
     export_diagram_to_html(output, mermaid_code)
+    output = generate_local_file_url(output)
     print(output)
```

### Comparing `dbt_lineage_viewer-0.6/dbt_lineage_viewer/mermaid.py` & `dbt_lineage_viewer-0.7/dbt_lineage_viewer/mermaid.py`

 * *Files identical despite different names*

### Comparing `dbt_lineage_viewer-0.6/dbt_lineage_viewer/model.py` & `dbt_lineage_viewer-0.7/dbt_lineage_viewer/model.py`

 * *Files identical despite different names*

### Comparing `dbt_lineage_viewer-0.6/dbt_lineage_viewer.egg-info/PKG-INFO` & `dbt_lineage_viewer-0.7/dbt_lineage_viewer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-lineage-viewer
-Version: 0.6
+Version: 0.7
 Summary: A DBT lineage viewer
 Home-page: https://github.com/ydai713/dbt-lineage-viewer
 Author: Yang Dai
 Author-email: yang.dai2020@gmail.com
 Description-Content-Type: text/markdown
 
 # DBT Dependency Viewer
```

### Comparing `dbt_lineage_viewer-0.6/setup.py` & `dbt_lineage_viewer-0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="dbt_lineage_viewer",
-    version="0.6",
+    version="0.7",
     author="Yang Dai",
     author_email="yang.dai2020@gmail.com",
     description="A DBT lineage viewer",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ydai713/dbt-lineage-viewer",
     packages=find_packages(),
```

