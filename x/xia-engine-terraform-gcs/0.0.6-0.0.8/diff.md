# Comparing `tmp/xia_engine_terraform_gcs-0.0.6-cp39-none-win_amd64.whl.zip` & `tmp/xia_engine_terraform_gcs-0.0.8-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 125715 bytes, number of entries: 7
--rw-r--r--  2.0 unx      378 b- defN 23-Apr-30 16:38 xia_engine_terraform_gcs/__init__.py
--rw-r--r--  2.0 unx   298496 b- defN 23-Apr-30 16:41 xia_engine_terraform_gcs/engine.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      152 b- defN 23-Apr-30 16:41 xia_engine_terraform_gcs-0.0.6.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      726 b- defN 23-Apr-30 16:41 xia_engine_terraform_gcs-0.0.6.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Apr-30 16:41 xia_engine_terraform_gcs-0.0.6.dist-info/WHEEL
--rw-r--r--  2.0 unx       25 b- defN 23-Apr-30 16:41 xia_engine_terraform_gcs-0.0.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      674 b- defN 23-Apr-30 16:41 xia_engine_terraform_gcs-0.0.6.dist-info/RECORD
-7 files, 300550 bytes uncompressed, 124493 bytes compressed:  58.6%
+Zip file size: 125919 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      378 b- defN 23-May-01 08:46 xia_engine_terraform_gcs/__init__.py
+-rw-r--r--  2.0 unx   299008 b- defN 23-May-01 08:48 xia_engine_terraform_gcs/engine.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 unx      152 b- defN 23-May-01 08:48 xia_engine_terraform_gcs-0.0.8.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      762 b- defN 23-May-01 08:48 xia_engine_terraform_gcs-0.0.8.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-May-01 08:48 xia_engine_terraform_gcs-0.0.8.dist-info/WHEEL
+-rw-r--r--  2.0 unx       25 b- defN 23-May-01 08:48 xia_engine_terraform_gcs-0.0.8.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      674 b- defN 23-May-01 08:48 xia_engine_terraform_gcs-0.0.8.dist-info/RECORD
+7 files, 301098 bytes uncompressed, 124697 bytes compressed:  58.6%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_engine_terraform_gcs/__init__.py
 Comment: 
 
 Filename: xia_engine_terraform_gcs/engine.cp39-win_amd64.pyd
 Comment: 
 
-Filename: xia_engine_terraform_gcs-0.0.6.dist-info/LICENSE.txt
+Filename: xia_engine_terraform_gcs-0.0.8.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_engine_terraform_gcs-0.0.6.dist-info/METADATA
+Filename: xia_engine_terraform_gcs-0.0.8.dist-info/METADATA
 Comment: 
 
-Filename: xia_engine_terraform_gcs-0.0.6.dist-info/WHEEL
+Filename: xia_engine_terraform_gcs-0.0.8.dist-info/WHEEL
 Comment: 
 
-Filename: xia_engine_terraform_gcs-0.0.6.dist-info/top_level.txt
+Filename: xia_engine_terraform_gcs-0.0.8.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_engine_terraform_gcs-0.0.6.dist-info/RECORD
+Filename: xia_engine_terraform_gcs-0.0.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_engine_terraform_gcs/__init__.py

```diff
@@ -3,8 +3,8 @@
 
 
 __all__ = [
     "TerraformGcsEngine", "TerraformGcsConnectParam", "TerraformGcsClient",
     "ScwTerraformGcsEngine", "ScwTerraformGcsConnectParam"
 ]
 
-__version__ = "0.0.6"
+__version__ = "0.0.8"
```

## Comparing `xia_engine_terraform_gcs-0.0.6.dist-info/METADATA` & `xia_engine_terraform_gcs-0.0.8.dist-info/METADATA`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: xia-engine-terraform-gcs
-Version: 0.0.6
+Version: 0.0.8
 Summary: X-I-A
-Home-page: https://develop.x-i-a.com/docs/xia-engine-terraform-gcs/0.0.6/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-engine-terraform-gcs/0.0.8/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 Requires-Dist: jinja2
+Requires-Dist: google-cloud-storage
 Requires-Dist: xia-engine-terraform
 
 .. image:: https://img.shields.io/pypi/v/xia-engine-terraform-gcs.svg?color=blue
    :alt: PyPI-Server
    :target: https://pypi.org/project/xia-engine-terraform-gcs/
 
 ====================================
```

