# Comparing `tmp/asyncapi-codegen-0.4.1.tar.gz` & `tmp/asyncapi-codegen-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/asyncapi-codegen-0.4.1.tar", last modified: Fri May  8 13:32:18 2020, max compression
+gzip compressed data, was "asyncapi-codegen-0.5.0.tar", last modified: Mon May  1 00:38:20 2023, max compression
```

## Comparing `asyncapi-codegen-0.4.1.tar` & `asyncapi-codegen-0.5.0.tar`

### file list

```diff
@@ -1,27 +1,46 @@
-drwxrwxr-x   0 jacob     (1000) jacob     (1000)        0 2020-05-08 13:32:18.000000 asyncapi-codegen-0.4.1/
--rw-rw-r--   0 jacob     (1000) jacob     (1000)     2738 2020-05-08 13:32:18.000000 asyncapi-codegen-0.4.1/PKG-INFO
--rw-rw-r--   0 jacob     (1000) jacob     (1000)     1962 2020-02-26 05:53:59.000000 asyncapi-codegen-0.4.1/README.md
-drwxrwxr-x   0 jacob     (1000) jacob     (1000)        0 2020-05-08 13:32:18.000000 asyncapi-codegen-0.4.1/asyncapi_codegen.egg-info/
--rw-rw-r--   0 jacob     (1000) jacob     (1000)     2738 2020-05-08 13:32:18.000000 asyncapi-codegen-0.4.1/asyncapi_codegen.egg-info/PKG-INFO
--rw-rw-r--   0 jacob     (1000) jacob     (1000)      603 2020-05-08 13:32:18.000000 asyncapi-codegen-0.4.1/asyncapi_codegen.egg-info/SOURCES.txt
--rw-rw-r--   0 jacob     (1000) jacob     (1000)        1 2020-05-08 13:32:18.000000 asyncapi-codegen-0.4.1/asyncapi_codegen.egg-info/dependency_links.txt
--rw-rw-r--   0 jacob     (1000) jacob     (1000)        1 2020-05-08 13:32:18.000000 asyncapi-codegen-0.4.1/asyncapi_codegen.egg-info/not-zip-safe
--rw-rw-r--   0 jacob     (1000) jacob     (1000)       81 2020-05-08 13:32:18.000000 asyncapi-codegen-0.4.1/asyncapi_codegen.egg-info/requires.txt
--rw-rw-r--   0 jacob     (1000) jacob     (1000)       16 2020-05-08 13:32:18.000000 asyncapi-codegen-0.4.1/asyncapi_codegen.egg-info/top_level.txt
-drwxrwxr-x   0 jacob     (1000) jacob     (1000)        0 2020-05-08 13:32:18.000000 asyncapi-codegen-0.4.1/asyncapicodegen/
--rw-rw-r--   0 jacob     (1000) jacob     (1000)      103 2020-02-26 05:53:59.000000 asyncapi-codegen-0.4.1/asyncapicodegen/__init__.py
--rw-rw-r--   0 jacob     (1000) jacob     (1000)       95 2020-05-08 13:30:57.000000 asyncapi-codegen-0.4.1/asyncapicodegen/_version.py
--rw-rw-r--   0 jacob     (1000) jacob     (1000)     6242 2020-04-09 05:06:09.000000 asyncapi-codegen-0.4.1/asyncapicodegen/cpp.py
--rw-rw-r--   0 jacob     (1000) jacob     (1000)      880 2020-04-09 05:08:10.000000 asyncapi-codegen-0.4.1/asyncapicodegen/markdown_summary.py
--rw-rw-r--   0 jacob     (1000) jacob     (1000)     3238 2020-05-08 13:25:41.000000 asyncapi-codegen-0.4.1/asyncapicodegen/python_client.py
--rw-rw-r--   0 jacob     (1000) jacob     (1000)     2850 2020-04-17 21:05:50.000000 asyncapi-codegen-0.4.1/asyncapicodegen/python_summary.py
--rw-rw-r--   0 jacob     (1000) jacob     (1000)    16540 2020-05-08 13:25:41.000000 asyncapi-codegen-0.4.1/asyncapicodegen/specwrapper.py
-drwxrwxr-x   0 jacob     (1000) jacob     (1000)        0 2020-05-08 13:32:18.000000 asyncapi-codegen-0.4.1/asyncapicodegen/templates/
-drwxrwxr-x   0 jacob     (1000) jacob     (1000)        0 2020-05-08 13:32:18.000000 asyncapi-codegen-0.4.1/asyncapicodegen/templates/cpp/
--rw-rw-r--   0 jacob     (1000) jacob     (1000)        0 2020-01-15 19:25:54.000000 asyncapi-codegen-0.4.1/asyncapicodegen/templates/cpp/__init__.py
-drwxrwxr-x   0 jacob     (1000) jacob     (1000)        0 2020-05-08 13:32:18.000000 asyncapi-codegen-0.4.1/asyncapicodegen/templates/markdown/
--rw-rw-r--   0 jacob     (1000) jacob     (1000)        0 2020-01-15 19:25:54.000000 asyncapi-codegen-0.4.1/asyncapicodegen/templates/markdown/__init__.py
-drwxrwxr-x   0 jacob     (1000) jacob     (1000)        0 2020-05-08 13:32:18.000000 asyncapi-codegen-0.4.1/asyncapicodegen/templates/python/
--rw-rw-r--   0 jacob     (1000) jacob     (1000)        0 2020-01-15 19:25:54.000000 asyncapi-codegen-0.4.1/asyncapicodegen/templates/python/__init__.py
--rw-rw-r--   0 jacob     (1000) jacob     (1000)       38 2020-05-08 13:32:18.000000 asyncapi-codegen-0.4.1/setup.cfg
--rw-rw-r--   0 jacob     (1000) jacob     (1000)     1147 2020-05-08 04:25:48.000000 asyncapi-codegen-0.4.1/setup.py
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-05-01 00:38:20.391116 asyncapi-codegen-0.5.0/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)    18091 2023-05-01 00:37:56.000000 asyncapi-codegen-0.5.0/LICENSE
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     4867 2023-05-01 00:38:20.391116 asyncapi-codegen-0.5.0/PKG-INFO
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     4540 2023-05-01 00:37:56.000000 asyncapi-codegen-0.5.0/README.md
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-05-01 00:38:20.359116 asyncapi-codegen-0.5.0/asyncapi_codegen.egg-info/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     4867 2023-05-01 00:38:20.000000 asyncapi-codegen-0.5.0/asyncapi_codegen.egg-info/PKG-INFO
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1453 2023-05-01 00:38:20.000000 asyncapi-codegen-0.5.0/asyncapi_codegen.egg-info/SOURCES.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)        1 2023-05-01 00:38:20.000000 asyncapi-codegen-0.5.0/asyncapi_codegen.egg-info/dependency_links.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)        1 2023-05-01 00:38:03.000000 asyncapi-codegen-0.5.0/asyncapi_codegen.egg-info/not-zip-safe
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       81 2023-05-01 00:38:20.000000 asyncapi-codegen-0.5.0/asyncapi_codegen.egg-info/requires.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       16 2023-05-01 00:38:20.000000 asyncapi-codegen-0.5.0/asyncapi_codegen.egg-info/top_level.txt
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-05-01 00:38:20.363116 asyncapi-codegen-0.5.0/asyncapicodegen/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      103 2023-05-01 00:37:56.000000 asyncapi-codegen-0.5.0/asyncapicodegen/__init__.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       95 2023-05-01 00:37:56.000000 asyncapi-codegen-0.5.0/asyncapicodegen/_version.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     6718 2023-05-01 00:37:56.000000 asyncapi-codegen-0.5.0/asyncapicodegen/cpp.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      880 2023-05-01 00:37:56.000000 asyncapi-codegen-0.5.0/asyncapicodegen/markdown_summary.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     3191 2023-05-01 00:37:56.000000 asyncapi-codegen-0.5.0/asyncapicodegen/python_client.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2850 2023-05-01 00:37:56.000000 asyncapi-codegen-0.5.0/asyncapicodegen/python_summary.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)    17607 2023-05-01 00:37:56.000000 asyncapi-codegen-0.5.0/asyncapicodegen/specwrapper.py
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-05-01 00:38:20.359116 asyncapi-codegen-0.5.0/asyncapicodegen/templates/
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-05-01 00:38:20.363116 asyncapi-codegen-0.5.0/asyncapicodegen/templates/cpp/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)        0 2023-05-01 00:37:56.000000 asyncapi-codegen-0.5.0/asyncapicodegen/templates/cpp/__init__.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     8855 2023-05-01 00:37:56.000000 asyncapi-codegen-0.5.0/asyncapicodegen/templates/cpp/broker.cpp.jinja2
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     5542 2023-05-01 00:37:56.000000 asyncapi-codegen-0.5.0/asyncapicodegen/templates/cpp/broker.hpp.jinja2
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      367 2023-05-01 00:37:56.000000 asyncapi-codegen-0.5.0/asyncapicodegen/templates/cpp/file_prologue.jinja2
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     8394 2023-05-01 00:37:56.000000 asyncapi-codegen-0.5.0/asyncapicodegen/templates/cpp/header.hpp.jinja2
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1106 2023-05-01 00:37:56.000000 asyncapi-codegen-0.5.0/asyncapicodegen/templates/cpp/ibrokerconnection.hpp.jinja2
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      549 2023-05-01 00:37:56.000000 asyncapi-codegen-0.5.0/asyncapicodegen/templates/cpp/message.hpp.jinja2
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)    11220 2023-05-01 00:37:56.000000 asyncapi-codegen-0.5.0/asyncapicodegen/templates/cpp/source.cpp.jinja2
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      733 2023-05-01 00:37:56.000000 asyncapi-codegen-0.5.0/asyncapicodegen/templates/cpp/type_helpers.jinja2
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-05-01 00:38:20.391116 asyncapi-codegen-0.5.0/asyncapicodegen/templates/markdown/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)        0 2023-05-01 00:37:56.000000 asyncapi-codegen-0.5.0/asyncapicodegen/templates/markdown/__init__.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      164 2023-05-01 00:37:56.000000 asyncapi-codegen-0.5.0/asyncapicodegen/templates/markdown/examples.md.jinja2
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      458 2023-05-01 00:37:56.000000 asyncapi-codegen-0.5.0/asyncapicodegen/templates/markdown/operation_list.md.jinja2
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      452 2023-05-01 00:37:56.000000 asyncapi-codegen-0.5.0/asyncapicodegen/templates/markdown/payload.md.jinja2
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     3218 2023-05-01 00:37:56.000000 asyncapi-codegen-0.5.0/asyncapicodegen/templates/markdown/summary.md.jinja2
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      152 2023-05-01 00:37:56.000000 asyncapi-codegen-0.5.0/asyncapicodegen/templates/markdown/tags.md.jinja2
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-05-01 00:38:20.391116 asyncapi-codegen-0.5.0/asyncapicodegen/templates/python/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)        0 2023-05-01 00:37:56.000000 asyncapi-codegen-0.5.0/asyncapicodegen/templates/python/__init__.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     6446 2023-05-01 00:37:56.000000 asyncapi-codegen-0.5.0/asyncapicodegen/templates/python/client.py.jinja2
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      873 2023-05-01 00:37:56.000000 asyncapi-codegen-0.5.0/asyncapicodegen/templates/python/setup.py.jinja2
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      920 2023-05-01 00:37:56.000000 asyncapi-codegen-0.5.0/asyncapicodegen/templates/python/summary.py.jinja2
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-05-01 00:38:20.391116 asyncapi-codegen-0.5.0/bin/
+-rwxr-xr-x   0 gitpod   (33333) gitpod   (33333)     4466 2023-05-01 00:37:56.000000 asyncapi-codegen-0.5.0/bin/asyncapi-codegen
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       38 2023-05-01 00:38:20.391116 asyncapi-codegen-0.5.0/setup.cfg
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1205 2023-05-01 00:37:56.000000 asyncapi-codegen-0.5.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `asyncapi-codegen-0.4.1/asyncapicodegen/cpp.py` & `asyncapi-codegen-0.5.0/asyncapicodegen/cpp.py`

 * *Files 24% similar despite different names*

```diff
@@ -15,17 +15,25 @@
         self.hpp = []
         if cppFile is not None:
             self.cpp.append(cppFile)
         if hppFile is not None:
             self.hpp.append(hppFile)
 
     def __iadd__(self, other):
-        assert(isinstance(other, type(self)))
-        self.cpp.extend(other.cpp)
-        self.hpp.extend(other.hpp)
+        assert(isinstance(other, type(self)) or len(other) == 2)
+        if isinstance(other, type(self)):
+            self.cpp.extend(other.cpp)
+            self.hpp.extend(other.hpp)
+        elif len(other) == 2:
+            if other[0] is not None:
+                self.cpp.append(other[0])
+            if other[1] is not None:
+                self.hpp.append(other[1])
+        else:
+            raise "Runtime error"
         return self
 
 
 class ResolverBaseClass(jsonschemacodegen.cpp.ResolverBaseClass):
     
     @abc.abstractmethod
     def cpp_get_client_filename_base(self, spec, uri):
@@ -64,14 +72,15 @@
 
         self.srcGenerator = templator.CodeTemplator(self.output_dir['src'])
         self.srcGenerator.add_template_package('asyncapicodegen.templates.cpp')
         self.srcGenerator.add_template_package('jsonschemacodegen.templates.cpp')
         self.headerGenerator = templator.CodeTemplator(self.output_dir['header'])
         self.headerGenerator.add_template_package('asyncapicodegen.templates.cpp')
         self.headerGenerator.add_template_package('jsonschemacodegen.templates.cpp')
+        self.library_generator = jsonschemacodegen.cpp.LibraryGenerator(src_output_dir, header_output_dir, resolver)
 
     def GenerateSchemasForType(self, spec, url, itemType, getSchemaFunc):
         assert(isinstance(spec, specwrapper.SpecRoot))
         genFiles = GeneratedFiles()
         pathBase = "%s#/components/%s/%s"
         if 'components' not in spec or itemType not in spec['components']:
             return genFiles
@@ -144,8 +153,9 @@
             ns=self.namespace,
             resolver=self.resolver,
             Name=class_name,
             codegenVersion=_version.__version__,
             codegenDate=datetime.datetime.now().strftime("%c"),
             spec=wrappedSpec)
         genFiles += GeneratedFiles(hppFile=headerFilename)
+        genFiles += self.library_generator.Generate()
         return genFiles
```

### Comparing `asyncapi-codegen-0.4.1/asyncapicodegen/markdown_summary.py` & `asyncapi-codegen-0.5.0/asyncapicodegen/markdown_summary.py`

 * *Files identical despite different names*

### Comparing `asyncapi-codegen-0.4.1/asyncapicodegen/python_client.py` & `asyncapi-codegen-0.5.0/asyncapicodegen/python_client.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import yaml
 
 from jacobsjinjatoo import templator
 from . import specwrapper
 from . import python_summary
 import jsonschemacodegen.python
 import jsonschemacodegen.resolver
+import os.path
 
 
 class SimpleResolver(python_summary.SimpleResolver):
     pass
 
 
 class PackageResolver(SimpleResolver):
@@ -38,14 +39,19 @@
 
     def py_client_filepath(self, client_type, filename):
         return filename
 
     def py_package_name(self):
         return "asyncapi-client"
 
+    def py_test_filename(self, reference):
+        simple_filename = super().py_test_filename(reference)
+        return os.path.join(f"tests", simple_filename)
+
+
 class GeneratorFromAsyncApi(python_summary.GeneratorFromAsyncApi):
 
     def Generate(self, spec, class_name, filename_base):
         assert(isinstance(spec, dict))
         wrappedSpec = specwrapper.SpecRoot(spec, self.resolver, class_name)
 
         self.GenerateSchemasForType(wrappedSpec, 'messages', lambda obj: obj['payload'])
@@ -62,17 +68,14 @@
                     Name = "{}{}".format(stringcase.pascalcase(class_name), stringcase.pascalcase(clientType)),
                     spec = wrappedSpec,
                     resolver=self.resolver)
     
     def GenerateSetup(self, spec, class_name):
         assert(isinstance(spec, dict))
         wrappedSpec = specwrapper.SpecRoot(spec, self.resolver)
-        clientType = 'x-client-role' in wrappedSpec and wrappedSpec['x-client-role'] or 'client'
-        print(f"Generating setup for {clientType}")
-        if clientType in ['provider', 'utilizer', 'library']:
-            self.generator.render_template(template_name="setup.py.jinja2", 
-                    output_name="setup.py", 
-                    Name = "{}".format(stringcase.pascalcase(class_name)),
-                    spec = wrappedSpec,
-                    resolver=self.resolver)
+        return self.generator.render_template(template_name="setup.py.jinja2", 
+                output_name="setup.py", 
+                Name = "{}".format(stringcase.pascalcase(class_name)),
+                spec = wrappedSpec,
+                resolver=self.resolver)
```

### Comparing `asyncapi-codegen-0.4.1/asyncapicodegen/python_summary.py` & `asyncapi-codegen-0.5.0/asyncapicodegen/python_summary.py`

 * *Files identical despite different names*

### Comparing `asyncapi-codegen-0.4.1/asyncapicodegen/specwrapper.py` & `asyncapi-codegen-0.5.0/asyncapicodegen/specwrapper.py`

 * *Files 6% similar despite different names*

```diff
@@ -64,23 +64,43 @@
                 schema = resolver.get_schema(schema['$ref'], hasattr(sch, 'root') and sch.root or root)
             if 'enum' in schema:
                 return " OR ".join([f'"{e}"' for e in schema['enum']])
             if 'type' in schema:
                 return "{}{}".format(schema['type'], 'title' in schema and f" - {schema['title']}" or '')
             if 'oneOf' in schema:
                 try:
-                    alternatives = set([GetEnglishTypeForSchema(root, resolver, s) for s in schema['oneOf']])
+                    alternatives = []
+                    for s in schema.GetComponents():
+                        english_type = GetEnglishTypeForSchema(root, resolver, s)
+                        if english_type not in alternatives:
+                            alternatives.append(english_type)
+                except:
+                    return ""
+                return " OR ".join([ f"[{a}]" for a in alternatives])
+            if 'anyOf' in schema:
+                try:
+                    alternatives = []
+                    for s in schema.GetComponents():
+                        english_type = GetEnglishTypeForSchema(root, resolver, s)
+                        if english_type not in alternatives:
+                            alternatives.append(english_type)
                 except:
                     return ""
                 return " OR ".join([ f"[{a}]" for a in alternatives])
             return schema
         
         engType = GetEnglishTypeForSchema(self.root, resolver, thedata['schema'])
         return engType
 
+    def Resolve(self):
+        instance = self
+        while '$ref' in instance.data:
+            instance = self.root.Resolve(instance.data['$ref'], Parameter, name=self.name)
+        return instance
+
     def __hash__(self):
         if '$ref' in self.data:
             return hash(self.data['$ref'])
         else:
             return 1
 
     def __eq__(self, other):
@@ -211,15 +231,15 @@
             return f"%{repl.i}%"
         repl.i = 0
         return re.sub(pattern, repl, self.channelPath)
 
     def GetPathParameters(self):
         pattern = r"\{\w+\}"
         results = re.findall(pattern, self.channelPath)
-        assert(len(results) == len(self.Parameters())), f"Mismatch of parameters from {self.GetName()}"
+        assert(len(results) == len(self.Parameters())), f"Mismatch of parameters from {self.GetName()}.  The path indicated {len(results)}, but we only found {len(self.Parameters())} parameters defined.  {self}"
         return results
 
     def GetSubscribePath(self):
         pattern = r"\{\w+\}"
         return re.sub(pattern, '+', self.channelPath)
 
     def GetPathParts(self):
@@ -303,21 +323,14 @@
 
     def TryGetBinding(self, name):
         try:
             return self.data['bindings'][self.data['protocol']][name]
         except:
             return None
 
-    def IDontKnowWhatThisDeadCodeIs(self):
-        if 'security' in self.data:
-            for schemeName in self.data['security'].keys():
-                scheme = self.root['components']['securitySchemes'][schemeName]
-                if scheme['type'] != 'userPassword':
-                    raise NotImplementedError
-
     def AcceptsUsernamePassword(self):
         if 'security' in self.data:
             for securityDef in self.data['security']:
                 for schemeName, schemeDetails in securityDef.items():
                     scheme = self.root['components']['securitySchemes'][schemeName]
                     if scheme['type'] == 'userPassword':
                         return True
@@ -407,16 +420,16 @@
 class SpecRoot(BaseDict):
     
     def __init__(self, initialdata, resolver=None, name=None):
         super().__init__(self, initialdata)
         self.resolver = resolver
         self.name = name
 
-        if self.data['asyncapi'] != '2.0.0':
-            raise NotImplementedError
+        if not self.data['asyncapi'].startswith('2'):
+            raise NotImplementedError(f"The AsyncAPI version {self.data['asyncapi']} is not supported")
 
         if 'channels' in self.data:
             self.data['channels'] = Channels(self, self.data['channels'])
 
         if 'components' in self.data:
             self.data['components'] = Components(self, self.data['components'])
 
@@ -435,26 +448,29 @@
         else:
             return self.resolver.get_schema(ref, root=otherRoot)
 
     def __repr__(self):
         return f"Spec<{self.name}>"
 
 def invert_spec(initialdata):
-    data = {}
-    theKeys = initialdata.keys()
+    data = dict()
+    theKeys = list(initialdata.keys())
     theKeys.remove('channels')
     for k in theKeys:
         data[k] = initialdata[k]
     data['channels'] = {}
-    for t in initialdata['channels']:
-        assert('$ref' not in initialdata['channels'][t]), "$ref to channel item not supported"
-        data['channels'][t] = {}
-        channelItemProps = data['channels'][t].keys()
-        channelItemProps.remove('subscribe')
-        channelItemProps.remove('publish')
-        for p in channelItemProps:
-            data['channels'][t][p] = initialdata['channels'][t][p]
-        if 'publish' in initialdata['channels'][t]:
-            data['channels'][t]['subscribe'] = initialdata['channels'][t]['publish']
-        if 'subscribe' in initialdata['channels'][t]:
-            data['channels'][t]['publish'] = initialdata['channels'][t]['subscribe']
+    for channel_topic in initialdata['channels']:
+        if '$ref' in initialdata['channels'][channel_topic]:
+            raise NotImplementedError("$ref to channel item not supported")
+        data['channels'][channel_topic] = dict()
+        channel_item_fields = list(initialdata['channels'][channel_topic].keys())
+        if 'subscribe' in channel_item_fields:
+            channel_item_fields.remove('subscribe')
+        if 'publish' in channel_item_fields:
+            channel_item_fields.remove('publish')
+        for field_name in channel_item_fields:
+            data['channels'][channel_topic][field_name] = initialdata['channels'][channel_topic][field_name]
+        if 'publish' in initialdata['channels'][channel_topic]:
+            data['channels'][channel_topic]['subscribe'] = initialdata['channels'][channel_topic]['publish']
+        if 'subscribe' in initialdata['channels'][channel_topic]:
+            data['channels'][channel_topic]['publish'] = initialdata['channels'][channel_topic]['subscribe']
     return data
```

### Comparing `asyncapi-codegen-0.4.1/setup.py` & `asyncapi-codegen-0.5.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,8 +27,11 @@
             'asyncapicodegen.templates.python': ['*.jinja2'],
             'asyncapicodegen.templates.markdown': ['*.jinja2'],
       },
       zip_safe=False,
       install_requires=requirements,
       include_package_data=True,
       python_requires='>=3.7',
+      scripts=[
+          'bin/asyncapi-codegen',
+      ]
 )
```

