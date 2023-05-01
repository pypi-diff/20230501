# Comparing `tmp/wasmer_compiler_cranelift-1.1.0-py3-none-any.whl.zip` & `tmp/wasmer_compiler_cranelift-1.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 1866 bytes, number of entries: 5
--rw-r--r--  2.0 unx       79 b- defN 22-Jan-07 23:13 wasmer_compiler_cranelift/__init__.py
--rw-r--r--  2.0 unx      856 b- defN 22-Jan-07 23:19 wasmer_compiler_cranelift-1.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Jan-07 23:19 wasmer_compiler_cranelift-1.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       26 b- defN 22-Jan-07 23:19 wasmer_compiler_cranelift-1.1.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      461 b- defN 22-Jan-07 23:19 wasmer_compiler_cranelift-1.1.0.dist-info/RECORD
-5 files, 1514 bytes uncompressed, 990 bytes compressed:  34.6%
+Zip file size: 1850 bytes, number of entries: 5
+-rw-r--r--  2.0 unx       79 b- defN 23-May-01 16:19 wasmer_compiler_cranelift/__init__.py
+-rw-r--r--  2.0 unx      836 b- defN 23-May-01 16:49 wasmer_compiler_cranelift-1.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-01 16:49 wasmer_compiler_cranelift-1.2.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       26 b- defN 23-May-01 16:49 wasmer_compiler_cranelift-1.2.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      461 b- defN 23-May-01 16:49 wasmer_compiler_cranelift-1.2.0.dist-info/RECORD
+5 files, 1494 bytes uncompressed, 974 bytes compressed:  34.8%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: wasmer_compiler_cranelift/__init__.py
 Comment: 
 
-Filename: wasmer_compiler_cranelift-1.1.0.dist-info/METADATA
+Filename: wasmer_compiler_cranelift-1.2.0.dist-info/METADATA
 Comment: 
 
-Filename: wasmer_compiler_cranelift-1.1.0.dist-info/WHEEL
+Filename: wasmer_compiler_cranelift-1.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: wasmer_compiler_cranelift-1.1.0.dist-info/top_level.txt
+Filename: wasmer_compiler_cranelift-1.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: wasmer_compiler_cranelift-1.1.0.dist-info/RECORD
+Filename: wasmer_compiler_cranelift-1.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `wasmer_compiler_cranelift-1.1.0.dist-info/METADATA` & `wasmer_compiler_cranelift-1.2.0.dist-info/METADATA`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 Metadata-Version: 2.1
 Name: wasmer-compiler-cranelift
-Version: 1.1.0
+Version: 1.2.0
 Summary: Python extension to run WebAssembly binaries
-Home-page: UNKNOWN
 Author: The Wasmer Engineering Team
 Author-email: engineering@wasmer.io
 License: MIT
 Platform: any
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
 # `wasmer-compiler-cranelift-any`
 
 A special `wasmer-$(version)-py3-none-any` wheel is built as a
-fallback. The `wasmer` libray will be installable, but it will raise
+fallback. The `wasmer` library will be installable, but it will raise
 an `ImportError` exception saying that “Wasmer is not available on
 this system”.
 
 This wheel will be installed if none matches before (learn more by
 reading the [PEP 425, Compatibility Tags for Built
 Distributions](https://www.python.org/dev/peps/pep-0425/)).
-
-
```

