# Comparing `tmp/xia_engine_terraform-0.1.5-cp39-none-win_amd64.whl.zip` & `tmp/xia_engine_terraform-0.1.6-cp39-none-macosx_11_0_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 221578 bytes, number of entries: 7
--rw-r--r--  2.0 unx      645 b- defN 23-May-01 07:49 xia_engine_terraform/__init__.py
--rw-r--r--  2.0 unx   596992 b- defN 23-May-01 07:52 xia_engine_terraform/engine.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      152 b- defN 23-May-01 07:52 xia_engine_terraform-0.1.5.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      724 b- defN 23-May-01 07:52 xia_engine_terraform-0.1.5.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-May-01 07:52 xia_engine_terraform-0.1.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       21 b- defN 23-May-01 07:52 xia_engine_terraform-0.1.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      646 b- defN 23-May-01 07:52 xia_engine_terraform-0.1.5.dist-info/RECORD
-7 files, 599279 bytes uncompressed, 220412 bytes compressed:  63.2%
+Zip file size: 186282 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      645 b- defN 23-May-01 11:23 xia_engine_terraform/__init__.py
+-rw-r--r--  2.0 unx   525816 b- defN 23-May-01 11:24 xia_engine_terraform/engine.cpython-310-darwin.so
+-rw-r--r--  2.0 unx      152 b- defN 23-May-01 11:24 xia_engine_terraform-0.1.6.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      687 b- defN 23-May-01 11:24 xia_engine_terraform-0.1.6.dist-info/METADATA
+-rw-r--r--  2.0 unx      108 b- defN 23-May-01 11:24 xia_engine_terraform-0.1.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       21 b- defN 23-May-01 11:24 xia_engine_terraform-0.1.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      650 b- defN 23-May-01 11:24 xia_engine_terraform-0.1.6.dist-info/RECORD
+7 files, 528079 bytes uncompressed, 185110 bytes compressed:  64.9%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_engine_terraform/__init__.py
 Comment: 
 
-Filename: xia_engine_terraform/engine.cp39-win_amd64.pyd
+Filename: xia_engine_terraform/engine.cpython-310-darwin.so
 Comment: 
 
-Filename: xia_engine_terraform-0.1.5.dist-info/LICENSE.txt
+Filename: xia_engine_terraform-0.1.6.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_engine_terraform-0.1.5.dist-info/METADATA
+Filename: xia_engine_terraform-0.1.6.dist-info/METADATA
 Comment: 
 
-Filename: xia_engine_terraform-0.1.5.dist-info/WHEEL
+Filename: xia_engine_terraform-0.1.6.dist-info/WHEEL
 Comment: 
 
-Filename: xia_engine_terraform-0.1.5.dist-info/top_level.txt
+Filename: xia_engine_terraform-0.1.6.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_engine_terraform-0.1.5.dist-info/RECORD
+Filename: xia_engine_terraform-0.1.6.dist-info/RECORD
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
 
-__version__ = "0.1.5"
+__version__ = "0.1.6"
```

## Comparing `xia_engine_terraform-0.1.5.dist-info/METADATA` & `xia_engine_terraform-0.1.6.dist-info/METADATA`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: xia-engine-terraform
-Version: 0.1.5
+Version: 0.1.6
 Summary: X-I-A
-Home-page: https://develop.x-i-a.com/docs/xia-engine-terraform/0.1.5/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-engine-terraform/0.1.6/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
-License: UNKNOWN
-Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 Requires-Dist: jinja2
 Requires-Dist: requests
 Requires-Dist: xia-engine
 
@@ -28,9 +26,7 @@
 =============================
 
 Install the package::
 
     pip install
 
 
-
-
```

