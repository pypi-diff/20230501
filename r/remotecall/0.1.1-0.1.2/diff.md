# Comparing `tmp/remotecall-0.1.1.tar.gz` & `tmp/remotecall-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remotecall-0.1.1.tar", last modified: Sun Apr 23 19:32:17 2023, max compression
+gzip compressed data, was "remotecall-0.1.2.tar", last modified: Mon May  1 19:17:18 2023, max compression
```

## Comparing `remotecall-0.1.1.tar` & `remotecall-0.1.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 slaine   (1355619077) 1965124760        0 2023-04-23 19:32:17.333120 remotecall-0.1.1/
--rw-r--r--   0 slaine   (1355619077) 1965124760     1481 2023-03-11 14:26:45.000000 remotecall-0.1.1/LICENSE
--rw-r--r--   0 slaine   (1355619077) 1965124760      364 2023-04-23 19:32:17.332840 remotecall-0.1.1/PKG-INFO
--rw-r--r--   0 slaine   (1355619077) 1965124760     7640 2023-03-19 20:05:21.000000 remotecall-0.1.1/README.md
--rw-r--r--   0 slaine   (1355619077) 1965124760       38 2023-04-23 19:32:17.333249 remotecall-0.1.1/setup.cfg
--rw-r--r--   0 slaine   (1355619077) 1965124760      970 2023-03-20 17:55:00.000000 remotecall-0.1.1/setup.py
-drwxr-xr-x   0 slaine   (1355619077) 1965124760        0 2023-04-23 19:32:17.302357 remotecall-0.1.1/src/
-drwxr-xr-x   0 slaine   (1355619077) 1965124760        0 2023-04-23 19:32:17.311326 remotecall-0.1.1/src/remotecall/
--rw-r--r--   0 slaine   (1355619077) 1965124760     1042 2023-03-20 07:11:43.000000 remotecall-0.1.1/src/remotecall/__init__.py
--rw-r--r--   0 slaine   (1355619077) 1965124760     3018 2023-03-18 08:49:15.000000 remotecall-0.1.1/src/remotecall/__main__.py
--rw-r--r--   0 slaine   (1355619077) 1965124760      212 2023-04-20 11:52:34.000000 remotecall-0.1.1/src/remotecall/_meta.py
-drwxr-xr-x   0 slaine   (1355619077) 1965124760        0 2023-04-23 19:32:17.330771 remotecall-0.1.1/src/remotecall/authentication/
--rw-r--r--   0 slaine   (1355619077) 1965124760      768 2023-03-17 11:15:02.000000 remotecall-0.1.1/src/remotecall/authentication/__init__.py
--rw-r--r--   0 slaine   (1355619077) 1965124760     2369 2023-03-19 09:02:03.000000 remotecall-0.1.1/src/remotecall/authentication/authenticator.py
--rw-r--r--   0 slaine   (1355619077) 1965124760     3590 2023-03-20 09:01:04.000000 remotecall-0.1.1/src/remotecall/client.py
--rw-r--r--   0 slaine   (1355619077) 1965124760     4452 2023-03-18 08:30:48.000000 remotecall-0.1.1/src/remotecall/clientfactory.py
--rw-r--r--   0 slaine   (1355619077) 1965124760     5504 2023-03-11 14:36:05.000000 remotecall-0.1.1/src/remotecall/codecs.py
-drwxr-xr-x   0 slaine   (1355619077) 1965124760        0 2023-04-23 19:32:17.332365 remotecall-0.1.1/src/remotecall/constants/
--rw-r--r--   0 slaine   (1355619077) 1965124760        0 2023-04-20 11:46:26.000000 remotecall-0.1.1/src/remotecall/constants/__init__.py
--rw-r--r--   0 slaine   (1355619077) 1965124760      174 2023-04-20 11:38:21.000000 remotecall-0.1.1/src/remotecall/constants/headers.py
--rw-r--r--   0 slaine   (1355619077) 1965124760      204 2023-03-19 20:17:29.000000 remotecall-0.1.1/src/remotecall/constants/statuscodes.py
--rw-r--r--   0 slaine   (1355619077) 1965124760     2186 2023-03-18 08:50:36.000000 remotecall-0.1.1/src/remotecall/endpoint.py
--rw-r--r--   0 slaine   (1355619077) 1965124760      456 2023-03-16 18:22:04.000000 remotecall-0.1.1/src/remotecall/errors.py
--rw-r--r--   0 slaine   (1355619077) 1965124760      629 2023-03-20 07:34:11.000000 remotecall-0.1.1/src/remotecall/gethandler.py
--rw-r--r--   0 slaine   (1355619077) 1965124760     6170 2023-03-20 07:48:34.000000 remotecall-0.1.1/src/remotecall/posthandler.py
--rw-r--r--   0 slaine   (1355619077) 1965124760     4588 2023-03-20 07:48:46.000000 remotecall-0.1.1/src/remotecall/requesthandler.py
--rw-r--r--   0 slaine   (1355619077) 1965124760      626 2023-03-19 20:16:41.000000 remotecall-0.1.1/src/remotecall/response.py
--rw-r--r--   0 slaine   (1355619077) 1965124760     2720 2023-03-20 07:49:47.000000 remotecall-0.1.1/src/remotecall/server.py
-drwxr-xr-x   0 slaine   (1355619077) 1965124760        0 2023-04-23 19:32:17.316234 remotecall-0.1.1/src/remotecall.egg-info/
--rw-r--r--   0 slaine   (1355619077) 1965124760      364 2023-04-23 19:32:17.000000 remotecall-0.1.1/src/remotecall.egg-info/PKG-INFO
--rw-r--r--   0 slaine   (1355619077) 1965124760      851 2023-04-23 19:32:17.000000 remotecall-0.1.1/src/remotecall.egg-info/SOURCES.txt
--rw-r--r--   0 slaine   (1355619077) 1965124760        1 2023-04-23 19:32:17.000000 remotecall-0.1.1/src/remotecall.egg-info/dependency_links.txt
--rw-r--r--   0 slaine   (1355619077) 1965124760       50 2023-04-23 19:32:17.000000 remotecall-0.1.1/src/remotecall.egg-info/entry_points.txt
--rw-r--r--   0 slaine   (1355619077) 1965124760        1 2023-02-07 05:13:42.000000 remotecall-0.1.1/src/remotecall.egg-info/not-zip-safe
--rw-r--r--   0 slaine   (1355619077) 1965124760       32 2023-04-23 19:32:17.000000 remotecall-0.1.1/src/remotecall.egg-info/requires.txt
--rw-r--r--   0 slaine   (1355619077) 1965124760       11 2023-04-23 19:32:17.000000 remotecall-0.1.1/src/remotecall.egg-info/top_level.txt
+drwxr-xr-x   0 slaine   (1355619077) 1965124760        0 2023-05-01 19:17:18.180900 remotecall-0.1.2/
+-rw-r--r--   0 slaine   (1355619077) 1965124760     1481 2023-03-11 14:26:45.000000 remotecall-0.1.2/LICENSE
+-rw-r--r--   0 slaine   (1355619077) 1965124760      364 2023-05-01 19:17:18.180471 remotecall-0.1.2/PKG-INFO
+-rw-r--r--   0 slaine   (1355619077) 1965124760     7640 2023-03-19 20:05:21.000000 remotecall-0.1.2/README.md
+-rw-r--r--   0 slaine   (1355619077) 1965124760       38 2023-05-01 19:17:18.181031 remotecall-0.1.2/setup.cfg
+-rw-r--r--   0 slaine   (1355619077) 1965124760      970 2023-03-20 17:55:00.000000 remotecall-0.1.2/setup.py
+drwxr-xr-x   0 slaine   (1355619077) 1965124760        0 2023-05-01 19:17:18.133600 remotecall-0.1.2/src/
+drwxr-xr-x   0 slaine   (1355619077) 1965124760        0 2023-05-01 19:17:18.168172 remotecall-0.1.2/src/remotecall/
+-rw-r--r--   0 slaine   (1355619077) 1965124760     1042 2023-03-20 07:11:43.000000 remotecall-0.1.2/src/remotecall/__init__.py
+-rw-r--r--   0 slaine   (1355619077) 1965124760     3018 2023-03-18 08:49:15.000000 remotecall-0.1.2/src/remotecall/__main__.py
+-rw-r--r--   0 slaine   (1355619077) 1965124760      218 2023-05-01 19:13:47.000000 remotecall-0.1.2/src/remotecall/_meta.py
+drwxr-xr-x   0 slaine   (1355619077) 1965124760        0 2023-05-01 19:17:18.176281 remotecall-0.1.2/src/remotecall/authentication/
+-rw-r--r--   0 slaine   (1355619077) 1965124760      768 2023-03-17 11:15:02.000000 remotecall-0.1.2/src/remotecall/authentication/__init__.py
+-rw-r--r--   0 slaine   (1355619077) 1965124760     2369 2023-03-19 09:02:03.000000 remotecall-0.1.2/src/remotecall/authentication/authenticator.py
+-rw-r--r--   0 slaine   (1355619077) 1965124760     3590 2023-03-20 09:01:04.000000 remotecall-0.1.2/src/remotecall/client.py
+-rw-r--r--   0 slaine   (1355619077) 1965124760     4807 2023-05-01 19:13:47.000000 remotecall-0.1.2/src/remotecall/clientfactory.py
+-rw-r--r--   0 slaine   (1355619077) 1965124760     5504 2023-03-11 14:36:05.000000 remotecall-0.1.2/src/remotecall/codecs.py
+drwxr-xr-x   0 slaine   (1355619077) 1965124760        0 2023-05-01 19:17:18.179262 remotecall-0.1.2/src/remotecall/constants/
+-rw-r--r--   0 slaine   (1355619077) 1965124760        0 2023-04-20 11:46:26.000000 remotecall-0.1.2/src/remotecall/constants/__init__.py
+-rw-r--r--   0 slaine   (1355619077) 1965124760      174 2023-04-20 11:38:21.000000 remotecall-0.1.2/src/remotecall/constants/headers.py
+-rw-r--r--   0 slaine   (1355619077) 1965124760      204 2023-03-19 20:17:29.000000 remotecall-0.1.2/src/remotecall/constants/statuscodes.py
+-rw-r--r--   0 slaine   (1355619077) 1965124760     3555 2023-05-01 19:13:47.000000 remotecall-0.1.2/src/remotecall/endpoint.py
+-rw-r--r--   0 slaine   (1355619077) 1965124760      456 2023-03-16 18:22:04.000000 remotecall-0.1.2/src/remotecall/errors.py
+-rw-r--r--   0 slaine   (1355619077) 1965124760      629 2023-03-20 07:34:11.000000 remotecall-0.1.2/src/remotecall/gethandler.py
+-rw-r--r--   0 slaine   (1355619077) 1965124760     6170 2023-03-20 07:48:34.000000 remotecall-0.1.2/src/remotecall/posthandler.py
+-rw-r--r--   0 slaine   (1355619077) 1965124760     4588 2023-03-20 07:48:46.000000 remotecall-0.1.2/src/remotecall/requesthandler.py
+-rw-r--r--   0 slaine   (1355619077) 1965124760      626 2023-03-19 20:16:41.000000 remotecall-0.1.2/src/remotecall/response.py
+-rw-r--r--   0 slaine   (1355619077) 1965124760     3249 2023-05-01 19:13:47.000000 remotecall-0.1.2/src/remotecall/server.py
+drwxr-xr-x   0 slaine   (1355619077) 1965124760        0 2023-05-01 19:17:18.174217 remotecall-0.1.2/src/remotecall.egg-info/
+-rw-r--r--   0 slaine   (1355619077) 1965124760      364 2023-05-01 19:17:18.000000 remotecall-0.1.2/src/remotecall.egg-info/PKG-INFO
+-rw-r--r--   0 slaine   (1355619077) 1965124760      851 2023-05-01 19:17:18.000000 remotecall-0.1.2/src/remotecall.egg-info/SOURCES.txt
+-rw-r--r--   0 slaine   (1355619077) 1965124760        1 2023-05-01 19:17:18.000000 remotecall-0.1.2/src/remotecall.egg-info/dependency_links.txt
+-rw-r--r--   0 slaine   (1355619077) 1965124760       50 2023-05-01 19:17:18.000000 remotecall-0.1.2/src/remotecall.egg-info/entry_points.txt
+-rw-r--r--   0 slaine   (1355619077) 1965124760        1 2023-02-07 05:13:42.000000 remotecall-0.1.2/src/remotecall.egg-info/not-zip-safe
+-rw-r--r--   0 slaine   (1355619077) 1965124760       32 2023-05-01 19:17:18.000000 remotecall-0.1.2/src/remotecall.egg-info/requires.txt
+-rw-r--r--   0 slaine   (1355619077) 1965124760       11 2023-05-01 19:17:18.000000 remotecall-0.1.2/src/remotecall.egg-info/top_level.txt
```

### Comparing `remotecall-0.1.1/LICENSE` & `remotecall-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `remotecall-0.1.1/README.md` & `remotecall-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `remotecall-0.1.1/setup.py` & `remotecall-0.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `remotecall-0.1.1/src/remotecall/__init__.py` & `remotecall-0.1.2/src/remotecall/__init__.py`

 * *Files identical despite different names*

### Comparing `remotecall-0.1.1/src/remotecall/__main__.py` & `remotecall-0.1.2/src/remotecall/__main__.py`

 * *Files identical despite different names*

### Comparing `remotecall-0.1.1/src/remotecall/authentication/__init__.py` & `remotecall-0.1.2/src/remotecall/authentication/__init__.py`

 * *Files identical despite different names*

### Comparing `remotecall-0.1.1/src/remotecall/authentication/authenticator.py` & `remotecall-0.1.2/src/remotecall/authentication/authenticator.py`

 * *Files identical despite different names*

### Comparing `remotecall-0.1.1/src/remotecall/client.py` & `remotecall-0.1.2/src/remotecall/client.py`

 * *Files identical despite different names*

### Comparing `remotecall-0.1.1/src/remotecall/clientfactory.py` & `remotecall-0.1.2/src/remotecall/clientfactory.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,161 +1,163 @@
-import typing
-from typing import Optional
-
-"""
-Example:
-    {
-        "endpoints": [
-            {
-                "name": "foo",
-                "documentation": "Foo.\n\nTest docstring.",
-                "parameters": [
-                    {
-                        "name": "a",
-                        "type": "int"
-                    },
-                    {
-                        "name": "b",
-                        "type": "str",
-                        "default": "foo"
-                    }
-                ],
-                "return_type": "bool"
-            }
-        ],
-        "address": {
-            "hostname": "127.0.0.1",
-            "port": 8000
-        }
-    }
-"""
-
-
-class ClientFactory:
-    def __init__(self, definition: dict, class_name: Optional[str] = None):
-        self._definition = definition
-        self._client_class_name = class_name or "Client"
-
-    def generate(self):
-        address = self._definition.get("address", {})
-        host = address.get("host", "localhost")
-        port = address.get("port", 8000)
-
-        c = Class(name=self._client_class_name)
-        c.doc = self._definition.get("documentation", "")
-        c.methods.append(self.generate_init_method((host, port)))
-
-        endpoints = self._definition.get("endpoints", [])
-        for endpoint in endpoints:
-            name = endpoint.get("name")
-            doc = endpoint.get("documentation")
-            return_type = endpoint.get("return_type")
-
-            m = Method(name=name, return_type=return_type, doc=doc)
-            c.methods.append(m)
-            for parameter in endpoint.get("parameters", []):
-                p = Parameter(
-                    parameter["name"], parameter["type"], parameter.get("default", None)
-                )
-                m.parameters.append(p)
-
-        lines = ["from __future__ import annotations\n"]
-        lines.append("from remotecall import BaseClient\n\n")
-        lines.append(str(c))
-
-        return "\n".join(lines)
-
-    @classmethod
-    def generate_init_method(cls, server_address):
-        return (
-            f"    def __init__(self, server_address={server_address}):\n"
-            f"        super().__init__(server_address=server_address)\n"
-        )
-
-
-class Parameter:
-    def __init__(self, name: str, type: typing.Type, default=None):
-        self.name = name
-        self.type = type
-        self.default = default
-
-    def __str__(self):
-        lines = [f"{self.name}: {self.type}"]
-
-        if self.default is not None:
-            if self.type == "str":
-                lines.append(f" = \"{self.default}\"")
-            else:
-                lines.append(f" = {self.default}")
-
-        return "".join(lines)
-
-
-class Method:
-    def __init__(self, name: str, return_type: str, doc: str = None):
-        self.name = name
-        self.return_type = return_type
-        self.parameters = []
-        self.indent = "    "
-        self.doc = indent_doc(doc, self.indent * 2)
-
-    def __str__(self):
-        lines = [f"{self.indent}def {self.name}(self"]
-
-        # Signature
-        for parameter in self.parameters:
-            lines.append(f", {parameter}")
-        lines.append(")")
-
-        # Return type
-        if self.return_type:
-            lines.append(f" -> {self.return_type}")
-
-        lines.append(":\n")
-
-        # Docstring
-        if self.doc:
-            lines.append(self.indent * 2)
-            lines.append(f'"""{self.doc}\n')
-            lines.append(self.indent * 2)
-            lines.append('"""\n')
-
-        # Method body
-        lines.append(self.indent * 2)
-        lines.append(f'return self.call("{self.name}"')
-
-        for parameter in self.parameters:
-            lines.append(f", {parameter.name}={parameter.name}")
-
-        lines.append(")\n")
-
-        return "".join(lines)
-
-
-class Class:
-    def __init__(self, name: str):
-        self.name = name.capitalize()
-        self.methods = []
-        self.indent = ""
-        self.doc = None
-
-    def __str__(self):
-        lines = [f"class {self.name}(BaseClient):"]
-
-        if self.doc:
-            lines.append(f'    """{self.doc}')
-            lines.append('    """')
-
-        for method in self.methods:
-            lines.append(str(method))
-
-        return "\n".join(lines)
-
-
-def indent_doc(doc: str, indent: str) -> str:
-    if not doc:
-        return doc
-
-    lines = doc.split("\n")
-    for i, line in enumerate(lines[1:], 1):
-        lines[i] = indent + line
-    return "\n".join(lines)
+import typing
+from typing import Optional
+
+"""
+Example:
+    {
+        "endpoints": [
+            {
+                "name": "foo",
+                "documentation": "Foo.\n\nTest docstring.",
+                "parameters": [
+                    {
+                        "name": "a",
+                        "annotation": "int"
+                    },
+                    {
+                        "name": "b",
+                        "annotation": "str",
+                        "default": "foo"
+                    }
+                ],
+                "return_annotation": "bool"
+            }
+        ],
+        "address": {
+            "hostname": "127.0.0.1",
+            "port": 8000
+        }
+    }
+"""
+
+
+class ClientFactory:
+    def __init__(self, definition: dict, class_name: Optional[str] = None):
+        self._definition = definition
+        self._client_class_name = class_name or "Client"
+
+    def generate(self):
+        address = self._definition.get("address", {})
+        host = address.get("host", "localhost")
+        port = address.get("port", 8000)
+
+        c = Class(name=self._client_class_name)
+        c.doc = self._definition.get("documentation", "")
+        c.methods.append(self.generate_init_method((host, port)))
+
+        endpoints = self._definition.get("endpoints", [])
+        for endpoint in endpoints:
+            name = endpoint.get("name")
+            doc = endpoint.get("documentation")
+            return_annotation = endpoint.get("return_annotation")
+
+            m = Method(name=name, return_annotation=return_annotation, doc=doc)
+            c.methods.append(m)
+            for parameter in endpoint.get("parameters", []):
+                p = Parameter(
+                    parameter["name"], parameter["annotation"], parameter.get("default", None)
+                )
+                m.parameters.append(p)
+
+        lines = ["from __future__ import annotations\n"]
+        lines.append("import typing")
+        lines.append("from typing import Optional\n")
+        lines.append("from remotecall import BaseClient\n\n")
+        lines.append(str(c))
+
+        return "\n".join(lines)
+
+    @classmethod
+    def generate_init_method(cls, server_address):
+        return (
+            f"    def __init__(self, server_address={server_address}):\n"
+            f"        super().__init__(server_address=server_address)\n"
+        )
+
+
+class Parameter:
+    def __init__(self, name: str, annotation: str, default=None):
+        self.name = name
+        self.annotation = annotation
+        self.default = default
+
+    def __str__(self):
+        lines = [f"{self.name}: {self.annotation}"]
+
+        if self.default is not None:
+            if self.annotation == "str":
+                lines.append(f" = \"{self.default}\"")
+            else:
+                lines.append(f" = {self.default}")
+
+        return "".join(lines)
+
+
+class Method:
+    def __init__(self, name: str, return_annotation: str, doc: str = None):
+        self.name = name
+        self.return_annotation = return_annotation
+        self.parameters = []
+        self.indent = "    "
+        self.doc = indent_doc(doc, self.indent * 2)
+
+    def __str__(self):
+        lines = [f"{self.indent}def {self.name}(self"]
+
+        # Signature
+        for parameter in self.parameters:
+            lines.append(f", {parameter}")
+        lines.append(")")
+
+        # Return type
+        if self.return_annotation:
+            lines.append(f" -> {self.return_annotation}")
+
+        lines.append(":\n")
+
+        # Docstring
+        if self.doc:
+            lines.append(self.indent * 2)
+            lines.append(f'"""{self.doc}\n')
+            lines.append(self.indent * 2)
+            lines.append('"""\n')
+
+        # Method body
+        lines.append(self.indent * 2)
+        lines.append(f'return self.call("{self.name}"')
+
+        for parameter in self.parameters:
+            lines.append(f", {parameter.name}={parameter.name}")
+
+        lines.append(")\n")
+
+        return "".join(lines)
+
+
+class Class:
+    def __init__(self, name: str):
+        self.name = name.capitalize()
+        self.methods = []
+        self.indent = ""
+        self.doc = None
+
+    def __str__(self):
+        lines = [f"class {self.name}(BaseClient):"]
+
+        if self.doc:
+            lines.append(f'    """{self.doc}')
+            lines.append('    """')
+
+        for method in self.methods:
+            lines.append(str(method))
+
+        return "\n".join(lines)
+
+
+def indent_doc(doc: str, indent: str) -> str:
+    if not doc:
+        return doc
+
+    lines = doc.split("\n")
+    for i, line in enumerate(lines[1:], 1):
+        lines[i] = indent + line
+    return "\n".join(lines)
```

### Comparing `remotecall-0.1.1/src/remotecall/codecs.py` & `remotecall-0.1.2/src/remotecall/codecs.py`

 * *Files identical despite different names*

### Comparing `remotecall-0.1.1/src/remotecall/gethandler.py` & `remotecall-0.1.2/src/remotecall/gethandler.py`

 * *Files identical despite different names*

### Comparing `remotecall-0.1.1/src/remotecall/posthandler.py` & `remotecall-0.1.2/src/remotecall/posthandler.py`

 * *Files identical despite different names*

### Comparing `remotecall-0.1.1/src/remotecall/requesthandler.py` & `remotecall-0.1.2/src/remotecall/requesthandler.py`

 * *Files identical despite different names*

### Comparing `remotecall-0.1.1/src/remotecall/response.py` & `remotecall-0.1.2/src/remotecall/response.py`

 * *Files identical despite different names*

### Comparing `remotecall-0.1.1/src/remotecall/server.py` & `remotecall-0.1.2/src/remotecall/server.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,87 +1,94 @@
-from __future__ import annotations
-
-import http.server
-import logging
-import typing
-from typing import Optional
-from .endpoint import Endpoint
-from .requesthandler import HTTPRequestHandler
-from .codecs import Codec
-from .codecs import Codecs
-from .authentication import Authenticator
-
-
-logger = logging.getLogger(__name__)
-
-
-class Server(http.server.ThreadingHTTPServer):
-    """Server."""
-
-    def __init__(self, server_address: tuple[str, int]):
-        super().__init__(
-            server_address=server_address, RequestHandlerClass=HTTPRequestHandler
-        )
-        self._ssl_enabled = False
-        self._authenticator: Optional[Authenticator] = None
-        self.codecs = Codecs(Codec.subclasses)
-        self.endpoints: typing.Dict[str, Endpoint] = {}
-
-    @property
-    def url(self) -> str:
-        """Server URL."""
-        hostname, port = self.server_address
-        scheme = "https" if self.ssl_enabled else "http"
-        return f"{scheme}://{hostname}:{port}"
-
-    @classmethod
-    def _create_endpoint(cls, function: typing.Callable, name: str = None):
-        """Create endpoint."""
-        if not name:
-            name = function.__name__
-        return Endpoint(name, function)
-
-    def expose(self, function: typing.Callable, name: str = None):
-        """Expose a function with given name.
-
-        Name of the callable shall be used if name is not given. The name is resolved by calling
-        __name__ of the callable.
-        """
-        logger.debug("Exposing %s ...", function)
-
-        endpoint = self._create_endpoint(function, name)
-        self.endpoints[endpoint.name] = endpoint
-
-        logger.debug("Exposed %s as %s", function, endpoint)
-
-    @property
-    def ssl_enabled(self) -> bool:
-        """Is SLL enabled."""
-        return self._ssl_enabled
-
-    def use_ssl(self, cert_file: str, key_file: str, password=None):
-        """Use SSL.
-
-        Use SSL to secure server to client transactions.
-        """
-        import ssl
-
-        logger.debug("Setting up SSL context.")
-        logger.debug("  Certificate file: %s", cert_file)
-        logger.debug("  Key file: %s", key_file)
-
-        context = ssl.SSLContext(ssl.PROTOCOL_TLS_SERVER)
-        context.check_hostname = False
-        context.load_cert_chain(certfile=cert_file, keyfile=key_file, password=password)
-
-        self.socket = context.wrap_socket(self.socket, server_side=True)
-        self._ssl_enabled = True
-
-        logger.debug("SSL enabled.")
-
-    def set_authenticator(self, authenticator: Authenticator):
-        """Set authenticator."""
-        self._authenticator = authenticator
-
-    def get_authenticator(self) -> Authenticator:
-        """Get authenticator."""
-        return self._authenticator
+from __future__ import annotations
+
+import http.server
+import logging
+import typing
+from typing import Optional
+from .endpoint import Endpoint
+from .requesthandler import HTTPRequestHandler
+from .codecs import Codec
+from .codecs import Codecs
+from .authentication import Authenticator
+
+
+logger = logging.getLogger(__name__)
+
+
+class Server(http.server.ThreadingHTTPServer):
+    """Server."""
+
+    def __init__(self, server_address: tuple[str, int]):
+        super().__init__(
+            server_address=server_address, RequestHandlerClass=HTTPRequestHandler
+        )
+        self._ssl_enabled = False
+        self._authenticator: Optional[Authenticator] = None
+        self.codecs = Codecs(Codec.subclasses)
+        self.endpoints: typing.Dict[str, Endpoint] = {}
+
+    @property
+    def url(self) -> str:
+        """Server URL."""
+        hostname, port = self.server_address
+        scheme = "https" if self.ssl_enabled else "http"
+        return f"{scheme}://{hostname}:{port}"
+
+    @classmethod
+    def _create_endpoint(cls, function: typing.Callable, name: str = None):
+        """Create endpoint."""
+        if not name:
+            try:
+                name = function.__name__
+            except AttributeError as err:
+                logger.warning("Endpoint name is optional if the value can be read from "
+                               "the provided function by calling function.__name__.")
+                raise ValueError("Endpoint name not provided and exposed function raised the "
+                                 f"following error when calling function.__name__: {err}") from err
+
+        return Endpoint(name, function)
+
+    def expose(self, function: typing.Callable, name: str = None):
+        """Expose a function with given name.
+
+        Name of the callable shall be used if name is not given. The name is resolved by calling
+        __name__ of the callable.
+        """
+        logger.debug("Exposing %s ...", function)
+
+        endpoint = self._create_endpoint(function, name)
+        self.endpoints[endpoint.name] = endpoint
+
+        logger.debug("Exposed %s as %s", function, endpoint)
+
+    @property
+    def ssl_enabled(self) -> bool:
+        """Is SLL enabled."""
+        return self._ssl_enabled
+
+    def use_ssl(self, cert_file: str, key_file: str, password=None):
+        """Use SSL.
+
+        Use SSL to secure server to client transactions.
+        """
+        import ssl
+
+        logger.debug("Setting up SSL context.")
+        logger.debug("  Certificate file: %s", cert_file)
+        logger.debug("  Key file: %s", key_file)
+
+        context = ssl.SSLContext(ssl.PROTOCOL_TLS_SERVER)
+        context.check_hostname = False
+        context.load_cert_chain(certfile=cert_file, keyfile=key_file, password=password)
+
+        self.socket = context.wrap_socket(self.socket, server_side=True)
+        self._ssl_enabled = True
+
+        logger.debug("SSL enabled.")
+
+    def set_authenticator(self, authenticator: Authenticator):
+        """Set authenticator."""
+        self._authenticator = authenticator
+
+    def get_authenticator(self) -> Authenticator:
+        """Get authenticator."""
+        return self._authenticator
```

### Comparing `remotecall-0.1.1/src/remotecall.egg-info/SOURCES.txt` & `remotecall-0.1.2/src/remotecall.egg-info/SOURCES.txt`

 * *Files identical despite different names*

