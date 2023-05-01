# Comparing `tmp/pgmini-0.1.4.tar.gz` & `tmp/pgmini-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pgmini-0.1.4.tar", max compression
+gzip compressed data, was "pgmini-0.1.5.tar", max compression
```

## Comparing `pgmini-0.1.4.tar` & `pgmini-0.1.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1461 2023-02-19 07:19:37.209313 pgmini-0.1.4/LICENSE
--rw-r--r--   0        0        0     7773 2023-04-03 05:59:48.504852 pgmini-0.1.4/README.md
--rw-r--r--   0        0        0     2054 2023-04-22 06:25:52.799975 pgmini-0.1.4/pgmini/__init__.py
--rw-r--r--   0        0        0      614 2023-02-24 08:44:04.617355 pgmini-0.1.4/pgmini/alias.py
--rw-r--r--   0        0        0      804 2023-02-23 11:58:37.582351 pgmini-0.1.4/pgmini/array.py
--rw-r--r--   0        0        0     1854 2023-02-23 11:58:37.573751 pgmini-0.1.4/pgmini/case.py
--rw-r--r--   0        0        0      874 2023-02-24 08:43:54.427071 pgmini-0.1.4/pgmini/cast.py
--rw-r--r--   0        0        0     1663 2023-02-23 11:58:37.566136 pgmini-0.1.4/pgmini/column.py
--rw-r--r--   0        0        0     1540 2023-02-24 08:45:15.018968 pgmini-0.1.4/pgmini/delete.py
--rw-r--r--   0        0        0      272 2023-02-23 06:15:18.337495 pgmini-0.1.4/pgmini/distinct.py
--rw-r--r--   0        0        0     4358 2023-03-10 11:05:47.770188 pgmini-0.1.4/pgmini/func.py
--rw-r--r--   0        0        0     6736 2023-03-10 11:20:29.617469 pgmini-0.1.4/pgmini/insert.py
--rw-r--r--   0        0        0     2018 2023-02-23 11:58:37.595454 pgmini-0.1.4/pgmini/literal.py
--rw-r--r--   0        0        0     2010 2023-02-27 06:30:22.659219 pgmini-0.1.4/pgmini/marks.py
--rw-r--r--   0        0        0     2687 2023-02-23 06:15:18.320773 pgmini-0.1.4/pgmini/operation.py
--rw-r--r--   0        0        0     6891 2023-04-01 15:12:57.306865 pgmini-0.1.4/pgmini/operations.py
--rw-r--r--   0        0        0     2829 2023-02-23 11:58:37.588950 pgmini-0.1.4/pgmini/operators.py
--rw-r--r--   0        0        0     1616 2023-02-24 08:44:04.622843 pgmini-0.1.4/pgmini/order_by.py
--rw-r--r--   0        0        0     1037 2023-02-23 11:58:37.570082 pgmini-0.1.4/pgmini/param.py
--rw-r--r--   0        0        0     9441 2023-02-24 08:45:15.014120 pgmini-0.1.4/pgmini/select.py
--rw-r--r--   0        0        0     1711 2023-02-23 11:57:58.880457 pgmini-0.1.4/pgmini/subquery.py
--rw-r--r--   0        0        0     1134 2023-02-23 09:40:15.343020 pgmini-0.1.4/pgmini/table.py
--rw-r--r--   0        0        0     2576 2023-02-24 08:45:15.029030 pgmini-0.1.4/pgmini/update.py
--rw-r--r--   0        0        0     2825 2023-02-26 06:21:00.926047 pgmini-0.1.4/pgmini/utils.py
--rw-r--r--   0        0        0      901 2023-04-22 06:27:53.347307 pgmini-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     8815 1970-01-01 00:00:00.000000 pgmini-0.1.4/setup.py
--rw-r--r--   0        0        0     8238 1970-01-01 00:00:00.000000 pgmini-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1461 2023-02-19 07:19:37.209313 pgmini-0.1.5/LICENSE
+-rw-r--r--   0        0        0     7773 2023-04-03 05:59:48.504852 pgmini-0.1.5/README.md
+-rw-r--r--   0        0        0     2259 2023-05-01 05:08:31.710026 pgmini-0.1.5/pgmini/__init__.py
+-rw-r--r--   0        0        0      614 2023-02-24 08:44:04.617355 pgmini-0.1.5/pgmini/alias.py
+-rw-r--r--   0        0        0      811 2023-05-01 05:08:02.585539 pgmini-0.1.5/pgmini/array.py
+-rw-r--r--   0        0        0     1861 2023-05-01 05:08:02.603966 pgmini-0.1.5/pgmini/case.py
+-rw-r--r--   0        0        0      946 2023-05-01 05:08:50.018185 pgmini-0.1.5/pgmini/cast.py
+-rw-r--r--   0        0        0     1670 2023-05-01 05:08:02.579642 pgmini-0.1.5/pgmini/column.py
+-rw-r--r--   0        0        0     1547 2023-05-01 05:08:02.600431 pgmini-0.1.5/pgmini/delete.py
+-rw-r--r--   0        0        0      272 2023-02-23 06:15:18.337495 pgmini-0.1.5/pgmini/distinct.py
+-rw-r--r--   0        0        0     4365 2023-05-01 05:08:02.612565 pgmini-0.1.5/pgmini/func.py
+-rw-r--r--   0        0        0     6743 2023-05-01 05:08:02.596689 pgmini-0.1.5/pgmini/insert.py
+-rw-r--r--   0        0        0     2025 2023-05-01 05:08:02.588339 pgmini-0.1.5/pgmini/literal.py
+-rw-r--r--   0        0        0     2010 2023-02-27 06:30:22.659219 pgmini-0.1.5/pgmini/marks.py
+-rw-r--r--   0        0        0     2687 2023-02-23 06:15:18.320773 pgmini-0.1.5/pgmini/operation.py
+-rw-r--r--   0        0        0     6954 2023-05-01 05:08:16.877681 pgmini-0.1.5/pgmini/operations.py
+-rw-r--r--   0        0        0     2850 2023-05-01 05:08:02.582903 pgmini-0.1.5/pgmini/operators.py
+-rw-r--r--   0        0        0     1616 2023-02-24 08:44:04.622843 pgmini-0.1.5/pgmini/order_by.py
+-rw-r--r--   0        0        0     1184 2023-05-01 05:01:36.361544 pgmini-0.1.5/pgmini/param.py
+-rw-r--r--   0        0        0     9462 2023-05-01 05:08:02.592762 pgmini-0.1.5/pgmini/select.py
+-rw-r--r--   0        0        0     1718 2023-05-01 05:08:02.571006 pgmini-0.1.5/pgmini/subquery.py
+-rw-r--r--   0        0        0     1134 2023-02-23 09:40:15.343020 pgmini-0.1.5/pgmini/table.py
+-rw-r--r--   0        0        0     2583 2023-05-01 05:08:02.615662 pgmini-0.1.5/pgmini/update.py
+-rw-r--r--   0        0        0     2896 2023-05-01 05:08:02.607073 pgmini-0.1.5/pgmini/utils.py
+-rw-r--r--   0        0        0      901 2023-05-01 05:08:41.372640 pgmini-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     8815 1970-01-01 00:00:00.000000 pgmini-0.1.5/setup.py
+-rw-r--r--   0        0        0     8238 1970-01-01 00:00:00.000000 pgmini-0.1.5/PKG-INFO
```

### Comparing `pgmini-0.1.4/LICENSE` & `pgmini-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pgmini-0.1.4/README.md` & `pgmini-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `pgmini-0.1.4/pgmini/__init__.py` & `pgmini-0.1.5/pgmini/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from contextvars import copy_context
+from typing import Literal as TypeLiteral
 
 import attrs
 
 from .array import Array
 from .case import Case
 from .column import Excluded
 from .delete import Delete
@@ -21,15 +22,15 @@
     CTX_DISABLE_TABLE_IN_COLUMN,
     CTX_FORCE_CAST_BRACKETS,
     CTX_TABLES,
     CompileABC,
 )
 
 
-__version__ = '0.1.4'
+__version__ = '0.1.5'
 __all__ = (
     'And',
     'Array',
     'Case',
     'Delete',
     'Excluded',
     'Exists',
@@ -72,17 +73,26 @@
     def Update(self, table: Table) -> Update:
         return Update(table, x_with=self._subqueries)
 
     def Delete(self, table: Table) -> Delete:
         return Delete(table, x_with=self._subqueries)
 
 
-def build(item: CompileABC) -> tuple[str | None, list]:
+def build(
+    item: CompileABC,
+    driver: TypeLiteral['asyncpg', 'psycopg'] = 'asyncpg',
+) -> tuple[str | None, list | dict]:
     def run():
         CTX_FORCE_CAST_BRACKETS.set(False)
         CTX_CTE.set(())
         CTX_TABLES.set(())
         CTX_ALIAS_ONLY.set(False)
         CTX_DISABLE_TABLE_IN_COLUMN.set(False)
-        return item._build(params := []), params
+
+        if driver == 'asyncpg':
+            params = []
+        else:
+            params = {}
+
+        return item._build(params), params
 
     return copy_context().run(run)
```

### Comparing `pgmini-0.1.4/pgmini/alias.py` & `pgmini-0.1.5/pgmini/alias.py`

 * *Files identical despite different names*

### Comparing `pgmini-0.1.4/pgmini/array.py` & `pgmini-0.1.5/pgmini/array.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 @attrs.frozen(eq=False)
 class Array(CompileABC, CastMX, AliasMX, OperationMX, SelectMX):
     _items: tuple[CompileABC, ...] = attrs.field(alias='items', converter=_convert_items)
     _marks: MARKS_TYPE = MARKS_FIELD
 
-    def _build(self, params: list) -> str:
+    def _build(self, params: list | dict) -> str:
         if alias := extract_alias(self):
             return alias
 
         res = 'ARRAY[%s]' % ', '.join(i._build(params) for i in self._items)
         if self._marks:
             res = self._marks.build(res)
         return res
```

### Comparing `pgmini-0.1.4/pgmini/case.py` & `pgmini-0.1.5/pgmini/case.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,15 +38,15 @@
             raise TypeError(bad)
 
     def __init__(self, *statements: tuple[Any, Any], Else=None, **kwargs):
         kwargs.setdefault('statements', statements)
         kwargs.setdefault('x_else', Else)
         self.__attrs_init__(**kwargs)
 
-    def _build(self, params: list) -> str:
+    def _build(self, params: list | dict) -> str:
         if alias := extract_alias(self):
             return alias
 
         parts = []
         for op, val in self._statements:
             parts.append('WHEN %s THEN %s' % (op._build(params), val._build(params)))
         if self._else is not None:
```

### Comparing `pgmini-0.1.4/pgmini/cast.py` & `pgmini-0.1.5/pgmini/cast.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from .marks import Marks
 from .utils import (
     CTX_FORCE_CAST_BRACKETS,
     RE_ARRAY,
     RE_FUNC_PARENTHESIZED,
     RE_NEED_BRACKETS,
     RE_PARENTHESIZED,
+    RE_PSYCOPG_PARAM,
     RE_SINGLE_QUOTED,
 )
 
 
 class CastMX:
     def Cast(self, to: str):
         if self._marks:
@@ -23,13 +24,14 @@
 def build_cast(value: str, cast: str) -> str:
     if (
         RE_NEED_BRACKETS.search(value)
         and not RE_PARENTHESIZED.fullmatch(value)
         and not RE_FUNC_PARENTHESIZED.fullmatch(value)
         and not RE_SINGLE_QUOTED.fullmatch(value)
         and not RE_ARRAY.fullmatch(value)
+        and not RE_PSYCOPG_PARAM.fullmatch(value)
     ):
         value = '(%s)' % value
     value = '%s::%s' % (value, cast)
     if CTX_FORCE_CAST_BRACKETS.get():
         value = '(%s)' % value
     return value
```

### Comparing `pgmini-0.1.4/pgmini/column.py` & `pgmini-0.1.5/pgmini/column.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 @attrs.frozen(eq=False, unsafe_hash=True)
 class Column(CompileABC, CastMX, AliasMX, DistinctMX, OrderByMX, OperationMX, SelectMX):
     _name: str = attrs.field(alias='name')
     _table: FromABC | None = attrs.field(alias='table', default=None)
     _marks: MARKS_TYPE = MARKS_FIELD
 
-    def _build(self, params: list) -> str:
+    def _build(self, params: list | dict) -> str:
         if alias := extract_alias(self):
             return alias
 
         res = self._name
         if (
             not CTX_DISABLE_TABLE_IN_COLUMN.get()
             and (
```

### Comparing `pgmini-0.1.4/pgmini/delete.py` & `pgmini-0.1.5/pgmini/delete.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
     def Returning(self, *columns):
         return attrs.evolve(self, x_returning=columns)
 
     def Subquery(self, alias: str, materialized: bool = False) -> Subquery:
         return Subquery(self, alias=alias, materialized=materialized)
 
-    def _build(self, params: list) -> str:
+    def _build(self, params: list | dict) -> str:
         parts = []
         if self._with:
             if CTX_CTE.get():
                 raise ValueError
             CTX_CTE.set(self._with)
             parts.append(build_with(self._with, params))
```

### Comparing `pgmini-0.1.4/pgmini/func.py` & `pgmini-0.1.5/pgmini/func.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,15 @@
 
     def Where(self, *statements: CompileABC):
         return attrs.evolve(self, x_where=statements)
 
     def OrderBy(self, *statements):
         return do_order_by(self, statements)
 
-    def _build(self, params: list) -> str:
+    def _build(self, params: list | dict) -> str:
         if alias := extract_alias(self):
             return alias
 
         args = ', '.join(
             (
                 STAR_SIGN
                 if isinstance(i, Literal) and i._value == STAR_SIGN and self._name == 'COUNT'
```

### Comparing `pgmini-0.1.4/pgmini/insert.py` & `pgmini-0.1.5/pgmini/insert.py`

 * *Files 0% similar despite different names*

```diff
@@ -172,15 +172,15 @@
 
     def Returning(self, *columns):
         return attrs.evolve(self, x_returning=columns)
 
     def Subquery(self, alias: str, materialized: bool = False) -> Subquery:
         return Subquery(self, alias=alias, materialized=materialized)
 
-    def _build(self, params: list) -> str:
+    def _build(self, params: list | dict) -> str:
         parts = []
         if self._with:
             if CTX_CTE.get():
                 raise ValueError
             CTX_CTE.set(self._with)
             parts.append(build_with(self._with, params))
```

### Comparing `pgmini-0.1.4/pgmini/literal.py` & `pgmini-0.1.5/pgmini/literal.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     def _vld_value(self, attribute, value):
         if isinstance(value, tuple):
             if not value:
                 raise ValueError(value)
             elif bad := [i for i in value if type(i) not in _TYPES]:
                 raise TypeError(bad)
 
-    def _build(self, params: list) -> str:
+    def _build(self, params: list | dict) -> str:
         if alias := extract_alias(self):
             return alias
 
         if handler := _TYPES.get(type(self._value)):
             res = handler(self._value)
         elif isinstance(self._value, tuple):
             res = "ARRAY[%s]" % ', '.join(_TYPES[type(i)](i) for i in self._value)
```

### Comparing `pgmini-0.1.4/pgmini/marks.py` & `pgmini-0.1.5/pgmini/marks.py`

 * *Files identical despite different names*

### Comparing `pgmini-0.1.4/pgmini/operation.py` & `pgmini-0.1.5/pgmini/operation.py`

 * *Files identical despite different names*

### Comparing `pgmini-0.1.4/pgmini/operations.py` & `pgmini-0.1.5/pgmini/operations.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,30 +27,30 @@
 
 @attrs.frozen(eq=False)
 class Operation(CompileABC, CastMX, AliasMX, DistinctMX, OrderByMX, OperationMX, SelectMX):
     _left: Any = attrs.field(alias='left')
     _right: Any = attrs.field(alias='right', converter=_convert_right)
     _marks: MARKS_TYPE = MARKS_FIELD
 
-    def _build(self, params: list) -> str:
+    def _build(self, params: list | dict) -> str:
         raise NotImplementedError
 
 
 _NULL_BOOL: Final[tuple] = (type(None), bool)
 
 
 def _check_null_or_bool(left, right) -> bool:
     for i in (left, right):
         if isinstance(i, (Literal, Param)) and isinstance(i._value, _NULL_BOOL):
             return True
 
     return False
 
 
-def _build(elem, params: list) -> str:
+def _build(elem, params: list | dict) -> str:
     from .select import Select
 
     res = elem._build(params)
     if (
         (isinstance(elem, Operation) and not RE_PARENTHESIZED.fullmatch(res))
         or isinstance(elem, Select)
     ):
@@ -72,15 +72,15 @@
 
     def __attrs_post_init__(self):
         if self._operator_equal is _NOT_SET:
             raise ValueError
         elif self._operator_is is _NOT_SET:
             raise ValueError
 
-    def _build(self, params: list) -> str:
+    def _build(self, params: list | dict) -> str:
         if alias := extract_alias(self):
             return alias
 
         if _check_null_or_bool(self._left, self._right):
             op = self._operator_is
         else:
             op = self._operator_equal
@@ -103,15 +103,15 @@
 class OperationMath(Operation):
     _operator: str = attrs.field(alias='operator', default=_NOT_SET)
 
     def __attrs_post_init__(self):
         if self._operator is _NOT_SET:
             raise ValueError
 
-    def _build(self, params: list) -> str:
+    def _build(self, params: list | dict) -> str:
         if alias := extract_alias(self):
             return alias
 
         expr = '%s %s %s' % (
             _wrap_operation_member(self._left),
             self._operator,
             _wrap_operation_member(self._right),
@@ -145,15 +145,15 @@
     _items: CompileABC | tuple[CompileABC, ...] = attrs.field(
         alias='items',
         converter=_convert_items,
     )
     _marks: MARKS_TYPE = MARKS_FIELD
     _operator: str = attrs.field(alias='operator', default='IN')
 
-    def _build(self, params: list) -> str:
+    def _build(self, params: list | dict) -> str:
         if alias := extract_alias(self):
             return alias
 
         expr = '%s %s' % (_wrap_operation_member(self._left), self._operator)
         res = expr % _build(self._left, params)
 
         if isinstance(self._items, tuple):
@@ -169,15 +169,15 @@
 @attrs.frozen(eq=False)
 class OperationBetween(CompileABC, CastMX, AliasMX, DistinctMX, OrderByMX, OperationMX, SelectMX):
     _left: Any = attrs.field(alias='left')
     _start: CompileABC = attrs.field(alias='start', converter=prepare_column)
     _end: CompileABC = attrs.field(alias='end', converter=prepare_column)
     _marks: MARKS_TYPE = MARKS_FIELD
 
-    def _build(self, params: list) -> str:
+    def _build(self, params: list | dict) -> str:
         if alias := extract_alias(self):
             return alias
 
         expr = '%s BETWEEN %%s AND %%s' % _wrap_operation_member(self._left)
         res = expr % (
             _build(self._left, params),
             _build(self._start, params),
@@ -186,15 +186,15 @@
         if self._marks:
             res = self._marks.build(res)
         return res
 
 
 @attrs.frozen(eq=False)
 class OperationAny(Operation):
-    def _build(self, params: list) -> str:
+    def _build(self, params: list | dict) -> str:
         if alias := extract_alias(self):
             return alias
 
         expr = '%s = ANY(%%s)' % _wrap_operation_member(self._left)
         res = expr % (
             _build(self._left, params),
             _build(self._right, params),
@@ -204,15 +204,15 @@
         return res
 
 
 @attrs.frozen(eq=False)
 class OperationLike(Operation):
     _operator: str = attrs.field(alias='operator', default='LIKE')
 
-    def _build(self, params: list) -> str:
+    def _build(self, params: list | dict) -> str:
         if alias := extract_alias(self):
             return alias
 
         expr = '%s %%s %%s' % _wrap_operation_member(self._left)
         res = expr % (
             _build(self._left, params),
             self._operator,
@@ -227,15 +227,15 @@
 class OperationCustom(Operation):
     _operator: str = attrs.field(alias='operator', default=_NOT_SET)
 
     def __attrs_post_init__(self):
         if self._operator is _NOT_SET:
             raise ValueError
 
-    def _build(self, params: list) -> str:
+    def _build(self, params: list | dict) -> str:
         if alias := extract_alias(self):
             return alias
 
         expr = '%s %s %%s' % (_wrap_operation_member(self._left), self._operator)
         res = expr % (
             _build(self._left, params),
             _build(self._right, params),
```

### Comparing `pgmini-0.1.4/pgmini/operators.py` & `pgmini-0.1.5/pgmini/operators.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         if not all(i is not None for i in value):
             raise ValueError(value)
 
     def __init__(self, *statements: CompileABC, **kwargs):
         kwargs.setdefault('statements', statements)
         self.__attrs_init__(**kwargs)
 
-    def _build(self, params: list) -> str | None:
+    def _build(self, params: list | dict) -> str | None:
         if not self._statements:
             return
         elif alias := extract_alias(self):
             return alias
 
         if len(self._statements) == 1:
             res = self._statements[0]._build(params)
@@ -55,15 +55,15 @@
 
 
 @attrs.frozen(eq=False, repr=False)
 class Not(CompileABC, CastMX, AliasMX, DistinctMX, OrderByMX, OperationMX, SelectMX):
     _statement: CompileABC = attrs.field(alias='statement')
     _marks: MARKS_TYPE = MARKS_FIELD
 
-    def _build(self, params: list) -> str:
+    def _build(self, params: list | dict) -> str:
         from .operations import Operation
 
         if alias := extract_alias(self):
             return alias
 
         if isinstance(self._statement, Operation):
             expr = 'NOT %s'
@@ -79,15 +79,15 @@
         if self._marks:
             res += f':{repr(self._marks)}'
         return res
 
 
 @attrs.frozen(eq=False, repr=False)
 class Exists(Not):
-    def _build(self, params: list) -> str:
+    def _build(self, params: list | dict) -> str:
         if alias := extract_alias(self):
             return alias
 
         res = 'EXISTS (%s)' % self._statement._build(params)
         if self._marks:
             res = self._marks.build(res)
         return res
```

### Comparing `pgmini-0.1.4/pgmini/order_by.py` & `pgmini-0.1.5/pgmini/order_by.py`

 * *Files identical despite different names*

### Comparing `pgmini-0.1.4/pgmini/param.py` & `pgmini-0.1.5/pgmini/param.py`

 * *Files 25% similar despite different names*

```diff
@@ -13,21 +13,26 @@
 
 
 @attrs.frozen(repr=False, eq=False)
 class Param(CompileABC, CastMX, AliasMX, DistinctMX, OrderByMX, OperationMX, SelectMX):
     _value: Any = attrs.field(alias='value', converter=deepcopy)
     _marks: MARKS_TYPE = MARKS_FIELD
 
-    def _build(self, params: list) -> str:
+    def _build(self, params: list | dict) -> str:
         if alias := extract_alias(self):
             return alias
 
         index = len(params) + 1
-        params.append(self._value)
-        res = '$%d' % index
+        if isinstance(params, list):
+            params.append(self._value)
+            res = '$%d' % index
+        else:
+            params[f'p{index}'] = self._value
+            res = f'%(p{index})s'
+
         if self._marks:
             res = self._marks.build(res)
         return res
 
     def __repr__(self):
         res = 'Param(%s)' % str(self._value)
         if self._marks:
```

### Comparing `pgmini-0.1.4/pgmini/select.py` & `pgmini-0.1.5/pgmini/select.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 @attrs.frozen
 class _Join:
     type: LiteralT['left', 'right'] = attrs.field(validator=attrs.validators.in_({'left', 'right'}))
     table: FromABC
     on_statement: Any = attrs.field(converter=_convert_on_statement)
     lateral: bool = attrs.field(validator=attrs.validators.in_({True, False}), default=False)
 
-    def _build(self, params: list):
+    def _build(self, params: list | dict):
         if self.type == 'right':
             sql = 'JOIN'
         else:
             sql = 'LEFT JOIN'
 
         cte = self.table in CTX_CTE.get()
         if self.lateral:
@@ -62,15 +62,15 @@
 @attrs.frozen
 class _Union:
     type: LiteralT['distinct', 'all'] = attrs.field(
         validator=attrs.validators.in_({'distinct', 'all'}),
     )
     select: Select
 
-    def _build(self, params: list) -> str:
+    def _build(self, params: list | dict) -> str:
         expr = 'UNION'
         if self.type == 'all':
             expr = '%s ALL' % expr
         return '%s %s' % (expr, self.select._build(params))
 
 
 def _convert_columns(values):
@@ -215,15 +215,15 @@
 
     def Cast(self, to: str):
         return attrs.evolve(self, x_cast=to)
 
     def Subquery(self, alias: str, materialized: bool = False):
         return Subquery(self, alias=alias, materialized=materialized)
 
-    def _build(self, params: list) -> str:
+    def _build(self, params: list | dict) -> str:
         parts = []
 
         if self._with:
             if CTX_CTE.get():
                 raise ValueError
             CTX_CTE.set(self._with)
             parts.append(build_with(self._with, params))
```

### Comparing `pgmini-0.1.4/pgmini/subquery.py` & `pgmini-0.1.5/pgmini/subquery.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,9 +48,9 @@
 
     def _get_with_statement(self, params: list) -> str:
         res = '%s AS' % self._alias
         if self._materialized:
             res = '%s MATERIALIZED' % res
         return '%s (%s)' % (res, self._statement._build(params))
 
-    def _build(self, params: list) -> str:
+    def _build(self, params: list | dict) -> str:
         return self._get_from_statement(params)
```

### Comparing `pgmini-0.1.4/pgmini/table.py` & `pgmini-0.1.5/pgmini/table.py`

 * *Files identical despite different names*

### Comparing `pgmini-0.1.4/pgmini/update.py` & `pgmini-0.1.5/pgmini/update.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 
     def Returning(self, *columns):
         return attrs.evolve(self, x_returning=columns)
 
     def Subquery(self, alias: str, materialized: bool = False) -> Subquery:
         return Subquery(self, alias=alias, materialized=materialized)
 
-    def _build(self, params: list) -> str:
+    def _build(self, params: list | dict) -> str:
         if not self._set:
             raise ValueError
 
         parts = []
         if self._with:
             if CTX_CTE.get():
                 raise ValueError
```

### Comparing `pgmini-0.1.4/pgmini/utils.py` & `pgmini-0.1.5/pgmini/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 class SelectMX:
     pass
 
 
 class CompileABC(ABC):
     @abstractmethod
-    def _build(self, params: list) -> str | None:
+    def _build(self, params: list | dict) -> str | None:
         raise NotImplementedError
 
 
 class FromABC(ABC):
     @abstractmethod
     def _get_from_statement(self, params: list) -> str:
         raise NotImplementedError
@@ -26,14 +26,15 @@
 
 
 RE_NEED_BRACKETS: Final[Pattern] = re.compile("[^a-z0-9$._']", flags=re.IGNORECASE)
 RE_PARENTHESIZED: Final[Pattern] = re.compile(r'\(.*\)')
 RE_FUNC_PARENTHESIZED: Final[Pattern] = re.compile(r'[a-z0-9_.]+\([^()]*\)', flags=re.IGNORECASE)
 RE_SINGLE_QUOTED: Final[Pattern] = re.compile("'[^']*'")
 RE_ARRAY: Final[Pattern] = re.compile(r'ARRAY\[.*\]')
+RE_PSYCOPG_PARAM: Final[Pattern] = re.compile(r'%\(p[0-9]+\)s')
 ITERABLES: Final[tuple] = (list, tuple, set, frozenset)
 STAR_SIGN: Final[str] = '*'
 CTX_FORCE_CAST_BRACKETS: Final[ContextVar[bool]] = ContextVar('force_cast_brackets')
 CTX_CTE: Final[ContextVar[tuple]] = ContextVar('cte')
 CTX_DISABLE_TABLE_IN_COLUMN: Final[ContextVar[bool]] = ContextVar('disable_table_in_column')
 CTX_TABLES: Final[ContextVar[tuple[FromABC, ...]]] = ContextVar('tables')
 CTX_ALIAS_ONLY: Final[ContextVar[bool]] = ContextVar('alias_only')
```

### Comparing `pgmini-0.1.4/pyproject.toml` & `pgmini-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pgmini"
-version = "0.1.4"
+version = "0.1.5"
 description = "Build sql for PostgreSQL"
 authors = ["Vitalii Ponomar"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/ponomar/pgmini"
 
 [tool.poetry.dependencies]
```

### Comparing `pgmini-0.1.4/setup.py` & `pgmini-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['attrs>=22.2.0']
 
 setup_kwargs = {
     'name': 'pgmini',
-    'version': '0.1.4',
+    'version': '0.1.5',
     'description': 'Build sql for PostgreSQL',
     'long_description': '[![Test & Lint](https://github.com/ponomar/pgmini/actions/workflows/main.yml/badge.svg)](https://github.com/ponomar/pgmini/actions/workflows/main.yml)\n\n## 🇺🇦 What is pgmini? 🇺🇦\n\nIt is the PostgreSQL query builder with next core principles:\n- simple (predictable, without magic)\n- fast\n\nAll object are immutable (thanks to [attrs](https://www.attrs.org) lib).\nPython code as close to SQL structure as possible.\nLibrary doesn\'t try to be everything.\nIt doesn\'t manage connections to postgres, doesn\'t escape params.\nAll this can and should be done with other tools: (asyncpg, psycopg2, postgresql itself etc.).\n\nI\'ve decided to use `PascalCase` methods naming to avoid collisions with python reserved words: \n`From`, `And`, `Or`, `Else`, `With`, `As` etc.\n\n## Examples\n```python\nUser = Table(\'user\')  # dynamic columns\n\nq = Select(User.id, User.name).From(User).Where(User.email == \'test@test.com\')\n\nbuild(q)\n# (\n#     \'SELECT id, name FROM "user" WHERE email = $1\', \n#     [\'test@test.com\'],\n# )\n```\n\nExplicitly defined table schema allows to save filters and methods for further reusing \nand to use IDE code analyzers for smart completions, find usages, bulk refactors etc.  \n```python\nclass RoleSchema(Table):\n    id: int\n    name: str\n    status: str\n    \n    @property\n    def status_active(self):  # can also be decorated with functools.cache\n        return self.status == Literal(\'active\')\n    \n    def name_startswith(self, value: str):\n        return self.name.Like(f\'{value}%\')\n\nRole = RoleSchema(\'role\')\nq = Select(Role.id).From(Role).Where(Role.status_active, Role.name_startswith(\'admin\'))\n\nRoleAlias = Role.As(\'role2\')  # all columns/methods are visible for IDE live inspection as well\nq = (\n    Select(Role.STAR).From(Role)\n    .Where(Not(Exists(\n        Select(1).From(RoleAlias)\n        .Where(RoleAlias.id < Role.id, RoleAlias.status_active)\n    )))\n)\n```\n\n#### WHERE\nWhere takes *args which work like AND operator.\n```python\nt = Table(\'tbl\')\nq = (\n    Select(t.id).From(t)\n    .Where(\n        t.id.Between(10, 20), \n        Or(t.name > \'name\', And(t.status == \'active\', Not(t.id == 15))),\n    )\n)\n# SELECT id FROM tbl WHERE id BETWEEN $1 AND $2 AND (name > $3 OR (status = $4 AND NOT (id = $5)))\n\n# Add filters to existent query\nq2 = q.Where(t.id != 14)\n```\n\n#### JOIN\n```python\nt, t2 = Table(\'tbl\'), Table(\'tbl2\')\n\nsq = Select(t2.name).From(t2).Where(t2.id == t.id).Subquery(\'sq\')\nq = (\n    Select(t.id).From(t)\n    .Join(t2, t2.id == t.id)\n    .LeftJoin(t2, And(t2.id == t.id, t2.status == \'active\'))\n    .JoinLateral(sq, True)\n    .LeftJoinLateral(sq, sq.name != \'test\')\n)\n```\n\n#### PARAMETERS / LITERALS\nBy default, all values are considered as parameters. \nIf you need to cast value or add alias use Param wrapper.\nIf you need to literally insert value into sql use special Literal wrapper, \nbut be very careful - it won\'t be escaped and can lead to SQL injections. \nUse Literal only with data you can 100% trust.\n```python\nt = Table(\'tbl\')\nq = (\n    Select(t.STAR, Param(10).Cast(\'int\').As(\'added\')).From(t)\n    .Where(\n        t.id1 == 1, \n        t.id2 != Param(2).Cast(\'float\'), \n        t.id3 > Literal(3), \n        t.id4 < Literal(4).Cast(\'numeric\'),\n    )\n)\nbuild(q)\n# (\n#     \'SELECT *, $1::int AS added FROM tbl WHERE id1 == $2 AND id2 != $3::float AND id3 > 3 AND id4 < 4::numeric\',\n#     [10, 1, 2],\n# )\n```\n\n#### FUNCTIONS\nThere are `Func` and its `F` alias.\n```python\nt = Table(\'tbl\')\n\nq1 = (\n    Select(\n        F.count(\'*\'), \n        F.count(t.id).Where(t.id > 10, t.id < 20),\n        F.array_agg(t.id).OrderBy(t.id.Desc().NullsLast()).As(\'ids\'),\n    )\n    .From(t)\n)\n\nq2 = Select(t.id, F.row_number().Over(partition_by=t.status, order_by=t.id)).From(t)\n\nf = F.unnest(Literal([1, 2, 3])).As(\'idx\')\nq3 = Select(f.STAR).From(f)\n# SELECT * FROM UNNEST(ARRAY[1, 2, 3]) AS idx\n\nq4 = Select(Case((t.id == 1, \'first\'), (t.id == 2, \'second\'), Else=\'third\').As(\'val\')).From(t)\n\nq5 = Select(Array([t.id, 5, 7])).From(t)\n```\n\n#### ORDER BY / GROUP BY / HAVING / DISTINCT / DISTINCT ON\n```python\nt = Table(\'tbl\')\n\nq1 = Select(t.id.Distinct()).From(t)\n# SELECT DISTINCT id FROM tbl\n\nq2 = Select(t.STAR).From(t).OrderBy(t.id.Desc(), t.name.NullsLast())\n\nq3 = Select(F.count(\'*\')).From(t).GroupBy(t.status).Having(F.count(\'*\') > 10)\n\nq4 = Select(t.id, t.status).From(t).DistinctOn(t.status)\n# SELECT DISTINCT ON (status) id, status FROM tbl\n```\n\n#### OPERATIONS\nBasic math operator are supported out of the box: \n`+`, `-`, `*`, `/`, `>`, `>=`, `<`, `<=`. \nOthers are support as methods:\n```python\nt = Table(\'tbl\')\nq = (\n    Select(\n        t.id + t.id,\n        t.id - 1,\n        t.id * 10,\n        t.id > 15,\n        (t.id == 10).As(\'equals_ten\'),\n        (t.id != 11).As(\'not_equals_eleven\'),\n        Param(10) > 9,\n        (Literal(5) * 3.5).Cast(\'int\'),\n        t.id.Between(1, 2),\n        t.id.In([1, 2, 3]),\n        t.id.NotIn(Select(t.id).From(t).Where(t.id < 10)),\n        t.name.Is(None),\n        t.active.IsNot(False),\n        t.data.Op(\'->>\', \'key\').As(\'value1\'),\n        t.data.Op(\'#>>\', [\'key1\', \'key2\']).As(\'value2\'),\n        t.id.Any(list(range(1_000))),\n        t.name.Like(\'%ABC%\'),\n        t.name.Ilike(\'%abc%\'),\n    )\n    .From(t)\n)\n```\n\n#### INSERT\n```python\nt = Table(\'tbl\')\nq = (\n    Insert(t, columns=(t.name, t.status))\n    .Values(\n        (Param(\'some text\').Cast(\'varchar(10)\'), \'active\'),\n        (\'other text\', Literal(\'deleted\')),\n    )\n    .Returning(t.STAR)\n)\n\nbuild(q)\n# (\n#     "INSERT INTO tbl (name, status) VALUES ($1::varchar(10), $2), ($3, \'deleted\') RETURNING *",\n#     [\'some text\', \'active\', \'other text\'],\n# )\n\n# From select\nq = (\n    Insert(t, columns=(t.name, t.status))\n    .Select(\n        Select(F.concat(t.name, F.random().Cast(\'text\')), t.status)\n        .From(t)\n        .Where(t.id < 100)\n        .Limit(10)\n    )\n    .Returning(t.STAR)\n)\n\n# CTE\nsq = Select(t.STAR).From(t).Where(t.id < 100).Subquery(\'sq\')\nq = (\n    With(sq)\n    .Insert(t, (\'name\', \'status\'))\n    .From(Select(sq.name, sq.status).From(sq))\n)\n\n# Efficient bulk insert from the list of values\nvalues = [(str(i), \'active\') for i in range(1_000)]\nq = (\n    Insert(t, (\'name\', \'status\'))\n    .From(Select(\n        F.unnest(Param([name for name, _ in values]).Cast(\'text[]\')),\n        F.unnest(Param([status for _, status in values]).Cast(\'enum_status[]\')),\n    ))\n)\n```\n\n#### UPDATE / DELETE\n```python\nt = Table(\'stmh\')\nq1 = Update(t).Set({t.name: \'second\'}).Where(t.name == \'first\', t.status == \'active\').Returning(t.id)\nq2 = Delete(t).Where(t.id == 25).Returning(t.id)\n```\n\n#### Subquery / CTE\nAny Select/Insert/Update/Delete has Subquery method.\n```python\nt = Table(\'tbl\')\nsq = Select(t.id).From(t).Where(t.id < 100).Subquery(\'sq\')\n\n# Subquery\nq = Select(sq.id).From(sq).Where(sq.id > 50)\n# SELECT id FROM (SELECT id FROM tbl WHERE id < $1) As sq WHERE id > $2\n\n# CTE\nq = With(sq).Select(sq.id).From(sq).Where(sq.id > 50).Limit(2)\n# WITH sq AS (SELECT id FROM tbl WHERE id < $1) SELECT id FROM sq WHERE id > $2 LIMIT $3\n```\n\n***\n\n### Why not sqlalchemy?\n- too smart (tries to do everything: from connection/session management, to sql generating and params escaping)\n- too complex\n- too slow\n- mutable (on its core)\n\nIt is good for simple projects with simple sql queries. \nBut when your project grows up, your team grows up, sqlalchemy always leads to errors,\nunnecessary complexity, extra time your team need to spend to learn it, find not obvious bugs etc.  \n\n\n### Why not pypika?\nWhile it is much simpler then sqlalchemy, it also requires you to learn their own "sql syntax" which is not always obvious.\nAnd by default it uses parameters as literals, so it can lead to sql injections.\n\n\n***\n\nThe library is inspired by Ukraine🇺🇦 (Kyiv is my home) and its brave and free people🔱.\n\nSlava Ukraini, Heroyam slava!\n',
     'author': 'Vitalii Ponomar',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/ponomar/pgmini',
```

### Comparing `pgmini-0.1.4/PKG-INFO` & `pgmini-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pgmini
-Version: 0.1.4
+Version: 0.1.5
 Summary: Build sql for PostgreSQL
 Home-page: https://github.com/ponomar/pgmini
 License: MIT
 Author: Vitalii Ponomar
 Requires-Python: >=3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

