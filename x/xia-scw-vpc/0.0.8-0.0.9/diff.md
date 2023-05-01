# Comparing `tmp/xia_scw_vpc-0.0.8-cp39-none-win_amd64.whl.zip` & `tmp/xia_scw_vpc-0.0.9-cp39-none-macosx_11_0_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 110355 bytes, number of entries: 12
--rw-r--r--  2.0 unx       87 b- defN 23-May-01 05:24 xia_scw_vpc/__init__.py
--rw-r--r--  2.0 unx   259072 b- defN 23-May-01 05:32 xia_scw_vpc/vpc.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx       69 b- defN 23-Apr-21 13:39 xia_scw_vpc/templates/ScwVpc/backend.tf
--rw-rw-rw-  2.0 unx      991 b- defN 23-Apr-21 16:00 xia_scw_vpc/templates/ScwVpc/main.tf
--rw-rw-rw-  2.0 unx      651 b- defN 23-Apr-21 16:00 xia_scw_vpc/templates/ScwVpc/output.tf
--rw-rw-rw-  2.0 unx      343 b- defN 23-Apr-21 13:39 xia_scw_vpc/templates/ScwVpc/provider.tf
--rw-rw-rw-  2.0 unx     1953 b- defN 23-Apr-21 16:00 xia_scw_vpc/templates/ScwVpc/variables.tf
--rw-rw-rw-  2.0 unx      152 b- defN 23-May-01 05:32 xia_scw_vpc-0.0.8.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      652 b- defN 23-May-01 05:32 xia_scw_vpc-0.0.8.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-May-01 05:32 xia_scw_vpc-0.0.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 23-May-01 05:32 xia_scw_vpc-0.0.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1053 b- defN 23-May-01 05:32 xia_scw_vpc-0.0.8.dist-info/RECORD
-12 files, 265134 bytes uncompressed, 108553 bytes compressed:  59.1%
+Zip file size: 87745 bytes, number of entries: 12
+-rw-r--r--  2.0 unx       87 b- defN 23-May-01 09:15 xia_scw_vpc/__init__.py
+-rw-r--r--  2.0 unx   235400 b- defN 23-May-01 09:15 xia_scw_vpc/vpc.cpython-310-darwin.so
+-rw-r--r--  2.0 unx       69 b- defN 23-Apr-21 16:02 xia_scw_vpc/templates/ScwVpc/backend.tf
+-rw-r--r--  2.0 unx      991 b- defN 23-Apr-21 16:02 xia_scw_vpc/templates/ScwVpc/main.tf
+-rw-r--r--  2.0 unx      651 b- defN 23-Apr-21 16:02 xia_scw_vpc/templates/ScwVpc/output.tf
+-rw-r--r--  2.0 unx      343 b- defN 23-Apr-21 16:02 xia_scw_vpc/templates/ScwVpc/provider.tf
+-rw-r--r--  2.0 unx     1953 b- defN 23-Apr-21 16:02 xia_scw_vpc/templates/ScwVpc/variables.tf
+-rw-r--r--  2.0 unx      152 b- defN 23-May-01 09:15 xia_scw_vpc-0.0.9.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      605 b- defN 23-May-01 09:15 xia_scw_vpc-0.0.9.dist-info/METADATA
+-rw-r--r--  2.0 unx      108 b- defN 23-May-01 09:15 xia_scw_vpc-0.0.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 23-May-01 09:15 xia_scw_vpc-0.0.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1057 b- defN 23-May-01 09:15 xia_scw_vpc-0.0.9.dist-info/RECORD
+12 files, 241428 bytes uncompressed, 85937 bytes compressed:  64.4%
```

## zipnote {}

```diff
@@ -1,11 +1,11 @@
 Filename: xia_scw_vpc/__init__.py
 Comment: 
 
-Filename: xia_scw_vpc/vpc.cp39-win_amd64.pyd
+Filename: xia_scw_vpc/vpc.cpython-310-darwin.so
 Comment: 
 
 Filename: xia_scw_vpc/templates/ScwVpc/backend.tf
 Comment: 
 
 Filename: xia_scw_vpc/templates/ScwVpc/main.tf
 Comment: 
@@ -15,23 +15,23 @@
 
 Filename: xia_scw_vpc/templates/ScwVpc/provider.tf
 Comment: 
 
 Filename: xia_scw_vpc/templates/ScwVpc/variables.tf
 Comment: 
 
-Filename: xia_scw_vpc-0.0.8.dist-info/LICENSE.txt
+Filename: xia_scw_vpc-0.0.9.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_scw_vpc-0.0.8.dist-info/METADATA
+Filename: xia_scw_vpc-0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: xia_scw_vpc-0.0.8.dist-info/WHEEL
+Filename: xia_scw_vpc-0.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: xia_scw_vpc-0.0.8.dist-info/top_level.txt
+Filename: xia_scw_vpc-0.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_scw_vpc-0.0.8.dist-info/RECORD
+Filename: xia_scw_vpc-0.0.9.dist-info/RECORD
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
 
-__version__ = "0.0.8"
+__version__ = "0.0.9"
```

