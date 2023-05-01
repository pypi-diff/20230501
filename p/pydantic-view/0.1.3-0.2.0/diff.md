# Comparing `tmp/pydantic_view-0.1.3.tar.gz` & `tmp/pydantic_view-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_view-0.1.3.tar", max compression
+gzip compressed data, was "pydantic_view-0.2.0.tar", max compression
```

## Comparing `pydantic_view-0.1.3.tar` & `pydantic_view-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1068 2023-04-22 16:35:00.000000 pydantic_view-0.1.3/LICENSE
--rw-r--r--   0        0        0     5625 2023-04-28 19:14:58.000000 pydantic_view-0.1.3/README.md
--rw-r--r--   0        0        0      142 2023-04-28 16:02:37.000000 pydantic_view-0.1.3/pydantic_view/__init__.py
--rw-r--r--   0        0        0     4867 2023-04-28 21:54:10.000000 pydantic_view-0.1.3/pydantic_view/pydantic_view.py
--rw-r--r--   0        0        0      872 2023-04-28 22:11:40.000000 pydantic_view-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     6545 1970-01-01 00:00:00.000000 pydantic_view-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-04-22 16:35:00.000000 pydantic_view-0.2.0/LICENSE
+-rw-r--r--   0        0        0     5704 2023-04-29 10:58:09.000000 pydantic_view-0.2.0/README.md
+-rw-r--r--   0        0        0      163 2023-04-29 10:56:18.000000 pydantic_view-0.2.0/pydantic_view/__init__.py
+-rw-r--r--   0        0        0     6473 2023-05-01 11:00:27.000000 pydantic_view-0.2.0/pydantic_view/pydantic_view.py
+-rw-r--r--   0        0        0      876 2023-05-01 14:19:36.000000 pydantic_view-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     6638 1970-01-01 00:00:00.000000 pydantic_view-0.2.0/PKG-INFO
```

### Comparing `pydantic_view-0.1.3/LICENSE` & `pydantic_view-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_view-0.1.3/README.md` & `pydantic_view-0.2.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -72,21 +72,22 @@
         return v
 
 
 @view("Out", exclude=["password"], recursive=True)
 @view(
     "Create",
     exclude=["id"],
-    optional_ex={"groups": Field(default_factory=lambda: [Group(id=0, name="default")])},
+    fields={"groups": Field(default_factory=lambda: [Group(id=0, name="default")])},
     config={"extra": "forbid"},
+    recursive=True,
 )
-@view("Update", exclude=["id"])
-@view("UpdateMany")
-@view("Patch", exclude=["id"], optional=["username", "password", "groups"])
-@view("PatchMany", optional=["username", "password", "groups"])
+@view("Update", exclude=["id"], recursive=True)
+@view("UpdateMany", recursive=True)
+@view("Patch", exclude=["id"], optional=["username", "password", "groups"], recursive=True)
+@view("PatchMany", optional=["username", "password", "groups"], recursive=True)
 class User(BaseModel):
     id: int
     username: str
     password: str
     groups: List[Group]
```

### Comparing `pydantic_view-0.1.3/pyproject.toml` & `pydantic_view-0.2.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydantic-view"
-version = "0.1.3"
+version = "0.2.0"
 description = "View decorator to create the child pydantic models from the root model."
 authors = ["Roman Koshel <roma.koshel@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["pydantic", "model", "view", "utils"]
 packages = [{include = "pydantic_view"}]
 classifiers = [
@@ -14,15 +14,15 @@
     "Framework :: Pydantic",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Utilities",
     "License :: OSI Approved :: MIT License",
 ]
 
 [tool.poetry.dependencies]
-pydantic = "*"
+pydantic = "^1.10"
 python = "^3.8"
 
 
 [tool.poetry.group.test.dependencies]
 ipdb = "*"
 fastapi = "*"
 httpx = "*"
```

### Comparing `pydantic_view-0.1.3/PKG-INFO` & `pydantic_view-0.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-view
-Version: 0.1.3
+Version: 0.2.0
 Summary: View decorator to create the child pydantic models from the root model.
 License: MIT
 Keywords: pydantic,model,view,utils
 Author: Roman Koshel
 Author-email: roma.koshel@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
-Requires-Dist: pydantic
+Requires-Dist: pydantic (>=1.10,<2.0)
 Description-Content-Type: text/markdown
 
 # Pydantic view helper decorator
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 ### Installation
@@ -96,21 +96,22 @@
         return v
 
 
 @view("Out", exclude=["password"], recursive=True)
 @view(
     "Create",
     exclude=["id"],
-    optional_ex={"groups": Field(default_factory=lambda: [Group(id=0, name="default")])},
+    fields={"groups": Field(default_factory=lambda: [Group(id=0, name="default")])},
     config={"extra": "forbid"},
+    recursive=True,
 )
-@view("Update", exclude=["id"])
-@view("UpdateMany")
-@view("Patch", exclude=["id"], optional=["username", "password", "groups"])
-@view("PatchMany", optional=["username", "password", "groups"])
+@view("Update", exclude=["id"], recursive=True)
+@view("UpdateMany", recursive=True)
+@view("Patch", exclude=["id"], optional=["username", "password", "groups"], recursive=True)
+@view("PatchMany", optional=["username", "password", "groups"], recursive=True)
 class User(BaseModel):
     id: int
     username: str
     password: str
     groups: List[Group]
```

