# Comparing `tmp/dbt_lineage_viewer-0.1.tar.gz` & `tmp/dbt_lineage_viewer-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt_lineage_viewer-0.1.tar", last modified: Mon May  1 09:07:45 2023, max compression
+gzip compressed data, was "dbt_lineage_viewer-0.2.tar", last modified: Mon May  1 09:13:59 2023, max compression
```

## Comparing `dbt_lineage_viewer-0.1.tar` & `dbt_lineage_viewer-0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 yang      (1000) yang      (1000)        0 2023-05-01 09:07:45.230232 dbt_lineage_viewer-0.1/
--rw-r--r--   0 yang      (1000) yang      (1000)     1453 2023-05-01 09:07:45.230232 dbt_lineage_viewer-0.1/PKG-INFO
--rw-r--r--   0 yang      (1000) yang      (1000)     1211 2023-05-01 08:59:16.000000 dbt_lineage_viewer-0.1/README.md
-drwxr-xr-x   0 yang      (1000) yang      (1000)        0 2023-05-01 09:07:45.230232 dbt_lineage_viewer-0.1/dbt_lineage_viewer.egg-info/
--rw-r--r--   0 yang      (1000) yang      (1000)     1453 2023-05-01 09:07:45.000000 dbt_lineage_viewer-0.1/dbt_lineage_viewer.egg-info/PKG-INFO
--rw-r--r--   0 yang      (1000) yang      (1000)      272 2023-05-01 09:07:45.000000 dbt_lineage_viewer-0.1/dbt_lineage_viewer.egg-info/SOURCES.txt
--rw-r--r--   0 yang      (1000) yang      (1000)        1 2023-05-01 09:07:45.000000 dbt_lineage_viewer-0.1/dbt_lineage_viewer.egg-info/dependency_links.txt
--rw-r--r--   0 yang      (1000) yang      (1000)       49 2023-05-01 09:07:45.000000 dbt_lineage_viewer-0.1/dbt_lineage_viewer.egg-info/entry_points.txt
--rw-r--r--   0 yang      (1000) yang      (1000)        6 2023-05-01 09:07:45.000000 dbt_lineage_viewer-0.1/dbt_lineage_viewer.egg-info/requires.txt
--rw-r--r--   0 yang      (1000) yang      (1000)        1 2023-05-01 09:07:45.000000 dbt_lineage_viewer-0.1/dbt_lineage_viewer.egg-info/top_level.txt
--rw-r--r--   0 yang      (1000) yang      (1000)       38 2023-05-01 09:07:45.230232 dbt_lineage_viewer-0.1/setup.cfg
--rw-r--r--   0 yang      (1000) yang      (1000)      661 2023-05-01 09:07:37.000000 dbt_lineage_viewer-0.1/setup.py
+drwxr-xr-x   0 yang      (1000) yang      (1000)        0 2023-05-01 09:13:59.676679 dbt_lineage_viewer-0.2/
+-rw-r--r--   0 yang      (1000) yang      (1000)     1453 2023-05-01 09:13:59.676679 dbt_lineage_viewer-0.2/PKG-INFO
+-rw-r--r--   0 yang      (1000) yang      (1000)     1211 2023-05-01 08:59:16.000000 dbt_lineage_viewer-0.2/README.md
+drwxr-xr-x   0 yang      (1000) yang      (1000)        0 2023-05-01 09:13:59.676679 dbt_lineage_viewer-0.2/dbt_lineage_viewer.egg-info/
+-rw-r--r--   0 yang      (1000) yang      (1000)     1453 2023-05-01 09:13:59.000000 dbt_lineage_viewer-0.2/dbt_lineage_viewer.egg-info/PKG-INFO
+-rw-r--r--   0 yang      (1000) yang      (1000)      272 2023-05-01 09:13:59.000000 dbt_lineage_viewer-0.2/dbt_lineage_viewer.egg-info/SOURCES.txt
+-rw-r--r--   0 yang      (1000) yang      (1000)        1 2023-05-01 09:13:59.000000 dbt_lineage_viewer-0.2/dbt_lineage_viewer.egg-info/dependency_links.txt
+-rw-r--r--   0 yang      (1000) yang      (1000)       49 2023-05-01 09:13:59.000000 dbt_lineage_viewer-0.2/dbt_lineage_viewer.egg-info/entry_points.txt
+-rw-r--r--   0 yang      (1000) yang      (1000)        6 2023-05-01 09:13:59.000000 dbt_lineage_viewer-0.2/dbt_lineage_viewer.egg-info/requires.txt
+-rw-r--r--   0 yang      (1000) yang      (1000)        1 2023-05-01 09:13:59.000000 dbt_lineage_viewer-0.2/dbt_lineage_viewer.egg-info/top_level.txt
+-rw-r--r--   0 yang      (1000) yang      (1000)       38 2023-05-01 09:13:59.676679 dbt_lineage_viewer-0.2/setup.cfg
+-rw-r--r--   0 yang      (1000) yang      (1000)      661 2023-05-01 09:12:07.000000 dbt_lineage_viewer-0.2/setup.py
```

### Comparing `dbt_lineage_viewer-0.1/PKG-INFO` & `dbt_lineage_viewer-0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt_lineage_viewer
-Version: 0.1
+Version: 0.2
 Summary: A DBT lineage viewer
 Home-page: https://github.com/ydai713/dbt-lineage-viewer
 Author: Yang Dai
 Author-email: yang.dai2020@gmail.com
 Description-Content-Type: text/markdown
 
 # DBT Dependency Viewer
```

### Comparing `dbt_lineage_viewer-0.1/README.md` & `dbt_lineage_viewer-0.2/README.md`

 * *Files identical despite different names*

### Comparing `dbt_lineage_viewer-0.1/dbt_lineage_viewer.egg-info/PKG-INFO` & `dbt_lineage_viewer-0.2/dbt_lineage_viewer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-lineage-viewer
-Version: 0.1
+Version: 0.2
 Summary: A DBT lineage viewer
 Home-page: https://github.com/ydai713/dbt-lineage-viewer
 Author: Yang Dai
 Author-email: yang.dai2020@gmail.com
 Description-Content-Type: text/markdown
 
 # DBT Dependency Viewer
```

### Comparing `dbt_lineage_viewer-0.1/setup.py` & `dbt_lineage_viewer-0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="dbt_lineage_viewer",
-    version="0.1",
+    version="0.2",
     author="Yang Dai",
     author_email="yang.dai2020@gmail.com",
     description="A DBT lineage viewer",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ydai713/dbt-lineage-viewer",
     packages=find_packages(),
```

