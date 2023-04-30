# Comparing `tmp/itkwasm_compress_stringify_wasi-0.4.4.tar.gz` & `tmp/itkwasm_compress_stringify_wasi-0.4.5.tar.gz`

## Comparing `itkwasm_compress_stringify_wasi-0.4.4.tar` & `itkwasm_compress_stringify_wasi-0.4.5.tar`

### file list

```diff
@@ -1,11 +1,13 @@
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 itkwasm_compress_stringify_wasi-0.4.4/itkwasm_compress_stringify_wasi/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 itkwasm_compress_stringify_wasi-0.4.4/itkwasm_compress_stringify_wasi/_version.py
--rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 itkwasm_compress_stringify_wasi-0.4.4/itkwasm_compress_stringify_wasi/compress_stringify.py
--rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 itkwasm_compress_stringify_wasi-0.4.4/itkwasm_compress_stringify_wasi/parse_string_decompress.py
--rwxr-xr-x   0        0        0   985708 2020-02-02 00:00:00.000000 itkwasm_compress_stringify_wasi-0.4.4/itkwasm_compress_stringify_wasi/wasm_modules/compress-stringify.wasi.wasm
--rwxr-xr-x   0        0        0   678328 2020-02-02 00:00:00.000000 itkwasm_compress_stringify_wasi-0.4.4/itkwasm_compress_stringify_wasi/wasm_modules/parse-string-decompress.wasi.wasm
--rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 itkwasm_compress_stringify_wasi-0.4.4/test/test_compress_stringify.py
--rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 itkwasm_compress_stringify_wasi-0.4.4/.gitignore
--rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 itkwasm_compress_stringify_wasi-0.4.4/README.md
--rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 itkwasm_compress_stringify_wasi-0.4.4/pyproject.toml
--rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 itkwasm_compress_stringify_wasi-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 itkwasm_compress_stringify_wasi-0.4.5/itkwasm_compress_stringify_wasi/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 itkwasm_compress_stringify_wasi-0.4.5/itkwasm_compress_stringify_wasi/_version.py
+-rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 itkwasm_compress_stringify_wasi-0.4.5/itkwasm_compress_stringify_wasi/compress_stringify.py
+-rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 itkwasm_compress_stringify_wasi-0.4.5/itkwasm_compress_stringify_wasi/parse_string_decompress.py
+-rwxr-xr-x   0        0        0   985708 2020-02-02 00:00:00.000000 itkwasm_compress_stringify_wasi-0.4.5/itkwasm_compress_stringify_wasi/wasm_modules/compress-stringify.wasi.wasm
+-rwxr-xr-x   0        0        0   753714 2020-02-02 00:00:00.000000 itkwasm_compress_stringify_wasi-0.4.5/itkwasm_compress_stringify_wasi/wasm_modules/compress-stringify.wasm
+-rwxr-xr-x   0        0        0   678328 2020-02-02 00:00:00.000000 itkwasm_compress_stringify_wasi-0.4.5/itkwasm_compress_stringify_wasi/wasm_modules/parse-string-decompress.wasi.wasm
+-rwxr-xr-x   0        0        0   469805 2020-02-02 00:00:00.000000 itkwasm_compress_stringify_wasi-0.4.5/itkwasm_compress_stringify_wasi/wasm_modules/parse-string-decompress.wasm
+-rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 itkwasm_compress_stringify_wasi-0.4.5/test/test_compress_stringify.py
+-rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 itkwasm_compress_stringify_wasi-0.4.5/.gitignore
+-rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 itkwasm_compress_stringify_wasi-0.4.5/README.md
+-rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 itkwasm_compress_stringify_wasi-0.4.5/pyproject.toml
+-rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 itkwasm_compress_stringify_wasi-0.4.5/PKG-INFO
```

### Comparing `itkwasm_compress_stringify_wasi-0.4.4/itkwasm_compress_stringify_wasi/compress_stringify.py` & `itkwasm_compress_stringify_wasi-0.4.5/itkwasm_compress_stringify_wasi/compress_stringify.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Generated file. Do not edit.
 
 from pathlib import Path
 import os
-from typing import Dict, Tuple
+from typing import Dict, Tuple, Optional
 
 from importlib_resources import files as file_resources
 
 from itkwasm import (
     InterfaceTypes,
     PipelineOutput,
     PipelineInput,
@@ -18,36 +18,28 @@
     input: bytes,
     stringify: bool = False,
     compression_level: int = 3,
     data_url_prefix: str = "data:base64,",
 ) -> bytes:
     """Given a binary, compress and optionally base64 encode.
 
-    Parameters
-    ----------
+    :param input: Input binary
+    :type  input: bytes
 
-    input: bytes
-        Input binary
+    :param stringify: Stringify the output
+    :type  stringify: bool
 
-    stringify: bool, optional
-        Stringify the output
+    :param compression_level: Compression level, typically 1-9
+    :type  compression_level: int
 
-    compression_level: int, optional
-        Compression level, typically 1-9
-
-    data_url_prefix: str, optional
-        dataURL prefix
-
-
-    Returns
-    -------
-
-    bytes
-        Output compressed binary
+    :param data_url_prefix: dataURL prefix
+    :type  data_url_prefix: str
 
+    :return: Output compressed binary
+    :rtype:  bytes
     """
     pipeline = Pipeline(file_resources('itkwasm_compress_stringify_wasi').joinpath(Path('wasm_modules') / Path('compress-stringify.wasi.wasm')))
 
     pipeline_outputs: List[PipelineOutput] = [
         PipelineOutput(InterfaceTypes.BinaryStream),
     ]
 
@@ -57,26 +49,26 @@
 
     args: List[str] = ['--memory-io',]
     # Inputs
     args.append('0')
     # Outputs
     args.append('0')
     # Options
-    if stringify is not None:
+    if stringify:
         args.append('--stringify')
 
-    if compression_level is not None:
+    if compression_level:
         args.append('--compression-level')
         args.append(str(compression_level))
 
-    if data_url_prefix is not None:
+    if data_url_prefix:
         args.append('--data-url-prefix')
         args.append(str(data_url_prefix))
 
 
     outputs = pipeline.run(args, pipeline_outputs, pipeline_inputs)
 
+    del pipeline
+
     result = outputs[0].data.data
     return result
 
-
-    del pipeline
```

### Comparing `itkwasm_compress_stringify_wasi-0.4.4/itkwasm_compress_stringify_wasi/parse_string_decompress.py` & `itkwasm_compress_stringify_wasi-0.4.5/itkwasm_compress_stringify_wasi/parse_string_decompress.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Generated file. Do not edit.
 
 from pathlib import Path
 import os
-from typing import Dict, Tuple
+from typing import Dict, Tuple, Optional
 
 from importlib_resources import files as file_resources
 
 from itkwasm import (
     InterfaceTypes,
     PipelineOutput,
     PipelineInput,
@@ -16,30 +16,22 @@
 
 def parse_string_decompress(
     input: bytes,
     parse_string: bool = False,
 ) -> bytes:
     """Given a binary or string produced with compress-stringify, decompress and optionally base64 decode.
 
-    Parameters
-    ----------
+    :param input: Compressed input
+    :type  input: bytes
 
-    input: bytes
-        Compressed input
-
-    parse_string: bool, optional
-        Parse the input string before decompression
-
-
-    Returns
-    -------
-
-    bytes
-        Output decompressed binary
+    :param parse_string: Parse the input string before decompression
+    :type  parse_string: bool
 
+    :return: Output decompressed binary
+    :rtype:  bytes
     """
     pipeline = Pipeline(file_resources('itkwasm_compress_stringify_wasi').joinpath(Path('wasm_modules') / Path('parse-string-decompress.wasi.wasm')))
 
     pipeline_outputs: List[PipelineOutput] = [
         PipelineOutput(InterfaceTypes.BinaryStream),
     ]
 
@@ -49,18 +41,18 @@
 
     args: List[str] = ['--memory-io',]
     # Inputs
     args.append('0')
     # Outputs
     args.append('0')
     # Options
-    if parse_string is not None:
+    if parse_string:
         args.append('--parse-string')
 
 
     outputs = pipeline.run(args, pipeline_outputs, pipeline_inputs)
 
+    del pipeline
+
     result = outputs[0].data.data
     return result
 
-
-    del pipeline
```

### Comparing `itkwasm_compress_stringify_wasi-0.4.4/itkwasm_compress_stringify_wasi/wasm_modules/compress-stringify.wasi.wasm` & `itkwasm_compress_stringify_wasi-0.4.5/itkwasm_compress_stringify_wasi/wasm_modules/compress-stringify.wasi.wasm`

 * *Files identical despite different names*

### Comparing `itkwasm_compress_stringify_wasi-0.4.4/itkwasm_compress_stringify_wasi/wasm_modules/parse-string-decompress.wasi.wasm` & `itkwasm_compress_stringify_wasi-0.4.5/itkwasm_compress_stringify_wasi/wasm_modules/parse-string-decompress.wasi.wasm`

 * *Files identical despite different names*

### Comparing `itkwasm_compress_stringify_wasi-0.4.4/test/test_compress_stringify.py` & `itkwasm_compress_stringify_wasi-0.4.5/test/test_compress_stringify.py`

 * *Files identical despite different names*

### Comparing `itkwasm_compress_stringify_wasi-0.4.4/.gitignore` & `itkwasm_compress_stringify_wasi-0.4.5/.gitignore`

 * *Files identical despite different names*

### Comparing `itkwasm_compress_stringify_wasi-0.4.4/README.md` & `itkwasm_compress_stringify_wasi-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `itkwasm_compress_stringify_wasi-0.4.4/pyproject.toml` & `itkwasm_compress_stringify_wasi-0.4.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `itkwasm_compress_stringify_wasi-0.4.4/PKG-INFO` & `itkwasm_compress_stringify_wasi-0.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: itkwasm-compress-stringify-wasi
-Version: 0.4.4
+Version: 0.4.5
 License-Expression: Apache-2.0
 Keywords: itkwasm,wasi,webassembly
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: WebAssembly
 Classifier: Environment :: WebAssembly :: Emscripten
 Classifier: Environment :: WebAssembly :: WASI
 Classifier: Intended Audience :: Developers
```

