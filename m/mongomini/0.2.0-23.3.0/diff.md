# Comparing `tmp/mongomini-0.2.0.tar.gz` & `tmp/mongomini-23.3.0.tar.gz`

## Comparing `mongomini-0.2.0.tar` & `mongomini-23.3.0.tar`

### file list

```diff
@@ -1,14 +1,6 @@
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 mongomini-0.2.0/mongomini/__about__.py
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 mongomini-0.2.0/mongomini/__init__.py
--rw-r--r--   0        0        0     4910 2020-02-02 00:00:00.000000 mongomini-0.2.0/mongomini/dataclasses.py
--rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 mongomini-0.2.0/mongomini/documents.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 mongomini-0.2.0/mongomini/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mongomini-0.2.0/tests/__init__.py
--rw-r--r--   0        0        0     2552 2020-02-02 00:00:00.000000 mongomini-0.2.0/tests/test_dataclasses.py
--rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 mongomini-0.2.0/tests/test_document_classes.py
--rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 mongomini-0.2.0/tests/test_document_intances.py
--rw-r--r--   0        0        0     2035 2020-02-02 00:00:00.000000 mongomini-0.2.0/.gitignore
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 mongomini-0.2.0/LICENSE
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 mongomini-0.2.0/README.md
--rw-r--r--   0        0        0     1324 2020-02-02 00:00:00.000000 mongomini-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 mongomini-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     2209 2020-02-02 00:00:00.000000 mongomini-23.3.0/mongomini/__init__.py
+-rw-r--r--   0        0        0     2035 2020-02-02 00:00:00.000000 mongomini-23.3.0/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 mongomini-23.3.0/LICENSE
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 mongomini-23.3.0/README.md
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 mongomini-23.3.0/pyproject.toml
+-rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 mongomini-23.3.0/PKG-INFO
```

### Comparing `mongomini-0.2.0/mongomini/documents.py` & `mongomini-23.3.0/mongomini/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,75 +1,81 @@
-from dataclasses import dataclass
-from typing import Any
+from dataclasses import asdict, dataclass, field, fields
+from typing import ClassVar
 
 from bson import ObjectId
+from motor.motor_asyncio import AsyncIOMotorCollection, AsyncIOMotorCursor
+import pymongo
 
-from .dataclasses import (
-    documentclass, delete_one, insert_one, is_documentclass, update_one, find
-)
-from .exceptions import MultipleObjectsReturned, ObjectDoesNotExist
 
+CollectionType = ClassVar[AsyncIOMotorCollection]
 
-class DocumentMeta(type):
 
-    def __new__(metacls, name, bases, attrs):
-        new_cls = super().__new__(metacls, name, bases, attrs)
+@dataclass(kw_only=True)
+class Document:
+    _collection: CollectionType
+    _id: ObjectId = field(default_factory=ObjectId)
 
-        if name == 'Document' and not bases:
-            # if Base Document, then just make a regular dataclass.
-            return dataclass(new_cls)
-
-        settings: type | None = attrs.pop('Settings', None)
-
-        db = getattr(settings, 'db', None)
-        collection_name = getattr(settings, 'collection_name', "")
-        repr = getattr(settings, 'repr', True)
-        eq = getattr(settings, 'eq', True)
-        order = getattr(settings, 'order', False)
-
-        new_cls = documentclass(
-            db=db, collection_name=collection_name, repr=repr, eq=eq, order=order
-        )(new_cls)
-        return new_cls
-
-    def __call__(self, *args, **kwargs):
-        if not is_documentclass(self):
-            raise TypeError(f"Can't instantiate abstract class '{self.__name__}'.")
-        return super().__call__(*args, **kwargs)
+    @classmethod
+    def from_document(cls, document: dict):
+        field_names = set(f.name for f in fields(cls))
+        fields_in_doc = field_names.intersection(document)
+        params = {f: document[f] for f in fields_in_doc}
+        return cls(**params)
 
+    @classmethod
+    def find(
+        cls,
+        **kwargs
+    ) -> AsyncIOMotorCursor:
+        cursor = cls._collection.find(filter=kwargs)
+        return DocumentCursor(cls, cursor)
 
-class Document(metaclass=DocumentMeta):
+    @classmethod
+    async def find_one(cls, **kwargs):
+        document = await cls._collection.find_one(kwargs)
+        if document is None:
+            return None
+        return cls.from_document(document)
 
-    class Settings:
-        ...
+    async def insert(self):
+        result = await self._collection.insert_one(asdict(self))
+        assert result.inserted_id == self._id
 
-    _id: ObjectId | None = None
+    async def update(self):
+        result = await self._collection.update_one(
+            filter={"_id": self._id}, update={"$set": asdict(self)}
+        )
+        assert result.matched_count == 1
+        assert result.modified_count == 1
 
-    @classmethod
-    def find(cls, query: dict[str, Any]):
-        return find(cls, query)
+    async def delete(self):
+        result = await self._collection.delete_one({"_id": self._id})
+        assert result.deleted_count == 1
 
-    @classmethod
-    async def get(cls, query: dict[str, Any]):
-        cursor = cls.find(query)
-        try:
-            result = await anext(cursor)
 
-        except StopAsyncIteration as exc:
-            raise ObjectDoesNotExist
+@dataclass
+class DocumentCursor:
 
-        try:
-            await anext(cursor)
+    class_: type[Document]
+    cursor: AsyncIOMotorCursor
 
-        except StopAsyncIteration:
-            return result
+    def __aiter__(self):
+        return self
 
-        raise MultipleObjectsReturned
+    async def __anext__(self):
+        document = await anext(self.cursor)
+        return self.class_.from_document(document)
 
-    async def insert(self):
-        return await insert_one(self)
+    def limit(self, limit: int):
+        self.cursor.limit(limit)
 
-    async def update(self, *fields):
-        return await update_one(self, *fields)
+    def skip(self, skip: int):
+        self.cursor.skip(skip)
 
-    async def delete(self):
-        return await delete_one(self)
+    def sort(self, *fields: str):
+        field_list =[
+            (f, pymongo.ASCENDING)
+            if not f.startswith('-')
+            else (f[1:], pymongo.DESCENDING)
+            for f in fields
+        ]
+        self.cursor.sort(field_list)
```

### Comparing `mongomini-0.2.0/.gitignore` & `mongomini-23.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `mongomini-0.2.0/LICENSE` & `mongomini-23.3.0/LICENSE`

 * *Files identical despite different names*

