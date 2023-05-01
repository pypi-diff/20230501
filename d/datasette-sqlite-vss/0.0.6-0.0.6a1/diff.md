# Comparing `tmp/datasette_sqlite_vss-0.0.6-py3-none-any.whl.zip` & `tmp/datasette_sqlite_vss-0.0.6a1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 2094 bytes, number of entries: 7
+Zip file size: 2126 bytes, number of entries: 7
 -rw-r--r--  2.0 unx      190 b- defN 23-Apr-11 23:32 datasette_sqlite_vss/__init__.py
--rw-r--r--  2.0 unx       71 b- defN 23-May-01 21:12 datasette_sqlite_vss/version.py
--rw-r--r--  2.0 unx      555 b- defN 23-May-01 21:16 datasette_sqlite_vss-0.0.6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-01 21:16 datasette_sqlite_vss-0.0.6.dist-info/WHEEL
--rw-r--r--  2.0 unx       46 b- defN 23-May-01 21:16 datasette_sqlite_vss-0.0.6.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       21 b- defN 23-May-01 21:16 datasette_sqlite_vss-0.0.6.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      631 b- defN 23-May-01 21:16 datasette_sqlite_vss-0.0.6.dist-info/RECORD
-7 files, 1606 bytes uncompressed, 948 bytes compressed:  41.0%
+-rw-r--r--  2.0 unx       79 b- defN 23-May-01 18:21 datasette_sqlite_vss/version.py
+-rw-r--r--  2.0 unx      557 b- defN 23-May-01 18:38 datasette_sqlite_vss-0.0.6a1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-01 18:38 datasette_sqlite_vss-0.0.6a1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       46 b- defN 23-May-01 18:38 datasette_sqlite_vss-0.0.6a1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       21 b- defN 23-May-01 18:38 datasette_sqlite_vss-0.0.6a1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      641 b- defN 23-May-01 18:38 datasette_sqlite_vss-0.0.6a1.dist-info/RECORD
+7 files, 1626 bytes uncompressed, 960 bytes compressed:  41.0%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: datasette_sqlite_vss/__init__.py
 Comment: 
 
 Filename: datasette_sqlite_vss/version.py
 Comment: 
 
-Filename: datasette_sqlite_vss-0.0.6.dist-info/METADATA
+Filename: datasette_sqlite_vss-0.0.6a1.dist-info/METADATA
 Comment: 
 
-Filename: datasette_sqlite_vss-0.0.6.dist-info/WHEEL
+Filename: datasette_sqlite_vss-0.0.6a1.dist-info/WHEEL
 Comment: 
 
-Filename: datasette_sqlite_vss-0.0.6.dist-info/entry_points.txt
+Filename: datasette_sqlite_vss-0.0.6a1.dist-info/entry_points.txt
 Comment: 
 
-Filename: datasette_sqlite_vss-0.0.6.dist-info/top_level.txt
+Filename: datasette_sqlite_vss-0.0.6a1.dist-info/top_level.txt
 Comment: 
 
-Filename: datasette_sqlite_vss-0.0.6.dist-info/RECORD
+Filename: datasette_sqlite_vss-0.0.6a1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## datasette_sqlite_vss/version.py

```diff
@@ -1,2 +1,2 @@
-__version__ = "0.0.6"
+__version__ = "0.0.6-alpha.1"
 __version_info__ = tuple(__version__.split("."))
```

## Comparing `datasette_sqlite_vss-0.0.6.dist-info/METADATA` & `datasette_sqlite_vss-0.0.6a1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datasette-sqlite-vss
-Version: 0.0.6
+Version: 0.0.6a1
 Home-page: https://github.com/asg017/sqlite-vss
 Author: Alex Garcia
 License: MIT License, Apache License, Version 2.0
 Project-URL: Issues, https://github.com/asg017/sqlite-vss/issues
 Project-URL: CI, https://github.com/asg017/sqlite-vss/actions
 Project-URL: Changelog, https://github.com/asg017/sqlite-vss/releases
 Requires-Python: >=3.7
```

## Comparing `datasette_sqlite_vss-0.0.6.dist-info/RECORD` & `datasette_sqlite_vss-0.0.6a1.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 datasette_sqlite_vss/__init__.py,sha256=1LCY-tIpHYiF1CGp5tVBgnPCn78QmwrvJqYyXm9l6Lg,190
-datasette_sqlite_vss/version.py,sha256=eIFQfgHdSnossakRkddTLMf-gqn3H8qsKnvTNoZuv9M,71
-datasette_sqlite_vss-0.0.6.dist-info/METADATA,sha256=MYt-7kyePnh8y-LWX2WghW39HdNggKQ-dS4VOvBBhzs,555
-datasette_sqlite_vss-0.0.6.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-datasette_sqlite_vss-0.0.6.dist-info/entry_points.txt,sha256=g6SBQV6Ze7DSQV75d0uxi0GSY9DKaGFreDJOoEHFU9o,46
-datasette_sqlite_vss-0.0.6.dist-info/top_level.txt,sha256=8_4ggvGdXsDCGTgnJVyL91drVfMloM7dakkdf2EPRcw,21
-datasette_sqlite_vss-0.0.6.dist-info/RECORD,,
+datasette_sqlite_vss/version.py,sha256=OAOSSOPnNB5MG0JvavhpgRS1AuZXUdRUpkDUkwGWqOA,79
+datasette_sqlite_vss-0.0.6a1.dist-info/METADATA,sha256=ps2RcznEi_-dxvQZ31qaJ78iT2LW_SYevn-x1hSx5DY,557
+datasette_sqlite_vss-0.0.6a1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+datasette_sqlite_vss-0.0.6a1.dist-info/entry_points.txt,sha256=g6SBQV6Ze7DSQV75d0uxi0GSY9DKaGFreDJOoEHFU9o,46
+datasette_sqlite_vss-0.0.6a1.dist-info/top_level.txt,sha256=8_4ggvGdXsDCGTgnJVyL91drVfMloM7dakkdf2EPRcw,21
+datasette_sqlite_vss-0.0.6a1.dist-info/RECORD,,
```

