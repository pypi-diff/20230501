# Comparing `tmp/xia_scw_template-0.0.2-cp39-none-win_amd64.whl.zip` & `tmp/xia_scw_template-0.0.4-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,12 @@
-Zip file size: 101069 bytes, number of entries: 11
--rw-r--r--  2.0 unx      107 b- defN 23-Apr-30 20:24 xia_scw_template/__init__.py
--rw-r--r--  2.0 unx   236032 b- defN 23-Apr-30 20:26 xia_scw_template/template.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      103 b- defN 23-Apr-30 20:24 xia_scw_template/templates/ScwTemplate/backend.tf
+Zip file size: 100773 bytes, number of entries: 10
+-rw-r--r--  2.0 unx      107 b- defN 23-May-01 05:15 xia_scw_template/__init__.py
+-rw-r--r--  2.0 unx   236032 b- defN 23-May-01 06:22 xia_scw_template/template.cp39-win_amd64.pyd
 -rw-rw-rw-  2.0 unx      414 b- defN 23-Apr-30 20:24 xia_scw_template/templates/ScwTemplate/main.tf
--rw-rw-rw-  2.0 unx       88 b- defN 23-Apr-30 20:24 xia_scw_template/templates/ScwTemplate/output.tf
+-rw-rw-rw-  2.0 unx      124 b- defN 23-May-01 05:15 xia_scw_template/templates/ScwTemplate/output.tf
 -rw-rw-rw-  2.0 unx      136 b- defN 23-Apr-30 20:24 xia_scw_template/templates/ScwTemplate/variables.tf
--rw-rw-rw-  2.0 unx      152 b- defN 23-Apr-30 20:26 xia_scw_template-0.0.2.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      672 b- defN 23-Apr-30 20:26 xia_scw_template-0.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Apr-30 20:26 xia_scw_template-0.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       17 b- defN 23-Apr-30 20:26 xia_scw_template-0.0.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1037 b- defN 23-Apr-30 20:26 xia_scw_template-0.0.2.dist-info/RECORD
-11 files, 238857 bytes uncompressed, 99263 bytes compressed:  58.4%
+-rw-rw-rw-  2.0 unx      152 b- defN 23-May-01 06:22 xia_scw_template-0.0.4.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      698 b- defN 23-May-01 06:22 xia_scw_template-0.0.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-May-01 06:22 xia_scw_template-0.0.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       17 b- defN 23-May-01 06:22 xia_scw_template-0.0.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      933 b- defN 23-May-01 06:22 xia_scw_template-0.0.4.dist-info/RECORD
+10 files, 238712 bytes uncompressed, 99141 bytes compressed:  58.5%
```

## zipnote {}

```diff
@@ -1,34 +1,31 @@
 Filename: xia_scw_template/__init__.py
 Comment: 
 
 Filename: xia_scw_template/template.cp39-win_amd64.pyd
 Comment: 
 
-Filename: xia_scw_template/templates/ScwTemplate/backend.tf
-Comment: 
-
 Filename: xia_scw_template/templates/ScwTemplate/main.tf
 Comment: 
 
 Filename: xia_scw_template/templates/ScwTemplate/output.tf
 Comment: 
 
 Filename: xia_scw_template/templates/ScwTemplate/variables.tf
 Comment: 
 
-Filename: xia_scw_template-0.0.2.dist-info/LICENSE.txt
+Filename: xia_scw_template-0.0.4.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_scw_template-0.0.2.dist-info/METADATA
+Filename: xia_scw_template-0.0.4.dist-info/METADATA
 Comment: 
 
-Filename: xia_scw_template-0.0.2.dist-info/WHEEL
+Filename: xia_scw_template-0.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: xia_scw_template-0.0.2.dist-info/top_level.txt
+Filename: xia_scw_template-0.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_scw_template-0.0.2.dist-info/RECORD
+Filename: xia_scw_template-0.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_scw_template/__init__.py

```diff
@@ -1,8 +1,8 @@
 from xia_scw_template.template import ScwTemplate
 
 
 __all__ = [
     "ScwTemplate"
 ]
 
-__version__ = "0.0.2"
+__version__ = "0.0.4"
```

## xia_scw_template/templates/ScwTemplate/output.tf

```diff
@@ -1,7 +1,11 @@
 output "name" {
   value = var.name
 }
 
 output "description" {
   value = var.description
+}
+
+output "tf_state" {
+  value = ""
 }
```

## Comparing `xia_scw_template-0.0.2.dist-info/METADATA` & `xia_scw_template-0.0.4.dist-info/METADATA`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: xia-scw-template
-Version: 0.0.2
+Version: 0.0.4
 Summary: X-I-A
-Home-page: https://develop.x-i-a.com/docs/xia-scw-template/0.0.2/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-scw-template/0.0.4/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 Requires-Dist: xia-engine-terraform
+Requires-Dist: xia-engine
 
 .. image:: https://img.shields.io/pypi/v/xia-scw-template.svg?color=blue
    :alt: PyPI-Server
    :target: https://pypi.org/project/xia-scw-template/
 
 ====================================
 X-I-A
```

## Comparing `xia_scw_template-0.0.2.dist-info/RECORD` & `xia_scw_template-0.0.4.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-xia_scw_template/__init__.py,sha256=O03FiJ1FnOSSupNBZMHPHBQbbbhPMCFBnUaUwwJHJRY,107
-xia_scw_template/template.cp39-win_amd64.pyd,sha256=o0NVWdnhQ0z8R9nG7hCJoh3HlBOmdSam4ggTaTwjRUE,236032
-xia_scw_template/templates/ScwTemplate/backend.tf,sha256=bbBhWpPkAyaZDrgmjRWClB3kEffcP-qaiC2vlXXlAKY,103
+xia_scw_template/__init__.py,sha256=tmPmPL3cUvog_LwiX_pLoNJEVFY244P4UUJeL7eDnM4,107
+xia_scw_template/template.cp39-win_amd64.pyd,sha256=uzXLSWSzBk9kaafZ7uxPs_eTg-Jt3K98oK0pki-3lcw,236032
 xia_scw_template/templates/ScwTemplate/main.tf,sha256=USKe9YPVicChcPSxUbZP_-f-kcFqLY4Ssi3zkPkHS8Q,414
-xia_scw_template/templates/ScwTemplate/output.tf,sha256=1KMXhU7r9bqIjg7VEHcajCLA-ZSvh12mqYzXsK2Jaqs,88
+xia_scw_template/templates/ScwTemplate/output.tf,sha256=DfWBNaXPS42F-qEgemsPOWdtPMiqaUN-1ekPd_h7nyc,124
 xia_scw_template/templates/ScwTemplate/variables.tf,sha256=aR-VP5gMS05TmxMvdMAIuKoGmfNULd0cBGUqelhyCv8,136
-xia_scw_template-0.0.2.dist-info/LICENSE.txt,sha256=t7dcmwWYpCopxtSO2xM5htr8WC8xUXgTax2q0dOA-Ak,152
-xia_scw_template-0.0.2.dist-info/METADATA,sha256=0xLOk5QO_uxqnsGLqurZ8NEK59_ikM2WXpF5IG8n7Yo,672
-xia_scw_template-0.0.2.dist-info/WHEEL,sha256=T8VPDjot1YI5-NaRzS6kIMlJNVl0SSGa_dm-8Fprszg,99
-xia_scw_template-0.0.2.dist-info/top_level.txt,sha256=PnzNPYJvb9BCFS0nMLHk3DDKw5vJjkdhUg0gD_vL_cU,17
-xia_scw_template-0.0.2.dist-info/RECORD,,
+xia_scw_template-0.0.4.dist-info/LICENSE.txt,sha256=t7dcmwWYpCopxtSO2xM5htr8WC8xUXgTax2q0dOA-Ak,152
+xia_scw_template-0.0.4.dist-info/METADATA,sha256=M0iL1hfqariA86gmpN1ptCaGb2aspJ2oOdWI18wtTLY,698
+xia_scw_template-0.0.4.dist-info/WHEEL,sha256=T8VPDjot1YI5-NaRzS6kIMlJNVl0SSGa_dm-8Fprszg,99
+xia_scw_template-0.0.4.dist-info/top_level.txt,sha256=PnzNPYJvb9BCFS0nMLHk3DDKw5vJjkdhUg0gD_vL_cU,17
+xia_scw_template-0.0.4.dist-info/RECORD,,
```

