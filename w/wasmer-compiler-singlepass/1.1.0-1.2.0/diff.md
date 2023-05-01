# Comparing `tmp/wasmer_compiler_singlepass-1.1.0-py3-none-any.whl.zip` & `tmp/wasmer_compiler_singlepass-1.2.0-cp38-cp38-manylinux_2_34_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 1879 bytes, number of entries: 5
--rw-r--r--  2.0 unx       80 b- defN 22-Jan-07 23:13 wasmer_compiler_singlepass/__init__.py
--rw-r--r--  2.0 unx      858 b- defN 22-Jan-07 23:19 wasmer_compiler_singlepass-1.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Jan-07 23:19 wasmer_compiler_singlepass-1.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       27 b- defN 22-Jan-07 23:19 wasmer_compiler_singlepass-1.1.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      466 b- defN 22-Jan-07 23:19 wasmer_compiler_singlepass-1.1.0.dist-info/RECORD
-5 files, 1523 bytes uncompressed, 993 bytes compressed:  34.8%
+Zip file size: 627511 bytes, number of entries: 5
+-rw-r--r--  4.6 unx     2628 b- defN 23-May-01 16:36 wasmer_compiler_singlepass-1.2.0.dist-info/METADATA
+-rw-r--r--  4.6 unx      108 b- defN 23-May-01 16:36 wasmer_compiler_singlepass-1.2.0.dist-info/WHEEL
+-rw-r--r--  4.6 unx      187 b- defN 23-May-01 16:36 wasmer_compiler_singlepass/__init__.py
+-rwxr-xr-x  4.6 unx  2124288 b- defN 23-May-01 16:36 wasmer_compiler_singlepass/wasmer_compiler_singlepass.cpython-38-x86_64-linux-gnu.so
+-rw-r--r--  4.6 unx      502 b- defN 23-May-01 16:36 wasmer_compiler_singlepass-1.2.0.dist-info/RECORD
+5 files, 2127713 bytes uncompressed, 626569 bytes compressed:  70.6%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
-Filename: wasmer_compiler_singlepass/__init__.py
+Filename: wasmer_compiler_singlepass-1.2.0.dist-info/METADATA
 Comment: 
 
-Filename: wasmer_compiler_singlepass-1.1.0.dist-info/METADATA
+Filename: wasmer_compiler_singlepass-1.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: wasmer_compiler_singlepass-1.1.0.dist-info/WHEEL
+Filename: wasmer_compiler_singlepass/__init__.py
 Comment: 
 
-Filename: wasmer_compiler_singlepass-1.1.0.dist-info/top_level.txt
+Filename: wasmer_compiler_singlepass/wasmer_compiler_singlepass.cpython-38-x86_64-linux-gnu.so
 Comment: 
 
-Filename: wasmer_compiler_singlepass-1.1.0.dist-info/RECORD
+Filename: wasmer_compiler_singlepass-1.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## wasmer_compiler_singlepass/__init__.py

```diff
@@ -1 +1,5 @@
-raise ImportError("Wasmer Singlepass Compiler is not available on this system")
+from .wasmer_compiler_singlepass import *
+
+__doc__ = wasmer_compiler_singlepass.__doc__
+if hasattr(wasmer_compiler_singlepass, "__all__"):
+    __all__ = wasmer_compiler_singlepass.__all__
```

