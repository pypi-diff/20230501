# Comparing `tmp/quivr-0.0.1.tar.gz` & `tmp/quivr-0.1.0.tar.gz`

## Comparing `quivr-0.0.1.tar` & `quivr-0.1.0.tar`

### file list

```diff
@@ -1,27 +1,29 @@
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 quivr-0.0.1/quivr/__init__.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 quivr-0.0.1/quivr/__init__.py~
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 quivr-0.0.1/quivr/__version__.py
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 quivr-0.0.1/quivr/__version__.py~
--rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 quivr-0.0.1/quivr/concat.py
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 quivr-0.0.1/quivr/concat.py~
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 quivr-0.0.1/quivr/coordinates.py~
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 quivr-0.0.1/quivr/defragment.py
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 quivr-0.0.1/quivr/defragment.py~
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 quivr-0.0.1/quivr/errors.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 quivr-0.0.1/quivr/errors.py~
--rw-r--r--   0        0        0     2333 2020-02-02 00:00:00.000000 quivr-0.0.1/quivr/indexing.py
--rw-r--r--   0        0        0     2339 2020-02-02 00:00:00.000000 quivr-0.0.1/quivr/indexing.py~
--rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 quivr-0.0.1/quivr/matrix.py
--rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 quivr-0.0.1/quivr/matrix.py~
--rw-r--r--   0        0        0     7644 2020-02-02 00:00:00.000000 quivr-0.0.1/quivr/models.py~
--rw-r--r--   0        0        0     7716 2020-02-02 00:00:00.000000 quivr-0.0.1/quivr/quiver.py~
--rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 quivr-0.0.1/quivr/schemagraph.py
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 quivr-0.0.1/quivr/schemagraph.py~
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 quivr-0.0.1/quivr/struct_demo.py~
--rw-r--r--   0        0        0    13053 2020-02-02 00:00:00.000000 quivr-0.0.1/quivr/tables.py
--rw-r--r--   0        0        0    13056 2020-02-02 00:00:00.000000 quivr-0.0.1/quivr/tables.py~
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 quivr-0.0.1/.gitignore
--rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 quivr-0.0.1/LICENSE
--rw-r--r--   0        0        0     8334 2020-02-02 00:00:00.000000 quivr-0.0.1/README.md
--rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 quivr-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     8732 2020-02-02 00:00:00.000000 quivr-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 quivr-0.1.0/quivr/__init__.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 quivr-0.1.0/quivr/__init__.py~
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 quivr-0.1.0/quivr/__version__.py
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 quivr-0.1.0/quivr/__version__.py~
+-rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 quivr-0.1.0/quivr/concat.py
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 quivr-0.1.0/quivr/concat.py~
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 quivr-0.1.0/quivr/coordinates.py~
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 quivr-0.1.0/quivr/defragment.py
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 quivr-0.1.0/quivr/defragment.py~
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 quivr-0.1.0/quivr/errors.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 quivr-0.1.0/quivr/errors.py~
+-rw-r--r--   0        0        0     2333 2020-02-02 00:00:00.000000 quivr-0.1.0/quivr/indexing.py
+-rw-r--r--   0        0        0     2339 2020-02-02 00:00:00.000000 quivr-0.1.0/quivr/indexing.py~
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 quivr-0.1.0/quivr/matrix.py
+-rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 quivr-0.1.0/quivr/matrix.py~
+-rw-r--r--   0        0        0     7644 2020-02-02 00:00:00.000000 quivr-0.1.0/quivr/models.py~
+-rw-r--r--   0        0        0     7716 2020-02-02 00:00:00.000000 quivr-0.1.0/quivr/quiver.py~
+-rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 quivr-0.1.0/quivr/schemagraph.py
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 quivr-0.1.0/quivr/schemagraph.py~
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 quivr-0.1.0/quivr/streaming.py
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 quivr-0.1.0/quivr/streaming.py~
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 quivr-0.1.0/quivr/struct_demo.py~
+-rw-r--r--   0        0        0    16606 2020-02-02 00:00:00.000000 quivr-0.1.0/quivr/tables.py
+-rw-r--r--   0        0        0    13056 2020-02-02 00:00:00.000000 quivr-0.1.0/quivr/tables.py~
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 quivr-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 quivr-0.1.0/LICENSE
+-rw-r--r--   0        0        0     8334 2020-02-02 00:00:00.000000 quivr-0.1.0/README.md
+-rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 quivr-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     8732 2020-02-02 00:00:00.000000 quivr-0.1.0/PKG-INFO
```

### Comparing `quivr-0.0.1/quivr/concat.py` & `quivr-0.1.0/quivr/concat.py`

 * *Files identical despite different names*

### Comparing `quivr-0.0.1/quivr/coordinates.py~` & `quivr-0.1.0/quivr/coordinates.py~`

 * *Files identical despite different names*

### Comparing `quivr-0.0.1/quivr/indexing.py` & `quivr-0.1.0/quivr/indexing.py`

 * *Files identical despite different names*

### Comparing `quivr-0.0.1/quivr/indexing.py~` & `quivr-0.1.0/quivr/indexing.py~`

 * *Files identical despite different names*

### Comparing `quivr-0.0.1/quivr/matrix.py` & `quivr-0.1.0/quivr/matrix.py`

 * *Files identical despite different names*

### Comparing `quivr-0.0.1/quivr/matrix.py~` & `quivr-0.1.0/quivr/matrix.py~`

 * *Files identical despite different names*

### Comparing `quivr-0.0.1/quivr/models.py~` & `quivr-0.1.0/quivr/models.py~`

 * *Files identical despite different names*

### Comparing `quivr-0.0.1/quivr/quiver.py~` & `quivr-0.1.0/quivr/quiver.py~`

 * *Files identical despite different names*

### Comparing `quivr-0.0.1/quivr/schemagraph.py` & `quivr-0.1.0/quivr/schemagraph.py`

 * *Files identical despite different names*

### Comparing `quivr-0.0.1/quivr/struct_demo.py~` & `quivr-0.1.0/quivr/struct_demo.py~`

 * *Files identical despite different names*

### Comparing `quivr-0.0.1/quivr/tables.py` & `quivr-0.1.0/quivr/tables.py~`

 * *Files 2% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 import pyarrow.compute as pc
 import pyarrow.feather
 import pyarrow.parquet
 
 from .errors import TableFragmentedError
 from .schemagraph import _walk_schema, compute_depth
 
-_METADATA_MODEL_KEY = b"__quivr_model_pickle"
-_METADATA_NAME_KEY = b"__quivr_model_name"
-_METADATA_UNPICKLE_KWARGS_KEY = b"__quivr_model_unpickle_kwargs"
+_METADATA_MODEL_KEY = b"__quiver_model_pickle"
+_METADATA_NAME_KEY = b"__quiver_model_name"
+_METADATA_UNPICKLE_KWARGS_KEY = b"__quiver_model_unpickle_kwargs"
 
 
 class TableMetaclass(type):
     """TableMetaclass is a metaclass which attaches accessors
     to Tables based on their schema class-level attribute.
 
     Each field in the class's schema becomes an attribute on the class.
```

### Comparing `quivr-0.0.1/quivr/tables.py~` & `quivr-0.1.0/quivr/tables.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,29 @@
+"""Table base classes."""
+
 import functools
 import pickle
 from typing import Any, Optional, Self, Union
+from io import IOBase
+import os
 
 import numpy as np
 import pandas as pd
 import pyarrow as pa
 import pyarrow.compute as pc
+import pyarrow.csv
 import pyarrow.feather
 import pyarrow.parquet
 
 from .errors import TableFragmentedError
 from .schemagraph import _walk_schema, compute_depth
 
-_METADATA_MODEL_KEY = b"__quiver_model_pickle"
-_METADATA_NAME_KEY = b"__quiver_model_name"
-_METADATA_UNPICKLE_KWARGS_KEY = b"__quiver_model_unpickle_kwargs"
+_METADATA_MODEL_KEY = b"__quivr_model_pickle"
+_METADATA_NAME_KEY = b"__quivr_model_name"
+_METADATA_UNPICKLE_KWARGS_KEY = b"__quivr_model_unpickle_kwargs"
 
 
 class TableMetaclass(type):
     """TableMetaclass is a metaclass which attaches accessors
     to Tables based on their schema class-level attribute.
 
     Each field in the class's schema becomes an attribute on the class.
@@ -67,31 +72,73 @@
 
 class TableBase(metaclass=TableMetaclass):
     table: pa.Table
     schema: pa.Schema = pa.schema([])
     _schema_depth: int
 
     def __init__(self, table: pa.Table):
+        self.table = []
         if not isinstance(table, pa.Table):
-            raise TypeError(f"Data must be a pyarrow.Table for {self.__class__.__name__}")
+            raise TypeError(
+                f"Data must be a pyarrow.Table for {self.__class__.__name__}"
+            )
         if table.schema != self.schema:
-            raise TypeError(f"Data schema must match schema for {self.__class__.__name__}")
+            raise TypeError(
+                f"Data schema must match schema for {self.__class__.__name__}"
+            )
         self.table = table
 
     @classmethod
     def from_arrays(cls, arrays: list[pa.array]):
+        """Create a TableBase object from a list of arrays.
+
+        Args:
+            arrays: A list of pyarrow.Array objects.
+
+        Returns:
+            A TableBase object.
+
+        """
         table = pa.Table.from_arrays(arrays, schema=cls.schema)
         return cls(table=table)
 
     @classmethod
     def from_pydict(cls, d: dict[str, Union[pa.array, list, np.ndarray]]):
         table = pa.Table.from_pydict(d, schema=cls.schema)
         return cls(table=table)
 
     @classmethod
+    def from_pylist(cls, l: list):
+        """
+        Create a TableBase object from a list of values.
+
+        Nested and hierarchical values can be represented as dictionaries in the list.
+
+        Args:
+            l: A list of values. Each value corresponds to a row in the table.
+
+        Returns:
+            A TableBase object.
+
+        Examples:
+            >>> import quivr
+            >>> class Inner(quivr.TableBase):
+            ...     schema = pyarrow.schema([pyarrow.field("a", pyarrow.string())])
+            ...
+            >>> class Outer(quivr.TableBase):
+            ...     schema = pyarrow.schema([pyarrow.field("z", pyarrow.string()), Inner.as_field("i")])
+            ...
+            >>> data = [{"z": "v1", "i": {"a": "v1_in"}}, {"z": "v2", "i": {"a": "v2_in"}}]
+            >>> Outer.from_pylist(data)
+            Outer(size=2)
+        """
+        table = pa.Table.from_pylist(l, schema=cls.schema)
+        return cls(table=table)
+
+    @classmethod
     def from_dataframe(cls, df: pd.DataFrame):
         """Load a DataFrame into the Table.
 
         If the DataFrame is missing any of the Table's columns, an
         error is raised. If the DataFrame has extra columns, they are
         ignored.
 
@@ -101,14 +148,56 @@
         unflattened DataFrame, or use from_flat_dataframe.
         """
 
         table = pa.Table.from_pandas(df, schema=cls.schema)
         return cls(table=table)
 
     @classmethod
+    def _unflatten_table(cls, table: pa.Table):
+        """Unflatten a Table.
+
+        This is used when loading a flattened DataFrame into a nested
+        Table. It takes a Table with a flat schema, and returns a
+        Table with a nested schema.
+
+        """
+        struct_fields = []
+
+        for field in cls.schema:
+            if pa.types.is_struct(field.type):
+                struct_fields.append(field)
+
+        if len(struct_fields) == 0:
+            return cls(table=pa.from_dataframe(df, schema=cls.schema))
+
+        # Walk the schema, and build a StructArray for each embedded
+        # type.
+
+        def struct_array_for(field: pa.Field, ancestors: list[pa.Field]):
+            prefix = ".".join([f.name for f in ancestors if f.name] + [field.name])
+
+            child_arrays = []
+            for subfield in field.type:
+                if pa.types.is_struct(subfield.type):
+                    child_arrays.append(struct_array_for(subfield, ancestors + [field]))
+                else:
+                    path = prefix + "." + subfield.name
+                    child_arrays.append(table.column(path).combine_chunks())
+            return pa.StructArray.from_arrays(child_arrays, fields=list(field.type))
+
+        child_arrays = []
+        for field in cls.schema:
+            if pa.types.is_struct(field.type):
+                child_arrays.append(struct_array_for(field, []))
+            else:
+                child_arrays.append(table.column(field.name).combine_chunks())
+
+        return pa.Table.from_arrays(child_arrays, schema=cls.schema)
+
+    @classmethod
     def from_flat_dataframe(cls, df: pd.DataFrame):
         """Load a flattened DataFrame into the Table.
 
         known bug: Doesn't correctly interpret fixed-length lists.
         """
         struct_fields = []
         for field in cls.schema:
@@ -267,32 +356,38 @@
         """
         table = self.table
         if flatten:
             table = self.flattened_table()
         return table.to_pandas()
 
     @classmethod
-    def as_field(cls, name: str, nullable: bool = True, metadata: Optional[dict] = None):
+    def as_field(
+        cls, name: str, nullable: bool = True, metadata: Optional[dict] = None
+    ):
         metadata = metadata or {}
         metadata[_METADATA_NAME_KEY] = cls.__name__
         metadata[_METADATA_MODEL_KEY] = pickle.dumps(cls)
-        field = pa.field(name, pa.struct(cls.schema), nullable=nullable, metadata=metadata)
+        field = pa.field(
+            name, pa.struct(cls.schema), nullable=nullable, metadata=metadata
+        )
         return field
 
     def column(self, field_name: str):
         field = self.schema.field(field_name)
         if field.metadata is not None and _METADATA_MODEL_KEY in field.metadata:
             # If the field has type information attached to it in
             # metadata, pull it out. The metadata store the model (as
             # a class object), and may optionally have some keyword
             # arguments to be used when instantiating the model from
             # the data.
             model = pickle.loads(field.metadata[_METADATA_MODEL_KEY])
             if _METADATA_UNPICKLE_KWARGS_KEY in field.metadata:
-                init_kwargs = pickle.loads(field.metadata[_METADATA_UNPICKLE_KWARGS_KEY])
+                init_kwargs = pickle.loads(
+                    field.metadata[_METADATA_UNPICKLE_KWARGS_KEY]
+                )
             else:
                 init_kwargs = {}
             table = _sub_table(self.table, field_name)
             return model(table=table, **init_kwargs)
         return self.table.column(field_name)
 
     def __repr__(self):
@@ -306,14 +401,19 @@
             return self.__class__(self.table[idx : idx + 1])
         return self.__class__(self.table[idx])
 
     def __iter__(self):
         for i in range(len(self)):
             yield self[i : i + 1]
 
+    def __eq__(self, other):
+        if not isinstance(other, TableBase):
+            return NotImplemented
+        return self.table.equals(other.table)
+
     def take(self, row_indices: Union[list[int], pa.IntegerArray]) -> Self:
         """Return a new Table with only the rows at the given indices."""
         return self.__class__(self.table.take(row_indices))
 
     def to_parquet(self, path: str, **kwargs):
         """Write the table to a Parquet file."""
         pyarrow.parquet.write_table(self.table, path, **kwargs)
@@ -326,15 +426,25 @@
     def to_feather(self, path: str, **kwargs):
         """Write the table to a Feather file."""
         pyarrow.feather.write_feather(self.table, path, **kwargs)
 
     @classmethod
     def from_feather(cls, path: str, **kwargs):
         """Read a table from a Feather file."""
-        return cls(table=pyarrow.feather.read_feather(path, **kwargs))
+        return cls(table=pyarrow.feather.read_table(path, **kwargs))
+
+    def to_csv(self, path: str):
+        """Write the table to a CSV file. Any nested structure is flattened."""
+        pyarrow.csv.write_csv(self.flattened_table(), path)
+
+    @classmethod
+    def from_csv(cls, input_file: Union[str, os.PathLike, IOBase]):
+        """Read a table from a CSV file."""
+        flat_table = pyarrow.csv.read_csv(input_file)
+        return cls(table=cls._unflatten_table(flat_table))
 
 
 def _sub_table(tab: pa.Table, field_name: str):
     """Given a table which contains a StructArray under given field
     name, construct a table from the sub-object.
 
     """
```

### Comparing `quivr-0.0.1/LICENSE` & `quivr-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `quivr-0.0.1/README.md` & `quivr-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `quivr-0.0.1/pyproject.toml` & `quivr-0.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `quivr-0.0.1/PKG-INFO` & `quivr-0.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quivr
-Version: 0.0.1
+Version: 0.1.0
 Summary: Container library for working with tabular Arrow data
 Project-URL: Source, https://github.com/spenczar/quivr
 Author-email: Spencer Nelson <spencer@spencerwnelson.com>
 License-File: LICENSE
 Requires-Python: >=3.11
 Requires-Dist: mmh3
 Requires-Dist: numpy
```

