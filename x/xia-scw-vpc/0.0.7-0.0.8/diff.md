# Comparing `tmp/xia_scw_vpc-0.0.7-cp39-none-win_amd64.whl.zip` & `tmp/xia_scw_vpc-0.0.8-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 110373 bytes, number of entries: 12
--rw-r--r--  2.0 unx       87 b- defN 23-Apr-30 07:48 xia_scw_vpc/__init__.py
--rw-r--r--  2.0 unx   259072 b- defN 23-Apr-30 08:01 xia_scw_vpc/vpc.cp39-win_amd64.pyd
+Zip file size: 110355 bytes, number of entries: 12
+-rw-r--r--  2.0 unx       87 b- defN 23-May-01 05:24 xia_scw_vpc/__init__.py
+-rw-r--r--  2.0 unx   259072 b- defN 23-May-01 05:32 xia_scw_vpc/vpc.cp39-win_amd64.pyd
 -rw-rw-rw-  2.0 unx       69 b- defN 23-Apr-21 13:39 xia_scw_vpc/templates/ScwVpc/backend.tf
 -rw-rw-rw-  2.0 unx      991 b- defN 23-Apr-21 16:00 xia_scw_vpc/templates/ScwVpc/main.tf
 -rw-rw-rw-  2.0 unx      651 b- defN 23-Apr-21 16:00 xia_scw_vpc/templates/ScwVpc/output.tf
 -rw-rw-rw-  2.0 unx      343 b- defN 23-Apr-21 13:39 xia_scw_vpc/templates/ScwVpc/provider.tf
 -rw-rw-rw-  2.0 unx     1953 b- defN 23-Apr-21 16:00 xia_scw_vpc/templates/ScwVpc/variables.tf
--rw-rw-rw-  2.0 unx      152 b- defN 23-Apr-30 08:01 xia_scw_vpc-0.0.7.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      652 b- defN 23-Apr-30 08:01 xia_scw_vpc-0.0.7.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Apr-30 08:01 xia_scw_vpc-0.0.7.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 23-Apr-30 08:01 xia_scw_vpc-0.0.7.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1053 b- defN 23-Apr-30 08:01 xia_scw_vpc-0.0.7.dist-info/RECORD
-12 files, 265134 bytes uncompressed, 108571 bytes compressed:  59.1%
+-rw-rw-rw-  2.0 unx      152 b- defN 23-May-01 05:32 xia_scw_vpc-0.0.8.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      652 b- defN 23-May-01 05:32 xia_scw_vpc-0.0.8.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-May-01 05:32 xia_scw_vpc-0.0.8.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 23-May-01 05:32 xia_scw_vpc-0.0.8.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1053 b- defN 23-May-01 05:32 xia_scw_vpc-0.0.8.dist-info/RECORD
+12 files, 265134 bytes uncompressed, 108553 bytes compressed:  59.1%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: xia_scw_vpc/templates/ScwVpc/provider.tf
 Comment: 
 
 Filename: xia_scw_vpc/templates/ScwVpc/variables.tf
 Comment: 
 
-Filename: xia_scw_vpc-0.0.7.dist-info/LICENSE.txt
+Filename: xia_scw_vpc-0.0.8.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_scw_vpc-0.0.7.dist-info/METADATA
+Filename: xia_scw_vpc-0.0.8.dist-info/METADATA
 Comment: 
 
-Filename: xia_scw_vpc-0.0.7.dist-info/WHEEL
+Filename: xia_scw_vpc-0.0.8.dist-info/WHEEL
 Comment: 
 
-Filename: xia_scw_vpc-0.0.7.dist-info/top_level.txt
+Filename: xia_scw_vpc-0.0.8.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_scw_vpc-0.0.7.dist-info/RECORD
+Filename: xia_scw_vpc-0.0.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_scw_vpc/__init__.py

```diff
@@ -1,8 +1,8 @@
 from xia_scw_vpc.vpc import ScwVpc
 
 
 __all__ = [
     "ScwVpc"
 ]
 
-__version__ = "0.0.7"
+__version__ = "0.0.8"
```

## Comparing `xia_scw_vpc-0.0.7.dist-info/METADATA` & `xia_scw_vpc-0.0.8.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: xia-scw-vpc
-Version: 0.0.7
+Version: 0.0.8
 Summary: X-I-A
-Home-page: https://develop.x-i-a.com/docs/xia-scw-vpc/0.0.7/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-scw-vpc/0.0.8/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
```

## Comparing `xia_scw_vpc-0.0.7.dist-info/RECORD` & `xia_scw_vpc-0.0.8.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-xia_scw_vpc/__init__.py,sha256=boeEMYTETOFJKibgW9Czixkd19lB_rf86Bs9XwgLBe4,87
-xia_scw_vpc/vpc.cp39-win_amd64.pyd,sha256=grQTo4COCRX3pZ-hEPg-MgDADCr9gzgzbD126dLqY-g,259072
+xia_scw_vpc/__init__.py,sha256=9rzF0up0QQQ6xzpBoYJNteN9p79ZHV_lNqI1vp5wFCU,87
+xia_scw_vpc/vpc.cp39-win_amd64.pyd,sha256=w_9w79_1Krfj8ia55ADl4iMPCMYYSFBukITblu3jAJo,259072
 xia_scw_vpc/templates/ScwVpc/backend.tf,sha256=E6fgAX-nMcTt9oErRKvK67uJPdB-O77YJpzAvf06zgs,69
 xia_scw_vpc/templates/ScwVpc/main.tf,sha256=UElrNqO31xqjS1yD5wEbdVb4kNxodZXW8d7n6W2_W5A,991
 xia_scw_vpc/templates/ScwVpc/output.tf,sha256=kx1Qbfc6mWyIN8_N1D1E9s30LiyIOgx3hW7z5R2-mYY,651
 xia_scw_vpc/templates/ScwVpc/provider.tf,sha256=h_zFGas7QtYJPGvufLGuPHtgDhoZa28Qa5t--1dpheI,343
 xia_scw_vpc/templates/ScwVpc/variables.tf,sha256=rrE9u584cXmGb9V79rOsyZxWH2yx9N7f3ode2XjHfxE,1953
-xia_scw_vpc-0.0.7.dist-info/LICENSE.txt,sha256=CgeJ1rTURAK7GLPD_GW3lyXH8ZFFrBDM0ekl9JHZR2s,152
-xia_scw_vpc-0.0.7.dist-info/METADATA,sha256=s-u2ZuWxUUsyshO8OS2CKoHTkzFmqVCeehqhbEvmVO0,652
-xia_scw_vpc-0.0.7.dist-info/WHEEL,sha256=T8VPDjot1YI5-NaRzS6kIMlJNVl0SSGa_dm-8Fprszg,99
-xia_scw_vpc-0.0.7.dist-info/top_level.txt,sha256=jNt0Wv07qq3bYLKNdao2gLQ4e_U6VYrOuw3Wehup0ts,12
-xia_scw_vpc-0.0.7.dist-info/RECORD,,
+xia_scw_vpc-0.0.8.dist-info/LICENSE.txt,sha256=t7dcmwWYpCopxtSO2xM5htr8WC8xUXgTax2q0dOA-Ak,152
+xia_scw_vpc-0.0.8.dist-info/METADATA,sha256=gPYrraISe48kyzQ-4-iOS8XP1HM0kjtfexqG9YMojx8,652
+xia_scw_vpc-0.0.8.dist-info/WHEEL,sha256=T8VPDjot1YI5-NaRzS6kIMlJNVl0SSGa_dm-8Fprszg,99
+xia_scw_vpc-0.0.8.dist-info/top_level.txt,sha256=jNt0Wv07qq3bYLKNdao2gLQ4e_U6VYrOuw3Wehup0ts,12
+xia_scw_vpc-0.0.8.dist-info/RECORD,,
```

