# Comparing `tmp/json-schema-codegen-0.6.1.tar.gz` & `tmp/json-schema-codegen-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/json-schema-codegen-0.6.1.tar", last modified: Fri May  8 13:28:42 2020, max compression
+gzip compressed data, was "json-schema-codegen-0.6.3.tar", last modified: Mon May  1 00:32:10 2023, max compression
```

## Comparing `json-schema-codegen-0.6.1.tar` & `json-schema-codegen-0.6.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 jacob     (1000) jacob     (1000)        0 2020-05-08 13:28:42.000000 json-schema-codegen-0.6.1/
--rw-rw-r--   0 jacob     (1000) jacob     (1000)    18091 2020-01-15 19:25:35.000000 json-schema-codegen-0.6.1/LICENSE
--rw-rw-r--   0 jacob     (1000) jacob     (1000)      133 2020-01-15 19:25:35.000000 json-schema-codegen-0.6.1/MANIFEST.in
--rw-rw-r--   0 jacob     (1000) jacob     (1000)     5539 2020-05-08 13:28:42.000000 json-schema-codegen-0.6.1/PKG-INFO
--rw-rw-r--   0 jacob     (1000) jacob     (1000)     3916 2020-01-15 19:25:35.000000 json-schema-codegen-0.6.1/README.md
-drwxrwxr-x   0 jacob     (1000) jacob     (1000)        0 2020-05-08 13:28:42.000000 json-schema-codegen-0.6.1/json_schema_codegen.egg-info/
--rw-rw-r--   0 jacob     (1000) jacob     (1000)     5539 2020-05-08 13:28:39.000000 json-schema-codegen-0.6.1/json_schema_codegen.egg-info/PKG-INFO
--rw-rw-r--   0 jacob     (1000) jacob     (1000)      647 2020-05-08 13:28:39.000000 json-schema-codegen-0.6.1/json_schema_codegen.egg-info/SOURCES.txt
--rw-rw-r--   0 jacob     (1000) jacob     (1000)        1 2020-05-08 13:28:39.000000 json-schema-codegen-0.6.1/json_schema_codegen.egg-info/dependency_links.txt
--rw-rw-r--   0 jacob     (1000) jacob     (1000)        1 2020-05-08 13:28:39.000000 json-schema-codegen-0.6.1/json_schema_codegen.egg-info/not-zip-safe
--rw-rw-r--   0 jacob     (1000) jacob     (1000)       35 2020-05-08 13:28:39.000000 json-schema-codegen-0.6.1/json_schema_codegen.egg-info/requires.txt
--rw-rw-r--   0 jacob     (1000) jacob     (1000)       18 2020-05-08 13:28:39.000000 json-schema-codegen-0.6.1/json_schema_codegen.egg-info/top_level.txt
-drwxrwxr-x   0 jacob     (1000) jacob     (1000)        0 2020-05-08 13:28:42.000000 json-schema-codegen-0.6.1/jsonschemacodegen/
--rw-rw-r--   0 jacob     (1000) jacob     (1000)      104 2020-02-26 05:53:15.000000 json-schema-codegen-0.6.1/jsonschemacodegen/__init__.py
--rw-rw-r--   0 jacob     (1000) jacob     (1000)       94 2020-05-08 13:26:41.000000 json-schema-codegen-0.6.1/jsonschemacodegen/_version.py
--rw-rw-r--   0 jacob     (1000) jacob     (1000)     5913 2020-05-07 17:17:09.000000 json-schema-codegen-0.6.1/jsonschemacodegen/cpp.py
--rw-rw-r--   0 jacob     (1000) jacob     (1000)     2980 2020-04-10 17:53:29.000000 json-schema-codegen-0.6.1/jsonschemacodegen/json_example.py
--rw-rw-r--   0 jacob     (1000) jacob     (1000)     3749 2020-04-17 21:05:36.000000 json-schema-codegen-0.6.1/jsonschemacodegen/python.py
--rw-rw-r--   0 jacob     (1000) jacob     (1000)     5532 2020-05-08 13:26:15.000000 json-schema-codegen-0.6.1/jsonschemacodegen/resolver.py
--rw-rw-r--   0 jacob     (1000) jacob     (1000)    17107 2020-05-07 17:17:09.000000 json-schema-codegen-0.6.1/jsonschemacodegen/schemawrappers.py
-drwxrwxr-x   0 jacob     (1000) jacob     (1000)        0 2020-05-08 13:28:42.000000 json-schema-codegen-0.6.1/jsonschemacodegen/templates/
-drwxrwxr-x   0 jacob     (1000) jacob     (1000)        0 2020-05-08 13:28:42.000000 json-schema-codegen-0.6.1/jsonschemacodegen/templates/cpp/
--rw-rw-r--   0 jacob     (1000) jacob     (1000)        0 2020-01-15 19:25:35.000000 json-schema-codegen-0.6.1/jsonschemacodegen/templates/cpp/__init__.py
-drwxrwxr-x   0 jacob     (1000) jacob     (1000)        0 2020-05-08 13:28:42.000000 json-schema-codegen-0.6.1/jsonschemacodegen/templates/markdown/
--rw-rw-r--   0 jacob     (1000) jacob     (1000)        0 2020-01-15 20:35:40.000000 json-schema-codegen-0.6.1/jsonschemacodegen/templates/markdown/__init__.py
-drwxrwxr-x   0 jacob     (1000) jacob     (1000)        0 2020-05-08 13:28:42.000000 json-schema-codegen-0.6.1/jsonschemacodegen/templates/python/
--rw-rw-r--   0 jacob     (1000) jacob     (1000)        0 2020-01-15 19:25:35.000000 json-schema-codegen-0.6.1/jsonschemacodegen/templates/python/__init__.py
--rw-rw-r--   0 jacob     (1000) jacob     (1000)       38 2020-05-08 13:28:42.000000 json-schema-codegen-0.6.1/setup.cfg
--rw-rw-r--   0 jacob     (1000) jacob     (1000)     1185 2020-02-26 05:53:16.000000 json-schema-codegen-0.6.1/setup.py
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-05-01 00:32:10.210139 json-schema-codegen-0.6.3/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)    18091 2023-05-01 00:29:12.000000 json-schema-codegen-0.6.3/LICENSE
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      133 2023-05-01 00:29:12.000000 json-schema-codegen-0.6.3/MANIFEST.in
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     4278 2023-05-01 00:32:10.210139 json-schema-codegen-0.6.3/PKG-INFO
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     3916 2023-05-01 00:29:12.000000 json-schema-codegen-0.6.3/README.md
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-05-01 00:32:10.210139 json-schema-codegen-0.6.3/json_schema_codegen.egg-info/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     4278 2023-05-01 00:32:10.000000 json-schema-codegen-0.6.3/json_schema_codegen.egg-info/PKG-INFO
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      647 2023-05-01 00:32:10.000000 json-schema-codegen-0.6.3/json_schema_codegen.egg-info/SOURCES.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)        1 2023-05-01 00:32:10.000000 json-schema-codegen-0.6.3/json_schema_codegen.egg-info/dependency_links.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)        1 2023-05-01 00:32:10.000000 json-schema-codegen-0.6.3/json_schema_codegen.egg-info/not-zip-safe
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       35 2023-05-01 00:32:10.000000 json-schema-codegen-0.6.3/json_schema_codegen.egg-info/requires.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       18 2023-05-01 00:32:10.000000 json-schema-codegen-0.6.3/json_schema_codegen.egg-info/top_level.txt
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-05-01 00:32:10.210139 json-schema-codegen-0.6.3/jsonschemacodegen/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      104 2023-05-01 00:29:12.000000 json-schema-codegen-0.6.3/jsonschemacodegen/__init__.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       94 2023-05-01 00:30:47.000000 json-schema-codegen-0.6.3/jsonschemacodegen/_version.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     5913 2023-05-01 00:29:12.000000 json-schema-codegen-0.6.3/jsonschemacodegen/cpp.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2980 2023-05-01 00:29:12.000000 json-schema-codegen-0.6.3/jsonschemacodegen/json_example.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     3749 2023-05-01 00:29:12.000000 json-schema-codegen-0.6.3/jsonschemacodegen/python.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     5532 2023-05-01 00:29:12.000000 json-schema-codegen-0.6.3/jsonschemacodegen/resolver.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)    18169 2023-05-01 00:29:12.000000 json-schema-codegen-0.6.3/jsonschemacodegen/schemawrappers.py
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-05-01 00:32:10.210139 json-schema-codegen-0.6.3/jsonschemacodegen/templates/
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-05-01 00:32:10.210139 json-schema-codegen-0.6.3/jsonschemacodegen/templates/cpp/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)        0 2023-05-01 00:29:12.000000 json-schema-codegen-0.6.3/jsonschemacodegen/templates/cpp/__init__.py
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-05-01 00:32:10.210139 json-schema-codegen-0.6.3/jsonschemacodegen/templates/markdown/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)        0 2023-05-01 00:29:12.000000 json-schema-codegen-0.6.3/jsonschemacodegen/templates/markdown/__init__.py
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-05-01 00:32:10.210139 json-schema-codegen-0.6.3/jsonschemacodegen/templates/python/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)        0 2023-05-01 00:29:12.000000 json-schema-codegen-0.6.3/jsonschemacodegen/templates/python/__init__.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       38 2023-05-01 00:32:10.210139 json-schema-codegen-0.6.3/setup.cfg
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1185 2023-05-01 00:29:12.000000 json-schema-codegen-0.6.3/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `json-schema-codegen-0.6.1/LICENSE` & `json-schema-codegen-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `json-schema-codegen-0.6.1/PKG-INFO` & `json-schema-codegen-0.6.3/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,171 +1,159 @@
-Metadata-Version: 2.1
-Name: json-schema-codegen
-Version: 0.6.1
-Summary: Generate C++ or Python structures from JSON-Schema
-Home-page: http://github.com/pearmaster/json-schema-codegen
-Author: Jacob Brunson
-Author-email: pypi@jacobbrunson.com
-License: GPLv2
-Description: # JSON-Schema Codegen
-        
-        This python library consumes JSON-Schema and generates C++ or Python code.  It generates structures to hold the values defined in the schema, restricting the values according to the schema. 
-        
-        ## Python Requirements for Code Generation
-        
-        These requirements should be satisfied when `pip3` installing `json-schema-codegen`.
-        
-        * python 3.7
-        * jinja2
-        * stringcase
-        
-        ## Installation
-        
-        ```sh
-        pip3 install json-schema-codegen
-        ```
-        
-        ## C++ Generated Code
-        
-        ### Supported Schema Features in C++ code generation
-        
-        A C++ class is generated for each schema node according to the schema's `type` property.  Schemas without a `type` property, with the exception of combining operators `*Of`, are not supported.
-        
-        * type: string
-            * minLength
-            * maxLength
-            * pattern
-            * format=date-time (enforces ISO8601 format)
-            * format=uuid (enables string object to be populated with a uuid)
-        * type: string with enum
-        * type: integer
-            * maximum
-            * minimum
-            * exclusiveMaximum
-            * exclusiveMinimum
-            * multipleOf
-        * type: number
-            * maximum
-            * minimum
-            * exclusiveMaximum
-            * exclusiveMinimum
-            * multipleOf 
-        * type: boolean
-        * type: null
-        * type: array
-            * items
-            * minItems
-            * maxItems
-        * type: object
-            * properties
-            * required
-        * allOf
-        * anyOf
-        * oneOf
-        
-        ##### References
-        
-        `$ref` references are supported for array items, object properties, allOf, anyOf, and oneOf.  However, the caller must provide a "resolver" class which translates the reference into a class name and namespace. 
-        
-        ### Dependencies of the C++ generated code
-        
-        * boost (boost::optional and boost::variant among others)
-        * rapidjson 1.1
-        * C++11
-        
-        ### Usage
-        See [example_usage.py](./examples/example_usage.py) for a more elaborate example on generating C++ code.
-        
-        ```py
-        import jsonschemacodegen.cpp as cpp
-        
-        simpleResolver = cpp.SimpleResolver()
-        output_dir = "/tmp"
-            
-        generator = cpp.GeneratorFromSchema(src_output_dir=output_dir,
-            header_output_dir=output_dir, 
-            resolver=simpleResolver,
-            namespace=[],
-            src_usings=[])
-        
-        sampleSchema = {"type": "string"}
-        
-        generator.Generate(sampleSchema, 'Example', 'example')
-        ```
-        
-        ## Python Generated Code
-        
-        A Python3 class is generated for each schema node; the class encapsulating the data described by the schema.  The class accepts in its constructor python primative data types that match the format described the the schema.  Each class has a `Serializable` method which returns data in a format that can be serialized.
-        
-        JSON (de-)serialization does not happen in the actual class.  This allows for flexibility to use other line-formats, for example, YAML.
-        
-        ### Supported schema features for generating Python code
-        
-        * type: string
-            * minLength
-            * maxLength
-            * pattern
-            * enum
-        * type: integer
-            * maximum
-            * minimum
-            * exclusiveMaximum
-            * exclusiveMinimum
-            * multipleOf
-            * enum
-        * type: number
-            * maximum
-            * minimum
-            * exclusiveMaximum
-            * exclusiveMinimum
-            * multipleOf 
-            * enum
-        * type: boolean
-        * type: null
-        * type: array
-            * items
-            * minItems
-            * maxItems
-        * type: object
-            * properties
-            * required
-        * allOf
-        * anyOf
-        * oneOf
-            * Component schemas with the `title` property.
-        
-        ### Example usage for generating Python code
-        
-        For a more elaborate example, see [example_python.py](./examples/example_python.py)
-        
-        ```py
-        from jsonschemacodegen import python as pygen
-        import json
-        
-        with open('schema.json') as fp:
-            generator = pygen.GeneratorFromSchema('output_dir')
-            generator.Generate(json.load(fp), 'Example', 'example')
-        ```
-        
-        This example will create the file `output_dir/example.py` containing the Python3 class `Example` and nested classes as required.
-        
-        Using the generated code looks like this:
-        ```py
-        import example
-        import json
-        
-        jsonText = '["an example string in an array"]'
-        
-        obj = example.Example(json.loads(jsonText))
-        
-        print(json.dumps(obj, default=lambda x: x.Serializable()))
-        ```
-        
-        ## License
-        
-        GPLv2
-        
-        
-        
-Platform: UNKNOWN
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
+# JSON-Schema Codegen
+
+This python library consumes JSON-Schema and generates C++ or Python code.  It generates structures to hold the values defined in the schema, restricting the values according to the schema. 
+
+## Python Requirements for Code Generation
+
+These requirements should be satisfied when `pip3` installing `json-schema-codegen`.
+
+* python 3.7
+* jinja2
+* stringcase
+
+## Installation
+
+```sh
+pip3 install json-schema-codegen
+```
+
+## C++ Generated Code
+
+### Supported Schema Features in C++ code generation
+
+A C++ class is generated for each schema node according to the schema's `type` property.  Schemas without a `type` property, with the exception of combining operators `*Of`, are not supported.
+
+* type: string
+    * minLength
+    * maxLength
+    * pattern
+    * format=date-time (enforces ISO8601 format)
+    * format=uuid (enables string object to be populated with a uuid)
+* type: string with enum
+* type: integer
+    * maximum
+    * minimum
+    * exclusiveMaximum
+    * exclusiveMinimum
+    * multipleOf
+* type: number
+    * maximum
+    * minimum
+    * exclusiveMaximum
+    * exclusiveMinimum
+    * multipleOf 
+* type: boolean
+* type: null
+* type: array
+    * items
+    * minItems
+    * maxItems
+* type: object
+    * properties
+    * required
+* allOf
+* anyOf
+* oneOf
+
+##### References
+
+`$ref` references are supported for array items, object properties, allOf, anyOf, and oneOf.  However, the caller must provide a "resolver" class which translates the reference into a class name and namespace. 
+
+### Dependencies of the C++ generated code
+
+* boost (boost::optional and boost::variant among others)
+* rapidjson 1.1
+* C++11
+
+### Usage
+See [example_usage.py](./examples/example_usage.py) for a more elaborate example on generating C++ code.
+
+```py
+import jsonschemacodegen.cpp as cpp
+
+simpleResolver = cpp.SimpleResolver()
+output_dir = "/tmp"
+    
+generator = cpp.GeneratorFromSchema(src_output_dir=output_dir,
+    header_output_dir=output_dir, 
+    resolver=simpleResolver,
+    namespace=[],
+    src_usings=[])
+
+sampleSchema = {"type": "string"}
+
+generator.Generate(sampleSchema, 'Example', 'example')
+```
+
+## Python Generated Code
+
+A Python3 class is generated for each schema node; the class encapsulating the data described by the schema.  The class accepts in its constructor python primative data types that match the format described the the schema.  Each class has a `Serializable` method which returns data in a format that can be serialized.
+
+JSON (de-)serialization does not happen in the actual class.  This allows for flexibility to use other line-formats, for example, YAML.
+
+### Supported schema features for generating Python code
+
+* type: string
+    * minLength
+    * maxLength
+    * pattern
+    * enum
+* type: integer
+    * maximum
+    * minimum
+    * exclusiveMaximum
+    * exclusiveMinimum
+    * multipleOf
+    * enum
+* type: number
+    * maximum
+    * minimum
+    * exclusiveMaximum
+    * exclusiveMinimum
+    * multipleOf 
+    * enum
+* type: boolean
+* type: null
+* type: array
+    * items
+    * minItems
+    * maxItems
+* type: object
+    * properties
+    * required
+* allOf
+* anyOf
+* oneOf
+    * Component schemas with the `title` property.
+
+### Example usage for generating Python code
+
+For a more elaborate example, see [example_python.py](./examples/example_python.py)
+
+```py
+from jsonschemacodegen import python as pygen
+import json
+
+with open('schema.json') as fp:
+    generator = pygen.GeneratorFromSchema('output_dir')
+    generator.Generate(json.load(fp), 'Example', 'example')
+```
+
+This example will create the file `output_dir/example.py` containing the Python3 class `Example` and nested classes as required.
+
+Using the generated code looks like this:
+```py
+import example
+import json
+
+jsonText = '["an example string in an array"]'
+
+obj = example.Example(json.loads(jsonText))
+
+print(json.dumps(obj, default=lambda x: x.Serializable()))
+```
+
+## License
+
+GPLv2
+
+
```

### Comparing `json-schema-codegen-0.6.1/README.md` & `json-schema-codegen-0.6.3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: json-schema-codegen
+Version: 0.6.3
+Summary: Generate C++ or Python structures from JSON-Schema
+Home-page: http://github.com/pearmaster/json-schema-codegen
+Author: Jacob Brunson
+Author-email: pypi@jacobbrunson.com
+License: GPLv2
+Platform: UNKNOWN
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # JSON-Schema Codegen
 
 This python library consumes JSON-Schema and generates C++ or Python code.  It generates structures to hold the values defined in the schema, restricting the values according to the schema. 
 
 ## Python Requirements for Code Generation
 
 These requirements should be satisfied when `pip3` installing `json-schema-codegen`.
@@ -153,7 +166,9 @@
 ```
 
 ## License
 
 GPLv2
 
 
+
+
```

### Comparing `json-schema-codegen-0.6.1/json_schema_codegen.egg-info/SOURCES.txt` & `json-schema-codegen-0.6.3/json_schema_codegen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `json-schema-codegen-0.6.1/jsonschemacodegen/cpp.py` & `json-schema-codegen-0.6.3/jsonschemacodegen/cpp.py`

 * *Files identical despite different names*

### Comparing `json-schema-codegen-0.6.1/jsonschemacodegen/json_example.py` & `json-schema-codegen-0.6.3/jsonschemacodegen/json_example.py`

 * *Files identical despite different names*

### Comparing `json-schema-codegen-0.6.1/jsonschemacodegen/python.py` & `json-schema-codegen-0.6.3/jsonschemacodegen/python.py`

 * *Files identical despite different names*

### Comparing `json-schema-codegen-0.6.1/jsonschemacodegen/resolver.py` & `json-schema-codegen-0.6.3/jsonschemacodegen/resolver.py`

 * *Files identical despite different names*

### Comparing `json-schema-codegen-0.6.1/jsonschemacodegen/schemawrappers.py` & `json-schema-codegen-0.6.3/jsonschemacodegen/schemawrappers.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import collections
 import random
+from copy import deepcopy
 
 def bitsNeededForNumber(num):
     bits = 0
     while num > 0:
         num = num >> 1
         bits += 1
     return bits
@@ -287,14 +288,23 @@
         return incs
 
     def AnExample(self, resolver, index: ExampleIndex):
         return None
 
 class ArraySchema(SchemaBase):
     
+    def IsTupleSchema(self):
+        return isinstance(self.data["items"], list)
+
+    def NumberTupleItems(self):
+        return len(self.data["items"])
+
+    def GetTupleSchema(self):
+        return [ SchemaFactory(x, self.root) for x in self.data['items'] ]
+
     def GetItemSchema(self):
         return SchemaFactory(self.data['items'], self.root)
 
     def CppIncludes(self, resolver=None):
         incs = super().CppIncludes(resolver=resolver)
         incs.update({"<vector>", "<string>"})
         incs.update(self.GetItemSchema().CppIncludes(resolver))
@@ -439,15 +449,32 @@
                 gotOne = True
                 ret.update(comp.Example(resolver, index, self.requiredProperties))
         if not gotOne:
             comp = index.Choice(self.GetComponents())
             ret.update(comp.Example(resolver, index, self.requiredProperties))
         return ret
 
+class AlwaysValidSchema(collections.UserDict):
+
+    def __init__(self, always:bool, root=None):
+        super().__init__()
+        self.always_valid = always
+        self.root = root
+
+    def Resolve(self, resolver):
+        return self
+
+    def Example(self, resolver, index: ExampleIndex, required=None):
+        pass
+
 def SchemaFactory(schema, root=None):
+    if isinstance(schema, bool):
+        return AlwaysValidSchema(schema, root)
+    elif isinstance(schema, AlwaysValidSchema):
+        return schema
     if 'type' in schema:
         if schema['type'] == 'string':
             if 'enum' in schema:
                 return StringEnumSchema(schema, root)
             return StringSchema(schema, root)
         elif schema['type'] == 'number' or schema['type'] == 'integer':
             return NumberSchema(schema, root)
@@ -455,14 +482,21 @@
             return BooleanSchema(schema, root)
         elif schema['type'] == 'null':
             return NullSchema(schema, root)
         elif schema['type'] == 'object':
             return ObjectSchema(schema, root)
         elif schema['type'] == 'array':
             return ArraySchema(schema, root)
+        elif isinstance(schema['type'], list):
+            allOfSchema = []
+            for t in schema["type"]:
+                new_schema = deepcopy(schema)
+                new_schema["type"] = t
+                allOfSchema.append(new_schema)
+            return OneOfSchema({"oneOf":allOfSchema}, root)
         else:
             raise NotImplementedError(f"The type '{schema['type']}' is not implemented")
     elif 'allOf' in schema:
         return AllOfSchema(schema, root)
     elif 'anyOf' in schema:
         return AnyOfSchema(schema, root)
     elif 'oneOf' in schema:
```

### Comparing `json-schema-codegen-0.6.1/setup.py` & `json-schema-codegen-0.6.3/setup.py`

 * *Files identical despite different names*

