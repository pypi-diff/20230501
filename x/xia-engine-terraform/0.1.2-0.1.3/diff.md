# Comparing `tmp/xia_engine_terraform-0.1.2-cp39-none-win_amd64.whl.zip` & `tmp/xia_engine_terraform-0.1.3-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 216463 bytes, number of entries: 7
--rw-r--r--  2.0 unx      645 b- defN 23-May-01 06:12 xia_engine_terraform/__init__.py
--rw-r--r--  2.0 unx   579584 b- defN 23-May-01 06:15 xia_engine_terraform/engine.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      152 b- defN 23-May-01 06:15 xia_engine_terraform-0.1.2.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      736 b- defN 23-May-01 06:15 xia_engine_terraform-0.1.2.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-May-01 06:15 xia_engine_terraform-0.1.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       21 b- defN 23-May-01 06:15 xia_engine_terraform-0.1.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      646 b- defN 23-May-01 06:15 xia_engine_terraform-0.1.2.dist-info/RECORD
-7 files, 581883 bytes uncompressed, 215297 bytes compressed:  63.0%
+Zip file size: 222644 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      645 b- defN 23-May-01 07:29 xia_engine_terraform/__init__.py
+-rw-r--r--  2.0 unx   600576 b- defN 23-May-01 07:32 xia_engine_terraform/engine.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 unx      152 b- defN 23-May-01 07:33 xia_engine_terraform-0.1.3.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      724 b- defN 23-May-01 07:33 xia_engine_terraform-0.1.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-May-01 07:33 xia_engine_terraform-0.1.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       21 b- defN 23-May-01 07:33 xia_engine_terraform-0.1.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      646 b- defN 23-May-01 07:33 xia_engine_terraform-0.1.3.dist-info/RECORD
+7 files, 602863 bytes uncompressed, 221478 bytes compressed:  63.3%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_engine_terraform/__init__.py
 Comment: 
 
 Filename: xia_engine_terraform/engine.cp39-win_amd64.pyd
 Comment: 
 
-Filename: xia_engine_terraform-0.1.2.dist-info/LICENSE.txt
+Filename: xia_engine_terraform-0.1.3.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_engine_terraform-0.1.2.dist-info/METADATA
+Filename: xia_engine_terraform-0.1.3.dist-info/METADATA
 Comment: 
 
-Filename: xia_engine_terraform-0.1.2.dist-info/WHEEL
+Filename: xia_engine_terraform-0.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: xia_engine_terraform-0.1.2.dist-info/top_level.txt
+Filename: xia_engine_terraform-0.1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_engine_terraform-0.1.2.dist-info/RECORD
+Filename: xia_engine_terraform-0.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_engine_terraform/__init__.py

```diff
@@ -6,8 +6,8 @@
 __all__ = [
     "TerraformEngine", "TerraformConnectParam", "TerraformClient",
     "TerraformLocalEngine", "TerraformLocalConnectParam", "TerraformLocalClient",
     "ScwTerraformLocalEngine", "ScwTerraformLocalConnectParam",
     "TerraformConfigFactory"
 ]
 
-__version__ = "0.1.2"
+__version__ = "0.1.3"
```

## Comparing `xia_engine_terraform-0.1.2.dist-info/METADATA` & `xia_engine_terraform-0.1.3.dist-info/METADATA`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: xia-engine-terraform
-Version: 0.1.2
+Version: 0.1.3
 Summary: X-I-A
-Home-page: https://develop.x-i-a.com/docs/xia-engine-terraform/0.1.2/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-engine-terraform/0.1.3/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 Requires-Dist: jinja2
-Requires-Dist: google-cloud-storage
+Requires-Dist: requests
 Requires-Dist: xia-engine
 
 .. image:: https://img.shields.io/pypi/v/xia-engine-terraform.svg?color=blue
    :alt: PyPI-Server
    :target: https://pypi.org/project/xia-engine-terraform/
 
 ====================================
```

