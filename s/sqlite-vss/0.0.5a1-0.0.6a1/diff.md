# Comparing `tmp/sqlite_vss-0.0.5a1-py3-none-manylinux_2_17_x86_64.manylinux2014_x86_64.manylinux1_x86_64.whl.zip` & `tmp/sqlite_vss-0.0.6a1-py3-none-manylinux_2_17_x86_64.manylinux2014_x86_64.manylinux1_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 1546219 bytes, number of entries: 9
--rwxr-xr-x  2.0 unx    15784 b- defN 23-Apr-26 20:21 noop.cpython-311-x86_64-linux-gnu.so
--rw-r--r--  2.0 unx      572 b- defN 23-Apr-26 20:21 sqlite_vss/__init__.py
--rw-r--r--  2.0 unx   186896 b- defN 23-Apr-26 20:21 sqlite_vss/vector0.so
--rw-r--r--  2.0 unx       79 b- defN 23-Apr-26 20:21 sqlite_vss/version.py
--rw-r--r--  2.0 unx  5124432 b- defN 23-Apr-26 20:21 sqlite_vss/vss0.so
--rw-r--r--  2.0 unx      496 b- defN 23-Apr-26 20:21 sqlite_vss-0.0.5a1.dist-info/METADATA
--rw-r--r--  2.0 unx      105 b- defN 23-Apr-26 20:21 sqlite_vss-0.0.5a1.dist-info/WHEEL
--rw-r--r--  2.0 unx       16 b- defN 23-Apr-26 20:21 sqlite_vss-0.0.5a1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      724 b- defN 23-Apr-26 20:21 sqlite_vss-0.0.5a1.dist-info/RECORD
-9 files, 5329104 bytes uncompressed, 1544981 bytes compressed:  71.0%
+Zip file size: 1546222 bytes, number of entries: 9
+-rwxr-xr-x  2.0 unx    15784 b- defN 23-May-01 18:25 noop.cpython-311-x86_64-linux-gnu.so
+-rw-r--r--  2.0 unx      572 b- defN 23-May-01 18:24 sqlite_vss/__init__.py
+-rw-r--r--  2.0 unx   186896 b- defN 23-May-01 18:25 sqlite_vss/vector0.so
+-rw-r--r--  2.0 unx       79 b- defN 23-May-01 18:24 sqlite_vss/version.py
+-rw-r--r--  2.0 unx  5124432 b- defN 23-May-01 18:25 sqlite_vss/vss0.so
+-rw-r--r--  2.0 unx      496 b- defN 23-May-01 18:25 sqlite_vss-0.0.6a1.dist-info/METADATA
+-rw-r--r--  2.0 unx      105 b- defN 23-May-01 18:25 sqlite_vss-0.0.6a1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       16 b- defN 23-May-01 18:25 sqlite_vss-0.0.6a1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      724 b- defN 23-May-01 18:25 sqlite_vss-0.0.6a1.dist-info/RECORD
+9 files, 5329104 bytes uncompressed, 1544984 bytes compressed:  71.0%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: sqlite_vss/version.py
 Comment: 
 
 Filename: sqlite_vss/vss0.so
 Comment: 
 
-Filename: sqlite_vss-0.0.5a1.dist-info/METADATA
+Filename: sqlite_vss-0.0.6a1.dist-info/METADATA
 Comment: 
 
-Filename: sqlite_vss-0.0.5a1.dist-info/WHEEL
+Filename: sqlite_vss-0.0.6a1.dist-info/WHEEL
 Comment: 
 
-Filename: sqlite_vss-0.0.5a1.dist-info/top_level.txt
+Filename: sqlite_vss-0.0.6a1.dist-info/top_level.txt
 Comment: 
 
-Filename: sqlite_vss-0.0.5a1.dist-info/RECORD
+Filename: sqlite_vss-0.0.6a1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sqlite_vss/vector0.so

 * *File has been modified after NT_GNU_BUILD_ID has been applied.*

### readelf --wide --notes {}

```diff
@@ -1,8 +1,8 @@
 
 Displaying notes found in: .note.gnu.property
   Owner                Data size 	Description
   GNU                  0x00000010	NT_GNU_PROPERTY_TYPE_0	      Properties: x86 feature: IBT, SHSTK
 
 Displaying notes found in: .note.gnu.build-id
   Owner                Data size 	Description
-  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: 5adb938442c7f6a32c049e73e79bce1c493549b5
+  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: 68f67eadb0d6ed9de3cf24b41ab53ea4e36e81f2
```

### strings --all --bytes=8 {}

```diff
@@ -331,15 +331,15 @@
 AWAVAUATUH
 []A\A]A^A_
 []A\A]A^A_
 AWAVAUATL
 []A\A]A^A_
 AVAUATUH
 []A\A]A^A_
-v0.0.5-alpha.1
+v0.0.6-alpha.1
 vector0_api_ptr
 Blob type not right
 vector_fvecs_each
 vector::_M_range_insert
 %d out of range: %s
 value not a vector
 size: %lld [
```

### readelf --wide --decompress --hex-dump=.rodata {}

```diff
@@ -1,10 +1,10 @@
 
 Hex dump of section '.rodata':
-  0x0001f000 76302e30 2e352d61 6c706861 2e310076 v0.0.5-alpha.1.v
+  0x0001f000 76302e30 2e362d61 6c706861 2e310076 v0.0.6-alpha.1.v
   0x0001f010 6563746f 72305f61 70695f70 74720042 ector0_api_ptr.B
   0x0001f020 6c6f6220 74797065 206e6f74 20726967 lob type not rig
   0x0001f030 68740076 6563746f 72300025 733a2025 ht.vector0.%s: %
   0x0001f040 73007665 63746f72 5f667665 63735f65 s.vector_fvecs_e
   0x0001f050 61636800 76656374 6f723a3a 5f4d5f72 ach.vector::_M_r
   0x0001f060 616e6765 5f696e73 65727400 2564206f ange_insert.%d o
   0x0001f070 7574206f 66207261 6e67653a 20257300 ut of range: %s.
```

## sqlite_vss/version.py

```diff
@@ -1,2 +1,2 @@
-__version__ = "0.0.5-alpha.1"
+__version__ = "0.0.6-alpha.1"
 __version_info__ = tuple(__version__.split("."))
```

## sqlite_vss/vss0.so

 * *File has been modified after NT_GNU_BUILD_ID has been applied.*

### readelf --wide --notes {}

```diff
@@ -1,8 +1,8 @@
 
 Displaying notes found in: .note.gnu.property
   Owner                Data size 	Description
   GNU                  0x00000010	NT_GNU_PROPERTY_TYPE_0	      Properties: x86 feature: IBT, SHSTK
 
 Displaying notes found in: .note.gnu.build-id
   Owner                Data size 	Description
-  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: 5b784ac561983f2d4d10dc5e0edcba571636a1f5
+  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: 0887affcc80398bcb92a4f0dee3ce479637e33f1
```

### strings --all --bytes=8 {}

```diff
@@ -7386,15 +7386,15 @@
 AWAVAUATUSH
 L$ H9L$8
 []A\A]A^A_
 AWAVAUATUSH
 []A\A]A^A_
 AWAVAUATI
 [A\A]A^A_]
-v0.0.5-alpha.1
+v0.0.6-alpha.1
 fullscan
 vss_search
 vss_range_search
 1st argument is not a vector
 vss0_rangesearchparams
 vss0_searchparams
 drop table "%w_index";
```

### readelf --wide --decompress --hex-dump=.rodata {}

```diff
@@ -1,10 +1,10 @@
 
 Hex dump of section '.rodata':
-  0x00380000 76302e30 2e352d61 6c706861 2e310066 v0.0.5-alpha.1.f
+  0x00380000 76302e30 2e362d61 6c706861 2e310066 v0.0.6-alpha.1.f
   0x00380010 756c6c73 63616e00 7673735f 73656172 ullscan.vss_sear
   0x00380020 63680076 73735f72 616e6765 5f736561 ch.vss_range_sea
   0x00380030 72636800 31737420 61726775 6d656e74 rch.1st argument
   0x00380040 20697320 6e6f7420 61207665 63746f72  is not a vector
   0x00380050 00767373 305f7261 6e676573 65617263 .vss0_rangesearc
   0x00380060 68706172 616d7300 76737330 5f736561 hparams.vss0_sea
   0x00380070 72636870 6172616d 73006472 6f702074 rchparams.drop t
```

## Comparing `sqlite_vss-0.0.5a1.dist-info/RECORD` & `sqlite_vss-0.0.6a1.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 noop.cpython-311-x86_64-linux-gnu.so,sha256=4swCe5ZHJGjSyqveLIyVe-H5qqHAIdWOwZb7Gpobwx8,15784
 sqlite_vss/__init__.py,sha256=5PIhAIaJ1cVKtzSV9eZaymWS4CjRHUjkJ6y8VXyaG8Y,572
-sqlite_vss/vector0.so,sha256=nZxRgX4HYLpmur-F3AJh0YAAaa-4pGFQwpu8Xi9PcOQ,186896
-sqlite_vss/version.py,sha256=-Nb9lEXxw0Qwq4JQs7JgIgGJpM2zBwRNWpqHF9CxOLQ,79
-sqlite_vss/vss0.so,sha256=GIQp40zXJHAu1F12GkBV-_EXNKWPpd4RLNmhnNjpgHw,5124432
-sqlite_vss-0.0.5a1.dist-info/METADATA,sha256=Sjnx8gqop9YNbJHvjDNM-xsGnUEM_CPHauZvoOO02bk,496
-sqlite_vss-0.0.5a1.dist-info/WHEEL,sha256=A8X7wachHegSPoWuFmtYiHrJoCGdZ0KzfYp5hU1FoC8,105
-sqlite_vss-0.0.5a1.dist-info/top_level.txt,sha256=Z2PPuSp9qvLljXNaO4Jwv8wSXtVhLIU2qBu5OEgZxGQ,16
-sqlite_vss-0.0.5a1.dist-info/RECORD,,
+sqlite_vss/vector0.so,sha256=P6pc2ot23dBU7Ojbiqf472owNHyxJqBjKJX2TljUGiQ,186896
+sqlite_vss/version.py,sha256=OAOSSOPnNB5MG0JvavhpgRS1AuZXUdRUpkDUkwGWqOA,79
+sqlite_vss/vss0.so,sha256=oSVtMfocAbn-cQuG36DaRft6dh22nJ-gwcdMJcHIbw0,5124432
+sqlite_vss-0.0.6a1.dist-info/METADATA,sha256=pkhvBEhRvE226cUCdbPBK7hKSgMJX4_pw-60bNMuNgM,496
+sqlite_vss-0.0.6a1.dist-info/WHEEL,sha256=A8X7wachHegSPoWuFmtYiHrJoCGdZ0KzfYp5hU1FoC8,105
+sqlite_vss-0.0.6a1.dist-info/top_level.txt,sha256=Z2PPuSp9qvLljXNaO4Jwv8wSXtVhLIU2qBu5OEgZxGQ,16
+sqlite_vss-0.0.6a1.dist-info/RECORD,,
```

