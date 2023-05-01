# Comparing `tmp/xia_engine_terraform-0.1.0-cp39-none-win_amd64.whl.zip` & `tmp/xia_engine_terraform-0.1.1-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 214357 bytes, number of entries: 7
--rw-r--r--  2.0 unx      645 b- defN 23-Apr-30 19:41 xia_engine_terraform/__init__.py
--rw-r--r--  2.0 unx   572928 b- defN 23-Apr-30 19:44 xia_engine_terraform/engine.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      152 b- defN 23-Apr-30 19:44 xia_engine_terraform-0.1.0.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      736 b- defN 23-Apr-30 19:44 xia_engine_terraform-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Apr-30 19:44 xia_engine_terraform-0.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       21 b- defN 23-Apr-30 19:44 xia_engine_terraform-0.1.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      646 b- defN 23-Apr-30 19:44 xia_engine_terraform-0.1.0.dist-info/RECORD
-7 files, 575227 bytes uncompressed, 213191 bytes compressed:  62.9%
+Zip file size: 216504 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      645 b- defN 23-May-01 05:51 xia_engine_terraform/__init__.py
+-rw-r--r--  2.0 unx   579584 b- defN 23-May-01 05:54 xia_engine_terraform/engine.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 unx      152 b- defN 23-May-01 05:54 xia_engine_terraform-0.1.1.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      736 b- defN 23-May-01 05:54 xia_engine_terraform-0.1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-May-01 05:54 xia_engine_terraform-0.1.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       21 b- defN 23-May-01 05:54 xia_engine_terraform-0.1.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      646 b- defN 23-May-01 05:54 xia_engine_terraform-0.1.1.dist-info/RECORD
+7 files, 581883 bytes uncompressed, 215338 bytes compressed:  63.0%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_engine_terraform/__init__.py
 Comment: 
 
 Filename: xia_engine_terraform/engine.cp39-win_amd64.pyd
 Comment: 
 
-Filename: xia_engine_terraform-0.1.0.dist-info/LICENSE.txt
+Filename: xia_engine_terraform-0.1.1.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_engine_terraform-0.1.0.dist-info/METADATA
+Filename: xia_engine_terraform-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: xia_engine_terraform-0.1.0.dist-info/WHEEL
+Filename: xia_engine_terraform-0.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: xia_engine_terraform-0.1.0.dist-info/top_level.txt
+Filename: xia_engine_terraform-0.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_engine_terraform-0.1.0.dist-info/RECORD
+Filename: xia_engine_terraform-0.1.1.dist-info/RECORD
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
 
-__version__ = "0.1.0"
+__version__ = "0.1.1"
```

## Comparing `xia_engine_terraform-0.1.0.dist-info/METADATA` & `xia_engine_terraform-0.1.1.dist-info/METADATA`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: xia-engine-terraform
-Version: 0.1.0
+Version: 0.1.1
 Summary: X-I-A
-Home-page: https://develop.x-i-a.com/docs/xia-engine-terraform/0.1.0/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-engine-terraform/0.1.1/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
```

## Comparing `xia_engine_terraform-0.1.0.dist-info/RECORD` & `xia_engine_terraform-0.1.1.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-xia_engine_terraform/__init__.py,sha256=p20r0Sn0lU61SWOkdOTqDqEDlF3WzBW5iGnCU5Zlzbc,645
-xia_engine_terraform/engine.cp39-win_amd64.pyd,sha256=W5h7mwwuFtou_PiyxQ9cLhRYrwsHEwUm2ARcnEUNDOY,572928
-xia_engine_terraform-0.1.0.dist-info/LICENSE.txt,sha256=30wWxpufZqbxK7WdwZRoX8iA_veQA4gbl5oih3j5vFs,152
-xia_engine_terraform-0.1.0.dist-info/METADATA,sha256=csgBqOZvqGBEk1z_68gojS6D-DBgF_kkR943ubKOoyw,736
-xia_engine_terraform-0.1.0.dist-info/WHEEL,sha256=T8VPDjot1YI5-NaRzS6kIMlJNVl0SSGa_dm-8Fprszg,99
-xia_engine_terraform-0.1.0.dist-info/top_level.txt,sha256=9T86e-QQo91fnAOB3rD5xeM_4EPL7Edk_oOlmR_xquQ,21
-xia_engine_terraform-0.1.0.dist-info/RECORD,,
+xia_engine_terraform/__init__.py,sha256=cCFrvLfQ9pXtUh6k1_di6TQHGCSCZCmQ10gveyraz40,645
+xia_engine_terraform/engine.cp39-win_amd64.pyd,sha256=m3xmQKH2ftjm4gqryIL3RN2Ktd-e5iiseLZJbG2LAHs,579584
+xia_engine_terraform-0.1.1.dist-info/LICENSE.txt,sha256=30wWxpufZqbxK7WdwZRoX8iA_veQA4gbl5oih3j5vFs,152
+xia_engine_terraform-0.1.1.dist-info/METADATA,sha256=IYqNyG-K6EmzorYFr9KkKBpeVXTw-OeDE2q9oHgOMdw,736
+xia_engine_terraform-0.1.1.dist-info/WHEEL,sha256=T8VPDjot1YI5-NaRzS6kIMlJNVl0SSGa_dm-8Fprszg,99
+xia_engine_terraform-0.1.1.dist-info/top_level.txt,sha256=9T86e-QQo91fnAOB3rD5xeM_4EPL7Edk_oOlmR_xquQ,21
+xia_engine_terraform-0.1.1.dist-info/RECORD,,
```

