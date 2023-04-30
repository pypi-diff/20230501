# Comparing `tmp/itkwasm_compress_stringify-0.4.4.tar.gz` & `tmp/itkwasm_compress_stringify-0.4.5.tar.gz`

## Comparing `itkwasm_compress_stringify-0.4.4.tar` & `itkwasm_compress_stringify-0.4.5.tar`

### file list

```diff
@@ -1,12 +1,19 @@
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-0.4.4/itkwasm_compress_stringify/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-0.4.4/itkwasm_compress_stringify/_version.py
--rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-0.4.4/itkwasm_compress_stringify/compress_stringify.py
--rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-0.4.4/itkwasm_compress_stringify/compress_stringify_async.py
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-0.4.4/itkwasm_compress_stringify/parse_string_decompress.py
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-0.4.4/itkwasm_compress_stringify/parse_string_decompress_async.py
--rw-r--r--   0        0        0     2562 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-0.4.4/test/test_compress_stringify_emscripten.py
--rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-0.4.4/test/test_compress_stringify_wasi.py
--rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-0.4.4/.gitignore
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-0.4.4/README.md
--rw-r--r--   0        0        0     1822 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-0.4.4/pyproject.toml
--rw-r--r--   0        0        0     1441 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-0.4.5/docs/Makefile
+-rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-0.4.5/docs/conf.py
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-0.4.5/docs/index.md
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-0.4.5/docs/make.bat
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-0.4.5/docs/requirements.txt
+-rw-r--r--   0        0        0    13605 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-0.4.5/docs/_static/favicon.png
+-rw-r--r--   0        0        0     2949 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-0.4.5/docs/_static/logo.svg
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-0.4.5/itkwasm_compress_stringify/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-0.4.5/itkwasm_compress_stringify/_version.py
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-0.4.5/itkwasm_compress_stringify/compress_stringify.py
+-rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-0.4.5/itkwasm_compress_stringify/compress_stringify_async.py
+-rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-0.4.5/itkwasm_compress_stringify/parse_string_decompress.py
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-0.4.5/itkwasm_compress_stringify/parse_string_decompress_async.py
+-rw-r--r--   0        0        0     2562 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-0.4.5/test/test_compress_stringify_emscripten.py
+-rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-0.4.5/test/test_compress_stringify_wasi.py
+-rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-0.4.5/.gitignore
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-0.4.5/README.md
+-rw-r--r--   0        0        0     1822 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-0.4.5/pyproject.toml
+-rw-r--r--   0        0        0     1441 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-0.4.5/PKG-INFO
```

### Comparing `itkwasm_compress_stringify-0.4.4/itkwasm_compress_stringify/compress_stringify.py` & `itkwasm_compress_stringify-0.4.5/itkwasm_compress_stringify/compress_stringify_async.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,41 +1,35 @@
 # Generated file. Do not edit.
 
+from typing import Optional
+
 from itkwasm import (
     environment_dispatch,
     BinaryStream,
 )
 
-def compress_stringify(
+async def compress_stringify_async(
     input: bytes,
     stringify: bool = False,
     compression_level: int = 3,
     data_url_prefix: str = "data:base64,",
 ) -> bytes:
     """Given a binary, compress and optionally base64 encode.
 
-    Parameters
-    ----------
-
-    input: bytes
-        Input binary
-
-    stringify: bool, optional
-        Stringify the output
-
-    compression_level: int, optional
-        Compression level, typically 1-9
-
-    data_url_prefix: str, optional
-        dataURL prefix
+    :param input: Input binary
+    :type  input: bytes
 
+    :param stringify: Stringify the output
+    :type  stringify: bool
 
-    Returns
-    -------
+    :param compression_level: Compression level, typically 1-9
+    :type  compression_level: int
 
-    bytes
-        Output compressed binary
+    :param data_url_prefix: dataURL prefix
+    :type  data_url_prefix: str
 
+    :return: Output compressed binary
+    :rtype:  bytes
     """
-    func = environment_dispatch("itkwasm_compress_stringify", "compress_stringify")
-    output = func(input, stringify=stringify, compression_level=compression_level, data_url_prefix=data_url_prefix)
+    func = environment_dispatch("itkwasm_compress_stringify", "compress_stringify_async")
+    output = await func(input, stringify=stringify, compression_level=compression_level, data_url_prefix=data_url_prefix)
     return output
```

### Comparing `itkwasm_compress_stringify-0.4.4/itkwasm_compress_stringify/compress_stringify_async.py` & `itkwasm_compress_stringify-0.4.5/itkwasm_compress_stringify/compress_stringify.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,41 +1,35 @@
 # Generated file. Do not edit.
 
+from typing import Optional
+
 from itkwasm import (
     environment_dispatch,
     BinaryStream,
 )
 
-async def compress_stringify_async(
+def compress_stringify(
     input: bytes,
     stringify: bool = False,
     compression_level: int = 3,
     data_url_prefix: str = "data:base64,",
 ) -> bytes:
     """Given a binary, compress and optionally base64 encode.
 
-    Parameters
-    ----------
-
-    input: bytes
-        Input binary
-
-    stringify: bool, optional
-        Stringify the output
-
-    compression_level: int, optional
-        Compression level, typically 1-9
-
-    data_url_prefix: str, optional
-        dataURL prefix
+    :param input: Input binary
+    :type  input: bytes
 
+    :param stringify: Stringify the output
+    :type  stringify: bool
 
-    Returns
-    -------
+    :param compression_level: Compression level, typically 1-9
+    :type  compression_level: int
 
-    bytes
-        Output compressed binary
+    :param data_url_prefix: dataURL prefix
+    :type  data_url_prefix: str
 
+    :return: Output compressed binary
+    :rtype:  bytes
     """
-    func = environment_dispatch("itkwasm_compress_stringify", "compress_stringify_async")
-    output = await func(input, stringify=stringify, compression_level=compression_level, data_url_prefix=data_url_prefix)
+    func = environment_dispatch("itkwasm_compress_stringify", "compress_stringify")
+    output = func(input, stringify=stringify, compression_level=compression_level, data_url_prefix=data_url_prefix)
     return output
```

### Comparing `itkwasm_compress_stringify-0.4.4/itkwasm_compress_stringify/parse_string_decompress.py` & `itkwasm_compress_stringify-0.4.5/itkwasm_compress_stringify/parse_string_decompress.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,33 +1,27 @@
 # Generated file. Do not edit.
 
+from typing import Optional
+
 from itkwasm import (
     environment_dispatch,
     BinaryStream,
 )
 
 def parse_string_decompress(
     input: bytes,
     parse_string: bool = False,
 ) -> bytes:
     """Given a binary or string produced with compress-stringify, decompress and optionally base64 decode.
 
-    Parameters
-    ----------
-
-    input: bytes
-        Compressed input
-
-    parse_string: bool, optional
-        Parse the input string before decompression
-
-
-    Returns
-    -------
+    :param input: Compressed input
+    :type  input: bytes
 
-    bytes
-        Output decompressed binary
+    :param parse_string: Parse the input string before decompression
+    :type  parse_string: bool
 
+    :return: Output decompressed binary
+    :rtype:  bytes
     """
     func = environment_dispatch("itkwasm_compress_stringify", "parse_string_decompress")
     output = func(input, parse_string=parse_string)
     return output
```

### Comparing `itkwasm_compress_stringify-0.4.4/itkwasm_compress_stringify/parse_string_decompress_async.py` & `itkwasm_compress_stringify-0.4.5/itkwasm_compress_stringify/parse_string_decompress_async.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,33 +1,27 @@
 # Generated file. Do not edit.
 
+from typing import Optional
+
 from itkwasm import (
     environment_dispatch,
     BinaryStream,
 )
 
 async def parse_string_decompress_async(
     input: bytes,
     parse_string: bool = False,
 ) -> bytes:
     """Given a binary or string produced with compress-stringify, decompress and optionally base64 decode.
 
-    Parameters
-    ----------
-
-    input: bytes
-        Compressed input
-
-    parse_string: bool, optional
-        Parse the input string before decompression
-
-
-    Returns
-    -------
+    :param input: Compressed input
+    :type  input: bytes
 
-    bytes
-        Output decompressed binary
+    :param parse_string: Parse the input string before decompression
+    :type  parse_string: bool
 
+    :return: Output decompressed binary
+    :rtype:  bytes
     """
     func = environment_dispatch("itkwasm_compress_stringify", "parse_string_decompress_async")
     output = await func(input, parse_string=parse_string)
     return output
```

### Comparing `itkwasm_compress_stringify-0.4.4/test/test_compress_stringify_emscripten.py` & `itkwasm_compress_stringify-0.4.5/test/test_compress_stringify_emscripten.py`

 * *Files identical despite different names*

### Comparing `itkwasm_compress_stringify-0.4.4/test/test_compress_stringify_wasi.py` & `itkwasm_compress_stringify-0.4.5/test/test_compress_stringify_wasi.py`

 * *Files identical despite different names*

### Comparing `itkwasm_compress_stringify-0.4.4/.gitignore` & `itkwasm_compress_stringify-0.4.5/.gitignore`

 * *Files identical despite different names*

### Comparing `itkwasm_compress_stringify-0.4.4/pyproject.toml` & `itkwasm_compress_stringify-0.4.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `itkwasm_compress_stringify-0.4.4/PKG-INFO` & `itkwasm_compress_stringify-0.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: itkwasm-compress-stringify
-Version: 0.4.4
+Version: 0.4.5
 License-Expression: Apache-2.0
 Keywords: emscripten,itkwasm,wasi,webassembly
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: WebAssembly
 Classifier: Environment :: WebAssembly :: Emscripten
 Classifier: Environment :: WebAssembly :: WASI
 Classifier: Intended Audience :: Developers
```

