# Comparing `tmp/dbt_lineage_viewer-1.0.tar.gz` & `tmp/dbt_lineage_viewer-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt_lineage_viewer-1.0.tar", last modified: Mon May  1 19:40:55 2023, max compression
+gzip compressed data, was "dbt_lineage_viewer-1.0.1.tar", last modified: Mon May  1 19:42:46 2023, max compression
```

## Comparing `dbt_lineage_viewer-1.0.tar` & `dbt_lineage_viewer-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 yang      (1000) yang      (1000)        0 2023-05-01 19:40:55.339120 dbt_lineage_viewer-1.0/
--rw-r--r--   0 yang      (1000) yang      (1000)     1453 2023-05-01 19:40:55.339120 dbt_lineage_viewer-1.0/PKG-INFO
--rw-r--r--   0 yang      (1000) yang      (1000)     1211 2023-05-01 08:59:16.000000 dbt_lineage_viewer-1.0/README.md
-drwxr-xr-x   0 yang      (1000) yang      (1000)        0 2023-05-01 19:40:55.339120 dbt_lineage_viewer-1.0/dbt_lineage_viewer/
--rw-r--r--   0 yang      (1000) yang      (1000)       23 2023-05-01 09:25:49.000000 dbt_lineage_viewer-1.0/dbt_lineage_viewer/__init__.py
--rw-r--r--   0 yang      (1000) yang      (1000)     2903 2023-05-01 18:29:11.000000 dbt_lineage_viewer-1.0/dbt_lineage_viewer/main.py
--rw-r--r--   0 yang      (1000) yang      (1000)     1636 2023-05-01 19:40:21.000000 dbt_lineage_viewer-1.0/dbt_lineage_viewer/mermaid.py
--rw-r--r--   0 yang      (1000) yang      (1000)     3630 2023-05-01 19:35:46.000000 dbt_lineage_viewer-1.0/dbt_lineage_viewer/model.py
--rw-r--r--   0 yang      (1000) yang      (1000)      237 2023-05-01 16:49:00.000000 dbt_lineage_viewer-1.0/dbt_lineage_viewer/utils.py
-drwxr-xr-x   0 yang      (1000) yang      (1000)        0 2023-05-01 19:40:55.339120 dbt_lineage_viewer-1.0/dbt_lineage_viewer.egg-info/
--rw-r--r--   0 yang      (1000) yang      (1000)     1453 2023-05-01 19:40:55.000000 dbt_lineage_viewer-1.0/dbt_lineage_viewer.egg-info/PKG-INFO
--rw-r--r--   0 yang      (1000) yang      (1000)      416 2023-05-01 19:40:55.000000 dbt_lineage_viewer-1.0/dbt_lineage_viewer.egg-info/SOURCES.txt
--rw-r--r--   0 yang      (1000) yang      (1000)        1 2023-05-01 19:40:55.000000 dbt_lineage_viewer-1.0/dbt_lineage_viewer.egg-info/dependency_links.txt
--rw-r--r--   0 yang      (1000) yang      (1000)       63 2023-05-01 19:40:55.000000 dbt_lineage_viewer-1.0/dbt_lineage_viewer.egg-info/entry_points.txt
--rw-r--r--   0 yang      (1000) yang      (1000)        6 2023-05-01 19:40:55.000000 dbt_lineage_viewer-1.0/dbt_lineage_viewer.egg-info/requires.txt
--rw-r--r--   0 yang      (1000) yang      (1000)       19 2023-05-01 19:40:55.000000 dbt_lineage_viewer-1.0/dbt_lineage_viewer.egg-info/top_level.txt
--rw-r--r--   0 yang      (1000) yang      (1000)       38 2023-05-01 19:40:55.339120 dbt_lineage_viewer-1.0/setup.cfg
--rw-r--r--   0 yang      (1000) yang      (1000)      675 2023-05-01 19:40:48.000000 dbt_lineage_viewer-1.0/setup.py
+drwxr-xr-x   0 yang      (1000) yang      (1000)        0 2023-05-01 19:42:46.365438 dbt_lineage_viewer-1.0.1/
+-rw-r--r--   0 yang      (1000) yang      (1000)     1455 2023-05-01 19:42:46.365438 dbt_lineage_viewer-1.0.1/PKG-INFO
+-rw-r--r--   0 yang      (1000) yang      (1000)     1211 2023-05-01 08:59:16.000000 dbt_lineage_viewer-1.0.1/README.md
+drwxr-xr-x   0 yang      (1000) yang      (1000)        0 2023-05-01 19:42:46.365438 dbt_lineage_viewer-1.0.1/dbt_lineage_viewer/
+-rw-r--r--   0 yang      (1000) yang      (1000)       23 2023-05-01 09:25:49.000000 dbt_lineage_viewer-1.0.1/dbt_lineage_viewer/__init__.py
+-rw-r--r--   0 yang      (1000) yang      (1000)     2903 2023-05-01 18:29:11.000000 dbt_lineage_viewer-1.0.1/dbt_lineage_viewer/main.py
+-rw-r--r--   0 yang      (1000) yang      (1000)     1637 2023-05-01 19:41:55.000000 dbt_lineage_viewer-1.0.1/dbt_lineage_viewer/mermaid.py
+-rw-r--r--   0 yang      (1000) yang      (1000)     3630 2023-05-01 19:35:46.000000 dbt_lineage_viewer-1.0.1/dbt_lineage_viewer/model.py
+-rw-r--r--   0 yang      (1000) yang      (1000)      237 2023-05-01 16:49:00.000000 dbt_lineage_viewer-1.0.1/dbt_lineage_viewer/utils.py
+drwxr-xr-x   0 yang      (1000) yang      (1000)        0 2023-05-01 19:42:46.365438 dbt_lineage_viewer-1.0.1/dbt_lineage_viewer.egg-info/
+-rw-r--r--   0 yang      (1000) yang      (1000)     1455 2023-05-01 19:42:46.000000 dbt_lineage_viewer-1.0.1/dbt_lineage_viewer.egg-info/PKG-INFO
+-rw-r--r--   0 yang      (1000) yang      (1000)      416 2023-05-01 19:42:46.000000 dbt_lineage_viewer-1.0.1/dbt_lineage_viewer.egg-info/SOURCES.txt
+-rw-r--r--   0 yang      (1000) yang      (1000)        1 2023-05-01 19:42:46.000000 dbt_lineage_viewer-1.0.1/dbt_lineage_viewer.egg-info/dependency_links.txt
+-rw-r--r--   0 yang      (1000) yang      (1000)       63 2023-05-01 19:42:46.000000 dbt_lineage_viewer-1.0.1/dbt_lineage_viewer.egg-info/entry_points.txt
+-rw-r--r--   0 yang      (1000) yang      (1000)        6 2023-05-01 19:42:46.000000 dbt_lineage_viewer-1.0.1/dbt_lineage_viewer.egg-info/requires.txt
+-rw-r--r--   0 yang      (1000) yang      (1000)       19 2023-05-01 19:42:46.000000 dbt_lineage_viewer-1.0.1/dbt_lineage_viewer.egg-info/top_level.txt
+-rw-r--r--   0 yang      (1000) yang      (1000)       38 2023-05-01 19:42:46.365438 dbt_lineage_viewer-1.0.1/setup.cfg
+-rw-r--r--   0 yang      (1000) yang      (1000)      677 2023-05-01 19:42:34.000000 dbt_lineage_viewer-1.0.1/setup.py
```

### Comparing `dbt_lineage_viewer-1.0/PKG-INFO` & `dbt_lineage_viewer-1.0.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt_lineage_viewer
-Version: 1.0
+Version: 1.0.1
 Summary: A DBT lineage viewer
 Home-page: https://github.com/ydai713/dbt-lineage-viewer
 Author: Yang Dai
 Author-email: yang.dai2020@gmail.com
 Description-Content-Type: text/markdown
 
 # DBT Dependency Viewer
```

### Comparing `dbt_lineage_viewer-1.0/README.md` & `dbt_lineage_viewer-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `dbt_lineage_viewer-1.0/dbt_lineage_viewer/main.py` & `dbt_lineage_viewer-1.0.1/dbt_lineage_viewer/main.py`

 * *Files identical despite different names*

### Comparing `dbt_lineage_viewer-1.0/dbt_lineage_viewer/mermaid.py` & `dbt_lineage_viewer-1.0.1/dbt_lineage_viewer/mermaid.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,14 +20,15 @@
             if key not in mentioned_nodes:
                 mentioned_nodes.add(key)
             if edge not in visited_edges:
                 visited_edges.add(edge)
                 # this is a bug from mermaid (click is a mermaid keyword)
                 key = key.replace("click", "Click")
                 parent = parent.replace("click", "Click")
+
                 code += (
                     f"{key} --> {parent}\n" if not downstream 
                     else f"{parent} --> {key}\n"
                 )
         if value:
             code += generate_mermaid_code(
                 value,
```

### Comparing `dbt_lineage_viewer-1.0/dbt_lineage_viewer/model.py` & `dbt_lineage_viewer-1.0.1/dbt_lineage_viewer/model.py`

 * *Files identical despite different names*

### Comparing `dbt_lineage_viewer-1.0/dbt_lineage_viewer.egg-info/PKG-INFO` & `dbt_lineage_viewer-1.0.1/dbt_lineage_viewer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-lineage-viewer
-Version: 1.0
+Version: 1.0.1
 Summary: A DBT lineage viewer
 Home-page: https://github.com/ydai713/dbt-lineage-viewer
 Author: Yang Dai
 Author-email: yang.dai2020@gmail.com
 Description-Content-Type: text/markdown
 
 # DBT Dependency Viewer
```

### Comparing `dbt_lineage_viewer-1.0/setup.py` & `dbt_lineage_viewer-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="dbt_lineage_viewer",
-    version="1.0",
+    version="1.0.1",
     author="Yang Dai",
     author_email="yang.dai2020@gmail.com",
     description="A DBT lineage viewer",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ydai713/dbt-lineage-viewer",
     packages=find_packages(),
```

