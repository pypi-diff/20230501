# Comparing `tmp/wasmer-1.1.0-py3-none-any.whl.zip` & `tmp/wasmer-1.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 1617 bytes, number of entries: 5
--rw-r--r--  2.0 unx       60 b- defN 22-Jan-07 23:13 wasmer/__init__.py
--rw-r--r--  2.0 unx      818 b- defN 22-Jan-07 23:19 wasmer-1.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Jan-07 23:19 wasmer-1.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 22-Jan-07 23:19 wasmer-1.1.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      365 b- defN 22-Jan-07 23:19 wasmer-1.1.0.dist-info/RECORD
-5 files, 1342 bytes uncompressed, 931 bytes compressed:  30.6%
+Zip file size: 1602 bytes, number of entries: 5
+-rw-r--r--  2.0 unx       60 b- defN 23-May-01 16:19 wasmer/__init__.py
+-rw-r--r--  2.0 unx      798 b- defN 23-May-01 16:49 wasmer-1.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-01 16:49 wasmer-1.2.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 23-May-01 16:49 wasmer-1.2.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      365 b- defN 23-May-01 16:49 wasmer-1.2.0.dist-info/RECORD
+5 files, 1322 bytes uncompressed, 916 bytes compressed:  30.7%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: wasmer/__init__.py
 Comment: 
 
-Filename: wasmer-1.1.0.dist-info/METADATA
+Filename: wasmer-1.2.0.dist-info/METADATA
 Comment: 
 
-Filename: wasmer-1.1.0.dist-info/WHEEL
+Filename: wasmer-1.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: wasmer-1.1.0.dist-info/top_level.txt
+Filename: wasmer-1.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: wasmer-1.1.0.dist-info/RECORD
+Filename: wasmer-1.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `wasmer-1.1.0.dist-info/METADATA` & `wasmer-1.2.0.dist-info/METADATA`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 Metadata-Version: 2.1
 Name: wasmer
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
 
 # `wasmer-any`
 
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

