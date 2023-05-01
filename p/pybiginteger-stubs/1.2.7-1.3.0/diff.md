# Comparing `tmp/pybiginteger_stubs-1.2.7-py3-none-any.whl.zip` & `tmp/pybiginteger_stubs-1.3.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 2411 bytes, number of entries: 5
--rw-r--r--  2.0 unx     6470 b- defN 22-May-17 12:19 pybiginteger-stubs/__init__.pyi
--rw-r--r--  2.0 unx      271 b- defN 22-May-17 12:19 pybiginteger_stubs-1.2.7.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-May-17 12:19 pybiginteger_stubs-1.2.7.dist-info/WHEEL
--rw-r--r--  2.0 unx       19 b- defN 22-May-17 12:19 pybiginteger_stubs-1.2.7.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      429 b- defN 22-May-17 12:19 pybiginteger_stubs-1.2.7.dist-info/RECORD
-5 files, 7281 bytes uncompressed, 1603 bytes compressed:  78.0%
+Zip file size: 2376 bytes, number of entries: 5
+-rw-r--r--  2.0 unx     6470 b- defN 23-May-01 10:31 pybiginteger-stubs/__init__.pyi
+-rw-r--r--  2.0 unx      207 b- defN 23-May-01 10:31 pybiginteger_stubs-1.3.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-01 10:31 pybiginteger_stubs-1.3.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       19 b- defN 23-May-01 10:31 pybiginteger_stubs-1.3.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      429 b- defN 23-May-01 10:31 pybiginteger_stubs-1.3.0.dist-info/RECORD
+5 files, 7217 bytes uncompressed, 1568 bytes compressed:  78.3%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: pybiginteger-stubs/__init__.pyi
 Comment: 
 
-Filename: pybiginteger_stubs-1.2.7.dist-info/METADATA
+Filename: pybiginteger_stubs-1.3.0.dist-info/METADATA
 Comment: 
 
-Filename: pybiginteger_stubs-1.2.7.dist-info/WHEEL
+Filename: pybiginteger_stubs-1.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: pybiginteger_stubs-1.2.7.dist-info/top_level.txt
+Filename: pybiginteger_stubs-1.3.0.dist-info/top_level.txt
 Comment: 
 
-Filename: pybiginteger_stubs-1.2.7.dist-info/RECORD
+Filename: pybiginteger_stubs-1.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pybiginteger-stubs/__init__.pyi

```diff
@@ -167,9 +167,9 @@
     def zero() -> BigInteger: ...
     @property
     def sign(self) -> int:
         """
         :type: int
         """
     __version__ = '1.2'
-    __version_bindings__ = '1.2.7'
+    __version_bindings__ = '1.3.0'
     pass
```

