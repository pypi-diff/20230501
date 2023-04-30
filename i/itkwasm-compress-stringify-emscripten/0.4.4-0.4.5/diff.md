# Comparing `tmp/itkwasm_compress_stringify_emscripten-0.4.4.tar.gz` & `tmp/itkwasm_compress_stringify_emscripten-0.4.5.tar.gz`

## Comparing `itkwasm_compress_stringify_emscripten-0.4.4.tar` & `itkwasm_compress_stringify_emscripten-0.4.5.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 itkwasm_compress_stringify_emscripten-0.4.4/itkwasm_compress_stringify_emscripten/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 itkwasm_compress_stringify_emscripten-0.4.4/itkwasm_compress_stringify_emscripten/_version.py
--rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 itkwasm_compress_stringify_emscripten-0.4.4/itkwasm_compress_stringify_emscripten/compress_stringify_async.py
--rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 itkwasm_compress_stringify_emscripten-0.4.4/itkwasm_compress_stringify_emscripten/parse_string_decompress_async.py
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 itkwasm_compress_stringify_emscripten-0.4.4/itkwasm_compress_stringify_emscripten/pyodide.py
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 itkwasm_compress_stringify_emscripten-0.4.4/test/test_compress_stringify.py
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 itkwasm_compress_stringify_emscripten-0.4.4/test/test_itkwasm_compress_stringify.py
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 itkwasm_compress_stringify_emscripten-0.4.4/.gitignore
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 itkwasm_compress_stringify_emscripten-0.4.4/README.md
--rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 itkwasm_compress_stringify_emscripten-0.4.4/pyproject.toml
--rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 itkwasm_compress_stringify_emscripten-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 itkwasm_compress_stringify_emscripten-0.4.5/itkwasm_compress_stringify_emscripten/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 itkwasm_compress_stringify_emscripten-0.4.5/itkwasm_compress_stringify_emscripten/_version.py
+-rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 itkwasm_compress_stringify_emscripten-0.4.5/itkwasm_compress_stringify_emscripten/compress_stringify_async.py
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 itkwasm_compress_stringify_emscripten-0.4.5/itkwasm_compress_stringify_emscripten/js_package.py
+-rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 itkwasm_compress_stringify_emscripten-0.4.5/itkwasm_compress_stringify_emscripten/parse_string_decompress_async.py
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 itkwasm_compress_stringify_emscripten-0.4.5/itkwasm_compress_stringify_emscripten/pyodide.py
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 itkwasm_compress_stringify_emscripten-0.4.5/test/test_compress_stringify.py
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 itkwasm_compress_stringify_emscripten-0.4.5/test/test_itkwasm_compress_stringify.py
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 itkwasm_compress_stringify_emscripten-0.4.5/.gitignore
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 itkwasm_compress_stringify_emscripten-0.4.5/README.md
+-rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 itkwasm_compress_stringify_emscripten-0.4.5/pyproject.toml
+-rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 itkwasm_compress_stringify_emscripten-0.4.5/PKG-INFO
```

### Comparing `itkwasm_compress_stringify_emscripten-0.4.4/itkwasm_compress_stringify_emscripten/compress_stringify_async.py` & `itkwasm_compress_stringify_emscripten-0.4.5/itkwasm_compress_stringify_emscripten/compress_stringify_async.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,56 +1,60 @@
 # Generated file. Do not edit.
 
 from pathlib import Path
 import os
-from typing import Dict, Tuple
+from typing import Dict, Tuple, Optional
 
-from .pyodide import js_package
+from .js_package import js_package
 
 from itkwasm.pyodide import (
     to_js,
     to_py,
     js_resources
 )
+from itkwasm import (
+    InterfaceTypes,
+    BinaryStream,
+)
 
 async def compress_stringify_async(
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
+    :param input: Input binary
+    :type  input: bytes
 
-    compression_level: int, optional
-        Compression level, typically 1-9
+    :param stringify: Stringify the output
+    :type  stringify: bool
 
-    data_url_prefix: str, optional
-        dataURL prefix
+    :param compression_level: Compression level, typically 1-9
+    :type  compression_level: int
 
+    :param data_url_prefix: dataURL prefix
+    :type  data_url_prefix: str
 
-    Returns
-    -------
-
-    bytes
-        Output compressed binary
-
+    :return: Output compressed binary
+    :rtype:  bytes
     """
     js_module = await js_package.js_module
     web_worker = js_resources.web_worker
 
-    outputs = await js_module.compressStringify(web_worker, to_js(input),  stringify=to_js(stringify), compressionLevel=to_js(compression_level), dataUrlPrefix=to_js(data_url_prefix), )
+    kwargs = {}
+    if stringify:
+        kwargs["stringify"] = to_js(stringify)
+    if compression_level:
+        kwargs["compressionLevel"] = to_js(compression_level)
+    if data_url_prefix:
+        kwargs["dataUrlPrefix"] = to_js(data_url_prefix)
+
+    outputs = await js_module.compressStringify(web_worker, to_js(input), **kwargs)
 
     output_web_worker = None
     output_list = []
     outputs_object_map = outputs.as_object_map()
     for output_name in outputs.object_keys():
         if output_name == 'webWorker':
             output_web_worker = outputs_object_map[output_name]
```

### Comparing `itkwasm_compress_stringify_emscripten-0.4.4/itkwasm_compress_stringify_emscripten/parse_string_decompress_async.py` & `itkwasm_compress_stringify_emscripten-0.4.5/itkwasm_compress_stringify_emscripten/parse_string_decompress_async.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 # Generated file. Do not edit.
 
 from pathlib import Path
 import os
-from typing import Dict, Tuple
+from typing import Dict, Tuple, Optional
 
-from .pyodide import js_package
+from .js_package import js_package
 
 from itkwasm.pyodide import (
     to_js,
     to_py,
     js_resources
 )
+from itkwasm import (
+    InterfaceTypes,
+    BinaryStream,
+)
 
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
+    :param input: Compressed input
+    :type  input: bytes
 
+    :param parse_string: Parse the input string before decompression
+    :type  parse_string: bool
 
-    Returns
-    -------
-
-    bytes
-        Output decompressed binary
-
+    :return: Output decompressed binary
+    :rtype:  bytes
     """
     js_module = await js_package.js_module
     web_worker = js_resources.web_worker
 
-    outputs = await js_module.parseStringDecompress(web_worker, to_js(input),  parseString=to_js(parse_string), )
+    kwargs = {}
+    if parse_string:
+        kwargs["parseString"] = to_js(parse_string)
+
+    outputs = await js_module.parseStringDecompress(web_worker, to_js(input), **kwargs)
 
     output_web_worker = None
     output_list = []
     outputs_object_map = outputs.as_object_map()
     for output_name in outputs.object_keys():
         if output_name == 'webWorker':
             output_web_worker = outputs_object_map[output_name]
```

### Comparing `itkwasm_compress_stringify_emscripten-0.4.4/test/test_compress_stringify.py` & `itkwasm_compress_stringify_emscripten-0.4.5/test/test_compress_stringify.py`

 * *Files identical despite different names*

### Comparing `itkwasm_compress_stringify_emscripten-0.4.4/test/test_itkwasm_compress_stringify.py` & `itkwasm_compress_stringify_emscripten-0.4.5/test/test_itkwasm_compress_stringify.py`

 * *Files identical despite different names*

### Comparing `itkwasm_compress_stringify_emscripten-0.4.4/README.md` & `itkwasm_compress_stringify_emscripten-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `itkwasm_compress_stringify_emscripten-0.4.4/pyproject.toml` & `itkwasm_compress_stringify_emscripten-0.4.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `itkwasm_compress_stringify_emscripten-0.4.4/PKG-INFO` & `itkwasm_compress_stringify_emscripten-0.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: itkwasm-compress-stringify-emscripten
-Version: 0.4.4
+Version: 0.4.5
 License-Expression: Apache-2.0
 Keywords: emscripten,itkwasm,webassembly
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: WebAssembly
 Classifier: Environment :: WebAssembly :: Emscripten
 Classifier: Environment :: WebAssembly :: WASI
 Classifier: Intended Audience :: Developers
```

