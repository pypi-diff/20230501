# Comparing `tmp/storedict-0.0.2-py3-none-any.whl.zip` & `tmp/storedict-0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 3225 bytes, number of entries: 7
--rw-r--r--  2.0 unx       59 b- defN 23-Apr-29 19:01 storedict/__init__.py
--rw-r--r--  2.0 unx     5568 b- defN 23-Apr-29 18:49 storedict/storedict.py
--rw-r--r--  2.0 unx     2787 b- defN 23-Apr-29 18:49 storedict/tests.py
--rw-r--r--  2.0 unx      175 b- defN 23-Apr-29 19:10 storedict-0.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-29 19:10 storedict-0.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 23-Apr-29 19:10 storedict-0.0.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      535 b- defN 23-Apr-29 19:10 storedict-0.0.2.dist-info/RECORD
-7 files, 9226 bytes uncompressed, 2277 bytes compressed:  75.3%
+Zip file size: 3264 bytes, number of entries: 7
+-rw-rw-r--  2.0 unx       59 b- defN 23-Apr-30 22:10 storedict/__init__.py
+-rw-rw-r--  2.0 unx     5573 b- defN 23-Apr-30 22:07 storedict/storedict.py
+-rw-rw-r--  2.0 unx     2864 b- defN 23-Apr-30 21:29 storedict/tests.py
+-rw-rw-r--  2.0 unx      239 b- defN 23-Apr-30 22:10 storedict-0.0.3.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Apr-30 22:10 storedict-0.0.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 23-Apr-30 22:10 storedict-0.0.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      535 b- defN 23-Apr-30 22:10 storedict-0.0.3.dist-info/RECORD
+7 files, 9372 bytes uncompressed, 2316 bytes compressed:  75.3%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: storedict/storedict.py
 Comment: 
 
 Filename: storedict/tests.py
 Comment: 
 
-Filename: storedict-0.0.2.dist-info/METADATA
+Filename: storedict-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: storedict-0.0.2.dist-info/WHEEL
+Filename: storedict-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: storedict-0.0.2.dist-info/top_level.txt
+Filename: storedict-0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: storedict-0.0.2.dist-info/RECORD
+Filename: storedict-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## storedict/__init__.py

```diff
@@ -1,3 +1,3 @@
 from .storedict import create_store
 
-__version__ = "0.0.2"
+__version__ = "0.0.3"
```

## storedict/storedict.py

```diff
@@ -1,19 +1,18 @@
 from collections.abc import MutableMapping
+from typing import Optional
 
 import requests
 
 
 class ProxyError(Exception):
     pass
 
 
 class BaseStore(MutableMapping):
-    """Keys must be strings"""
-
     def __getitem__(self, key):
         ...
 
     def __setitem__(self, key, value):
         ...
 
     def __delitem__(self, key):
@@ -45,15 +44,15 @@
 
     def validate_key(self, key):
         if not isinstance(key, str):
             raise TypeError("Key must be a string")
 
     def validate_value(self, value):
         """
-        Values must be strings, ints, dicts, or lists. Nested objects should
+        Values must be strings, ints, bools, dicts, or lists. Nested objects should
         follow the same rule. All dict keys must be strings.
         """
         if isinstance(value, (str, int, bool)):
             return
         elif isinstance(value, dict):
             for k, v in value.items():
                 if not isinstance(k, str):
@@ -65,146 +64,144 @@
         else:
             raise TypeError("Value must be a string, int, bool, dict, or list")
 
 
 class LocalStore(BaseStore):
     def __init__(self):
         super().__init__()
-        self._store = {}
+        self._data = {}
 
     def __getitem__(self, key):
         self.validate_key(key)
-        return self._store[key]
+        return self._data[key]
 
     def __setitem__(self, key, value):
         self.validate_key(key)
         self.validate_value(value)
-        self._store[key] = value
+        self._data[key] = value
 
     def __delitem__(self, key):
         self.validate_key(key)
-        del self._store[key]
+        del self._data[key]
 
     def __iter__(self):
-        return iter(self._store)
+        return iter(self._data)
 
     def __len__(self):
-        return len(self._store)
+        return len(self._data)
 
     def __contains__(self, key):
         self.validate_key(key)
-        return key in self._store
+        return key in self._data
 
     def get(self, key, default=None):
         self.validate_key(key)
-        return self._store.get(key, default)
+        return self._data.get(key, default)
 
     def items(self):
-        return self._store.items()
+        return self._data.items()
 
     def keys(self):
-        return self._store.keys()
+        return self._data.keys()
 
     def values(self):
-        return self._store.values()
+        return self._data.values()
 
     def clear(self):
-        self._store.clear()
+        self._data.clear()
 
 
 class ProductionStore(BaseStore):
-    def __init__(self, datastore_proxy_url):
+    def __init__(self, datastore_proxy_url: str):
         super().__init__()
         self.datastore_proxy_url = datastore_proxy_url
         self.urls = {
-            "key-exists": self.datastore_proxy_url + "/key-exists",
-            "put-value": self.datastore_proxy_url + "/put-value",
             "get-value": self.datastore_proxy_url + "/get-value",
-            "get-items": self.datastore_proxy_url + "/get-items",
-            "delete-item": self.datastore_proxy_url + "/delete-item",
-            "count": self.datastore_proxy_url + "/count",
-            "clear": self.datastore_proxy_url + "/clear",
+            "set-value": self.datastore_proxy_url + "/set-value",
+            "delete-key": self.datastore_proxy_url + "/delete-key",
+            "key-exists": self.datastore_proxy_url + "/key-exists",
+            "get-data": self.datastore_proxy_url + "/get-data",
+            "get-data-size": self.datastore_proxy_url + "/get-data-size",
+            "delete-data": self.datastore_proxy_url + "/delete-data",
         }
 
     def __getitem__(self, key):
         self.validate_key(key)
         r = requests.post(self.urls["get-value"], json={"key": key})
         if r.status_code == 404:
             raise KeyError()
         if r.status_code != 200:
             raise ProxyError()
         return r.json()
 
     def __setitem__(self, key, value):
         self.validate_key(key)
         self.validate_value(value)
-        r = requests.post(self.urls["put-value"], json={"key": key, "value": value})
+        r = requests.post(self.urls["set-value"], json={"key": key, "value": value})
         if r.status_code != 200:
             raise ProxyError()
 
     def __delitem__(self, key):
         self.validate_key(key)
-        r = requests.post(self.urls["delete-item"], json={"key": key})
+        r = requests.post(self.urls["delete-key"], json={"key": key})
         if r.status_code == 404:
             raise KeyError()
         if r.status_code != 200:
             raise ProxyError()
 
     def __iter__(self):
-        r = requests.post(self.urls["get-items"])
+        r = requests.post(self.urls["get-data"])
         if r.status_code != 200:
             raise ProxyError()
         return iter(r.json())
 
     def __len__(self):
-        r = requests.post(self.urls["count"])
+        r = requests.post(self.urls["get-data-size"])
         if r.status_code != 200:
             raise ProxyError()
         return r.json()
 
     def __contains__(self, key):
         self.validate_key(key)
         r = requests.post(self.urls["key-exists"], json={"key": key})
-        if r.status_code == 404:
-            return False
-        if r.status_code == 200:
-            return True
-        raise ProxyError()
+        if r.status_code != 200:
+            raise ProxyError()
+        return r.json()
 
     def get(self, key, default=None):
         self.validate_key(key)
         r = requests.post(self.urls["get-value"], json={"key": key})
         if r.status_code == 404:
             return default
         if r.status_code != 200:
             raise ProxyError()
         return r.json()
 
     def items(self):
-        r = requests.post(self.urls["get-items"])
+        r = requests.post(self.urls["get-data"])
         if r.status_code != 200:
             raise ProxyError()
         return r.json().items()
 
     def keys(self):
-        r = requests.post(self.urls["get-items"])
+        r = requests.post(self.urls["get-data"])
         if r.status_code != 200:
             raise ProxyError()
         return r.json().keys()
 
     def values(self):
-        r = requests.post(self.urls["get-items"])
+        r = requests.post(self.urls["get-data"])
         if r.status_code != 200:
             raise ProxyError()
         return r.json().values()
 
     def clear(self):
-        r = requests.post(self.urls["clear"])
+        r = requests.post(self.urls["delete-data"])
         if r.status_code != 200:
             raise ProxyError()
 
 
-def create_store(datastore_proxy_url=None):
+def create_store(datastore_proxy_url: Optional[str] = None) -> BaseStore:
     if datastore_proxy_url is None:
         return LocalStore()
     else:
         return ProductionStore(datastore_proxy_url)
```

## storedict/tests.py

```diff
@@ -118,13 +118,15 @@
     store["foo"] = 1
     store["foo"] = False
     store["foo"] = {"bar": 1}
     store["foo"] = [1, 2, 3]
 
     with pytest.raises(TypeError):
         store["foo"] = (1, 2, 3)
+    with pytest.raises(TypeError):
+        store["foo"] = {"bar": (1, 2, 3)}
 
     # Dict key must be a string
     with pytest.raises(TypeError):
         store["foo"] = {1: 2}
     with pytest.raises(TypeError):
         store["foo"] = {"bar": {1: 2}}
```

