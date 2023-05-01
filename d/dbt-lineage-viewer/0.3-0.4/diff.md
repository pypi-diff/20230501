# Comparing `tmp/dbt_lineage_viewer-0.3.tar.gz` & `tmp/dbt_lineage_viewer-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt_lineage_viewer-0.3.tar", last modified: Mon May  1 09:20:38 2023, max compression
+gzip compressed data, was "dbt_lineage_viewer-0.4.tar", last modified: Mon May  1 09:28:17 2023, max compression
```

## Comparing `dbt_lineage_viewer-0.3.tar` & `dbt_lineage_viewer-0.4.tar`

### file list

```diff
@@ -1,12 +1,17 @@
-drwxr-xr-x   0 yang      (1000) yang      (1000)        0 2023-05-01 09:20:38.533777 dbt_lineage_viewer-0.3/
--rw-r--r--   0 yang      (1000) yang      (1000)     1453 2023-05-01 09:20:38.533777 dbt_lineage_viewer-0.3/PKG-INFO
--rw-r--r--   0 yang      (1000) yang      (1000)     1211 2023-05-01 08:59:16.000000 dbt_lineage_viewer-0.3/README.md
-drwxr-xr-x   0 yang      (1000) yang      (1000)        0 2023-05-01 09:20:38.533777 dbt_lineage_viewer-0.3/dbt_lineage_viewer.egg-info/
--rw-r--r--   0 yang      (1000) yang      (1000)     1453 2023-05-01 09:20:38.000000 dbt_lineage_viewer-0.3/dbt_lineage_viewer.egg-info/PKG-INFO
--rw-r--r--   0 yang      (1000) yang      (1000)      272 2023-05-01 09:20:38.000000 dbt_lineage_viewer-0.3/dbt_lineage_viewer.egg-info/SOURCES.txt
--rw-r--r--   0 yang      (1000) yang      (1000)        1 2023-05-01 09:20:38.000000 dbt_lineage_viewer-0.3/dbt_lineage_viewer.egg-info/dependency_links.txt
--rw-r--r--   0 yang      (1000) yang      (1000)       63 2023-05-01 09:20:38.000000 dbt_lineage_viewer-0.3/dbt_lineage_viewer.egg-info/entry_points.txt
--rw-r--r--   0 yang      (1000) yang      (1000)        6 2023-05-01 09:20:38.000000 dbt_lineage_viewer-0.3/dbt_lineage_viewer.egg-info/requires.txt
--rw-r--r--   0 yang      (1000) yang      (1000)        1 2023-05-01 09:20:38.000000 dbt_lineage_viewer-0.3/dbt_lineage_viewer.egg-info/top_level.txt
--rw-r--r--   0 yang      (1000) yang      (1000)       38 2023-05-01 09:20:38.533777 dbt_lineage_viewer-0.3/setup.cfg
--rw-r--r--   0 yang      (1000) yang      (1000)      675 2023-05-01 09:20:07.000000 dbt_lineage_viewer-0.3/setup.py
+drwxr-xr-x   0 yang      (1000) yang      (1000)        0 2023-05-01 09:28:17.469778 dbt_lineage_viewer-0.4/
+-rw-r--r--   0 yang      (1000) yang      (1000)     1453 2023-05-01 09:28:17.469778 dbt_lineage_viewer-0.4/PKG-INFO
+-rw-r--r--   0 yang      (1000) yang      (1000)     1211 2023-05-01 08:59:16.000000 dbt_lineage_viewer-0.4/README.md
+drwxr-xr-x   0 yang      (1000) yang      (1000)        0 2023-05-01 09:28:17.469778 dbt_lineage_viewer-0.4/dbt_lineage_viewer/
+-rw-r--r--   0 yang      (1000) yang      (1000)       23 2023-05-01 09:25:49.000000 dbt_lineage_viewer-0.4/dbt_lineage_viewer/__init__.py
+-rw-r--r--   0 yang      (1000) yang      (1000)     2345 2023-05-01 09:26:18.000000 dbt_lineage_viewer-0.4/dbt_lineage_viewer/main.py
+-rw-r--r--   0 yang      (1000) yang      (1000)     1452 2023-05-01 09:24:52.000000 dbt_lineage_viewer-0.4/dbt_lineage_viewer/mermaid.py
+-rw-r--r--   0 yang      (1000) yang      (1000)     3667 2023-05-01 09:24:55.000000 dbt_lineage_viewer-0.4/dbt_lineage_viewer/model.py
+drwxr-xr-x   0 yang      (1000) yang      (1000)        0 2023-05-01 09:28:17.469778 dbt_lineage_viewer-0.4/dbt_lineage_viewer.egg-info/
+-rw-r--r--   0 yang      (1000) yang      (1000)     1453 2023-05-01 09:28:17.000000 dbt_lineage_viewer-0.4/dbt_lineage_viewer.egg-info/PKG-INFO
+-rw-r--r--   0 yang      (1000) yang      (1000)      388 2023-05-01 09:28:17.000000 dbt_lineage_viewer-0.4/dbt_lineage_viewer.egg-info/SOURCES.txt
+-rw-r--r--   0 yang      (1000) yang      (1000)        1 2023-05-01 09:28:17.000000 dbt_lineage_viewer-0.4/dbt_lineage_viewer.egg-info/dependency_links.txt
+-rw-r--r--   0 yang      (1000) yang      (1000)       63 2023-05-01 09:28:17.000000 dbt_lineage_viewer-0.4/dbt_lineage_viewer.egg-info/entry_points.txt
+-rw-r--r--   0 yang      (1000) yang      (1000)        6 2023-05-01 09:28:17.000000 dbt_lineage_viewer-0.4/dbt_lineage_viewer.egg-info/requires.txt
+-rw-r--r--   0 yang      (1000) yang      (1000)       19 2023-05-01 09:28:17.000000 dbt_lineage_viewer-0.4/dbt_lineage_viewer.egg-info/top_level.txt
+-rw-r--r--   0 yang      (1000) yang      (1000)       38 2023-05-01 09:28:17.469778 dbt_lineage_viewer-0.4/setup.cfg
+-rw-r--r--   0 yang      (1000) yang      (1000)      675 2023-05-01 09:27:59.000000 dbt_lineage_viewer-0.4/setup.py
```

### Comparing `dbt_lineage_viewer-0.3/PKG-INFO` & `dbt_lineage_viewer-0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt_lineage_viewer
-Version: 0.3
+Version: 0.4
 Summary: A DBT lineage viewer
 Home-page: https://github.com/ydai713/dbt-lineage-viewer
 Author: Yang Dai
 Author-email: yang.dai2020@gmail.com
 Description-Content-Type: text/markdown
 
 # DBT Dependency Viewer
```

### Comparing `dbt_lineage_viewer-0.3/README.md` & `dbt_lineage_viewer-0.4/README.md`

 * *Files identical despite different names*

### Comparing `dbt_lineage_viewer-0.3/dbt_lineage_viewer.egg-info/PKG-INFO` & `dbt_lineage_viewer-0.4/dbt_lineage_viewer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-lineage-viewer
-Version: 0.3
+Version: 0.4
 Summary: A DBT lineage viewer
 Home-page: https://github.com/ydai713/dbt-lineage-viewer
 Author: Yang Dai
 Author-email: yang.dai2020@gmail.com
 Description-Content-Type: text/markdown
 
 # DBT Dependency Viewer
```

### Comparing `dbt_lineage_viewer-0.3/setup.py` & `dbt_lineage_viewer-0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="dbt_lineage_viewer",
-    version="0.3",
+    version="0.4",
     author="Yang Dai",
     author_email="yang.dai2020@gmail.com",
     description="A DBT lineage viewer",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ydai713/dbt-lineage-viewer",
     packages=find_packages(),
```

