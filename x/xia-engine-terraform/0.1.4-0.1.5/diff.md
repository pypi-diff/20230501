# Comparing `tmp/xia_engine_terraform-0.1.4-cp39-none-win_amd64.whl.zip` & `tmp/xia_engine_terraform-0.1.5-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 221572 bytes, number of entries: 7
--rw-r--r--  2.0 unx      645 b- defN 23-May-01 07:43 xia_engine_terraform/__init__.py
--rw-r--r--  2.0 unx   596992 b- defN 23-May-01 07:46 xia_engine_terraform/engine.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      152 b- defN 23-May-01 07:46 xia_engine_terraform-0.1.4.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      724 b- defN 23-May-01 07:46 xia_engine_terraform-0.1.4.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-May-01 07:46 xia_engine_terraform-0.1.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       21 b- defN 23-May-01 07:46 xia_engine_terraform-0.1.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      646 b- defN 23-May-01 07:46 xia_engine_terraform-0.1.4.dist-info/RECORD
-7 files, 599279 bytes uncompressed, 220406 bytes compressed:  63.2%
+Zip file size: 221578 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      645 b- defN 23-May-01 07:49 xia_engine_terraform/__init__.py
+-rw-r--r--  2.0 unx   596992 b- defN 23-May-01 07:52 xia_engine_terraform/engine.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 unx      152 b- defN 23-May-01 07:52 xia_engine_terraform-0.1.5.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      724 b- defN 23-May-01 07:52 xia_engine_terraform-0.1.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-May-01 07:52 xia_engine_terraform-0.1.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       21 b- defN 23-May-01 07:52 xia_engine_terraform-0.1.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      646 b- defN 23-May-01 07:52 xia_engine_terraform-0.1.5.dist-info/RECORD
+7 files, 599279 bytes uncompressed, 220412 bytes compressed:  63.2%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_engine_terraform/__init__.py
 Comment: 
 
 Filename: xia_engine_terraform/engine.cp39-win_amd64.pyd
 Comment: 
 
-Filename: xia_engine_terraform-0.1.4.dist-info/LICENSE.txt
+Filename: xia_engine_terraform-0.1.5.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_engine_terraform-0.1.4.dist-info/METADATA
+Filename: xia_engine_terraform-0.1.5.dist-info/METADATA
 Comment: 
 
-Filename: xia_engine_terraform-0.1.4.dist-info/WHEEL
+Filename: xia_engine_terraform-0.1.5.dist-info/WHEEL
 Comment: 
 
-Filename: xia_engine_terraform-0.1.4.dist-info/top_level.txt
+Filename: xia_engine_terraform-0.1.5.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_engine_terraform-0.1.4.dist-info/RECORD
+Filename: xia_engine_terraform-0.1.5.dist-info/RECORD
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
 
-__version__ = "0.1.4"
+__version__ = "0.1.5"
```

## Comparing `xia_engine_terraform-0.1.4.dist-info/METADATA` & `xia_engine_terraform-0.1.5.dist-info/METADATA`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: xia-engine-terraform
-Version: 0.1.4
+Version: 0.1.5
 Summary: X-I-A
-Home-page: https://develop.x-i-a.com/docs/xia-engine-terraform/0.1.4/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-engine-terraform/0.1.5/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
```

## Comparing `xia_engine_terraform-0.1.4.dist-info/RECORD` & `xia_engine_terraform-0.1.5.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-xia_engine_terraform/__init__.py,sha256=oKA7-Eb2h1SYZ2Q7eNswv0UavugHow8BYMHOQWt_8rk,645
-xia_engine_terraform/engine.cp39-win_amd64.pyd,sha256=DmDteMz9CwnECqkRLv_AnNl_SkMiuJmLi3eXcFzHSiA,596992
-xia_engine_terraform-0.1.4.dist-info/LICENSE.txt,sha256=30wWxpufZqbxK7WdwZRoX8iA_veQA4gbl5oih3j5vFs,152
-xia_engine_terraform-0.1.4.dist-info/METADATA,sha256=8gX3c1KtajxYSO-lkkRwD8SCFeLoq7k15QO0QAViEZI,724
-xia_engine_terraform-0.1.4.dist-info/WHEEL,sha256=T8VPDjot1YI5-NaRzS6kIMlJNVl0SSGa_dm-8Fprszg,99
-xia_engine_terraform-0.1.4.dist-info/top_level.txt,sha256=9T86e-QQo91fnAOB3rD5xeM_4EPL7Edk_oOlmR_xquQ,21
-xia_engine_terraform-0.1.4.dist-info/RECORD,,
+xia_engine_terraform/__init__.py,sha256=Jg5B_IfCNk8QqXY2zq3fyjdfKAF9lta7H6GpH0hzDzw,645
+xia_engine_terraform/engine.cp39-win_amd64.pyd,sha256=q9RsUrp8vPp-C2PjelfPZxHVvOdsEFqwjiqJt5iFKHA,596992
+xia_engine_terraform-0.1.5.dist-info/LICENSE.txt,sha256=30wWxpufZqbxK7WdwZRoX8iA_veQA4gbl5oih3j5vFs,152
+xia_engine_terraform-0.1.5.dist-info/METADATA,sha256=g16kqkj0vAJBuj-axo6PNDCbrB_C6nN4S88PXEFVeSk,724
+xia_engine_terraform-0.1.5.dist-info/WHEEL,sha256=T8VPDjot1YI5-NaRzS6kIMlJNVl0SSGa_dm-8Fprszg,99
+xia_engine_terraform-0.1.5.dist-info/top_level.txt,sha256=9T86e-QQo91fnAOB3rD5xeM_4EPL7Edk_oOlmR_xquQ,21
+xia_engine_terraform-0.1.5.dist-info/RECORD,,
```

