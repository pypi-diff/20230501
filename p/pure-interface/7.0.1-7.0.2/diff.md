# Comparing `tmp/pure_interface-7.0.1.tar.gz` & `tmp/pure_interface-7.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\Source\pure_interface\dist\.tmp-fphbqodx\pure_interface-7.0.1.tar", last modified: Thu Apr 27 23:18:02 2023, max compression
+gzip compressed data, was "D:\Source\pure_interface\dist\.tmp-g_2wb4tl\pure_interface-7.0.2.tar", last modified: Mon May  1 21:19:49 2023, max compression
```

## Comparing `pure_interface-7.0.1.tar` & `pure_interface-7.0.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 23:18:02.710468 pure_interface-7.0.1/
--rw-rw-rw-   0        0        0     1070 2021-09-21 22:43:47.000000 pure_interface-7.0.1/LICENSE
--rw-rw-rw-   0        0        0    34872 2023-04-27 23:18:02.710468 pure_interface-7.0.1/PKG-INFO
--rw-rw-rw-   0        0        0    33904 2023-04-27 23:17:43.000000 pure_interface-7.0.1/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-27 23:18:02.683948 pure_interface-7.0.1/pure_interface/
--rw-rw-rw-   0        0        0      617 2023-04-27 23:17:43.000000 pure_interface-7.0.1/pure_interface/__init__.py
--rw-rw-rw-   0        0        0     7884 2023-03-01 20:08:43.000000 pure_interface-7.0.1/pure_interface/adaption.py
--rw-rw-rw-   0        0        0     2167 2023-03-01 20:08:43.000000 pure_interface-7.0.1/pure_interface/data_classes.py
--rw-rw-rw-   0        0        0     8441 2023-04-27 23:17:43.000000 pure_interface-7.0.1/pure_interface/delegation.py
--rw-rw-rw-   0        0        0      372 2023-03-01 20:08:43.000000 pure_interface-7.0.1/pure_interface/errors.py
--rw-rw-rw-   0        0        0    33894 2023-04-27 05:33:41.000000 pure_interface-7.0.1/pure_interface/interface.py
-drwxrwxrwx   0        0        0        0 2023-04-27 23:18:02.688467 pure_interface-7.0.1/pure_interface.egg-info/
--rw-rw-rw-   0        0        0    34872 2023-04-27 23:18:02.000000 pure_interface-7.0.1/pure_interface.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      821 2023-04-27 23:18:02.000000 pure_interface-7.0.1/pure_interface.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 23:18:02.000000 pure_interface-7.0.1/pure_interface.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-04-27 23:18:02.000000 pure_interface-7.0.1/pure_interface.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       90 2021-09-21 22:43:47.000000 pure_interface-7.0.1/pyproject.toml
--rw-rw-rw-   0        0        0     1088 2023-04-27 23:18:02.712468 pure_interface-7.0.1/setup.cfg
--rw-rw-rw-   0        0        0       43 2021-09-21 22:43:47.000000 pure_interface-7.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-27 23:18:02.709468 pure_interface-7.0.1/tests/
--rw-rw-rw-   0        0        0     3843 2023-04-27 05:33:41.000000 pure_interface-7.0.1/tests/test_adapt_args_anno.py
--rw-rw-rw-   0        0        0     2871 2023-04-27 05:33:41.000000 pure_interface-7.0.1/tests/test_adapt_args_no_anno.py
--rw-rw-rw-   0        0        0    12205 2023-04-27 05:33:41.000000 pure_interface-7.0.1/tests/test_adaption.py
--rw-rw-rw-   0        0        0     1022 2023-04-27 05:33:41.000000 pure_interface-7.0.1/tests/test_dataclass_support.py
--rw-rw-rw-   0        0        0     8573 2023-04-27 23:17:43.000000 pure_interface-7.0.1/tests/test_delegate.py
--rw-rw-rw-   0        0        0     5935 2023-04-27 05:33:41.000000 pure_interface-7.0.1/tests/test_func_sigs3.py
--rw-rw-rw-   0        0        0    11757 2023-04-27 05:33:41.000000 pure_interface-7.0.1/tests/test_function_sigs.py
--rw-rw-rw-   0        0        0      844 2023-04-27 05:33:41.000000 pure_interface-7.0.1/tests/test_generic_support.py
--rw-rw-rw-   0        0        0    16881 2023-04-27 05:33:41.000000 pure_interface-7.0.1/tests/test_implementation_checks.py
--rw-rw-rw-   0        0        0     2803 2023-04-27 05:33:41.000000 pure_interface-7.0.1/tests/test_inheritance.py
--rw-rw-rw-   0        0        0     4040 2023-04-27 05:33:41.000000 pure_interface-7.0.1/tests/test_isinstance.py
--rw-rw-rw-   0        0        0     2346 2023-03-01 20:08:43.000000 pure_interface-7.0.1/tests/test_meta_classes.py
--rw-rw-rw-   0        0        0     2877 2023-04-27 05:33:41.000000 pure_interface-7.0.1/tests/test_module_funcs.py
--rw-rw-rw-   0        0        0     3364 2023-03-01 20:08:43.000000 pure_interface-7.0.1/tests/test_no_content_checks.py
--rw-rw-rw-   0        0        0     2071 2023-04-27 05:33:41.000000 pure_interface-7.0.1/tests/test_tracker.py
--rw-rw-rw-   0        0        0      514 2023-04-27 05:33:41.000000 pure_interface-7.0.1/tests/test_versions_in_sync.py
+drwxrwxrwx   0        0        0        0 2023-05-01 21:19:49.815589 pure_interface-7.0.2/
+-rw-rw-rw-   0        0        0     1070 2021-09-21 22:43:47.000000 pure_interface-7.0.2/LICENSE
+-rw-rw-rw-   0        0        0    34872 2023-05-01 21:19:49.815589 pure_interface-7.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0    33904 2023-04-27 23:17:43.000000 pure_interface-7.0.2/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-01 21:19:49.787813 pure_interface-7.0.2/pure_interface/
+-rw-rw-rw-   0        0        0      617 2023-05-01 21:17:43.000000 pure_interface-7.0.2/pure_interface/__init__.py
+-rw-rw-rw-   0        0        0     7884 2023-03-01 20:08:43.000000 pure_interface-7.0.2/pure_interface/adaption.py
+-rw-rw-rw-   0        0        0     2167 2023-03-01 20:08:43.000000 pure_interface-7.0.2/pure_interface/data_classes.py
+-rw-rw-rw-   0        0        0     8441 2023-04-27 23:17:43.000000 pure_interface-7.0.2/pure_interface/delegation.py
+-rw-rw-rw-   0        0        0      372 2023-03-01 20:08:43.000000 pure_interface-7.0.2/pure_interface/errors.py
+-rw-rw-rw-   0        0        0    33634 2023-05-01 21:16:47.000000 pure_interface-7.0.2/pure_interface/interface.py
+drwxrwxrwx   0        0        0        0 2023-05-01 21:19:49.793583 pure_interface-7.0.2/pure_interface.egg-info/
+-rw-rw-rw-   0        0        0    34872 2023-05-01 21:19:49.000000 pure_interface-7.0.2/pure_interface.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      821 2023-05-01 21:19:49.000000 pure_interface-7.0.2/pure_interface.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 21:19:49.000000 pure_interface-7.0.2/pure_interface.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-05-01 21:19:49.000000 pure_interface-7.0.2/pure_interface.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       90 2021-09-21 22:43:47.000000 pure_interface-7.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0     1088 2023-05-01 21:19:49.816587 pure_interface-7.0.2/setup.cfg
+-rw-rw-rw-   0        0        0       43 2021-09-21 22:43:47.000000 pure_interface-7.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 21:19:49.813588 pure_interface-7.0.2/tests/
+-rw-rw-rw-   0        0        0     3843 2023-04-27 05:33:41.000000 pure_interface-7.0.2/tests/test_adapt_args_anno.py
+-rw-rw-rw-   0        0        0     2871 2023-04-27 05:33:41.000000 pure_interface-7.0.2/tests/test_adapt_args_no_anno.py
+-rw-rw-rw-   0        0        0    12205 2023-04-27 05:33:41.000000 pure_interface-7.0.2/tests/test_adaption.py
+-rw-rw-rw-   0        0        0     1022 2023-04-27 05:33:41.000000 pure_interface-7.0.2/tests/test_dataclass_support.py
+-rw-rw-rw-   0        0        0     8954 2023-05-01 21:04:02.000000 pure_interface-7.0.2/tests/test_delegate.py
+-rw-rw-rw-   0        0        0     5935 2023-04-27 05:33:41.000000 pure_interface-7.0.2/tests/test_func_sigs3.py
+-rw-rw-rw-   0        0        0    11757 2023-04-27 05:33:41.000000 pure_interface-7.0.2/tests/test_function_sigs.py
+-rw-rw-rw-   0        0        0     1051 2023-05-01 21:06:52.000000 pure_interface-7.0.2/tests/test_generic_support.py
+-rw-rw-rw-   0        0        0    16459 2023-05-01 21:18:53.000000 pure_interface-7.0.2/tests/test_implementation_checks.py
+-rw-rw-rw-   0        0        0     2803 2023-04-27 05:33:41.000000 pure_interface-7.0.2/tests/test_inheritance.py
+-rw-rw-rw-   0        0        0     4040 2023-04-27 05:33:41.000000 pure_interface-7.0.2/tests/test_isinstance.py
+-rw-rw-rw-   0        0        0     2346 2023-03-01 20:08:43.000000 pure_interface-7.0.2/tests/test_meta_classes.py
+-rw-rw-rw-   0        0        0     2877 2023-04-27 05:33:41.000000 pure_interface-7.0.2/tests/test_module_funcs.py
+-rw-rw-rw-   0        0        0     3364 2023-03-01 20:08:43.000000 pure_interface-7.0.2/tests/test_no_content_checks.py
+-rw-rw-rw-   0        0        0     2071 2023-04-27 05:33:41.000000 pure_interface-7.0.2/tests/test_tracker.py
+-rw-rw-rw-   0        0        0      514 2023-04-27 05:33:41.000000 pure_interface-7.0.2/tests/test_versions_in_sync.py
```

### Comparing `pure_interface-7.0.1/LICENSE` & `pure_interface-7.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pure_interface-7.0.1/PKG-INFO` & `pure_interface-7.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pure_interface
-Version: 7.0.1
+Version: 7.0.2
 Summary: A Python interface library that disallows function body content on interfaces and supports adaption.
 Home-page: https://github.com/seequent/pure_interface
 Download-URL: https://pypi.org/project/pure-interface/
 Author: Tim Mitchell
 Author-email: tim.mitchell@seequent.com
 License: MIT
 Keywords: abc interface adapt adaption mapper structural typing dataclass
```

### Comparing `pure_interface-7.0.1/README.rst` & `pure_interface-7.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `pure_interface-7.0.1/pure_interface/__init__.py` & `pure_interface-7.0.2/pure_interface/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 from .delegation import Delegate
 
 try:
     from .data_classes import dataclass
 except ImportError:
     pass
 
-__version__ = '7.0.1'
+__version__ = '7.0.2'
```

### Comparing `pure_interface-7.0.1/pure_interface/adaption.py` & `pure_interface-7.0.2/pure_interface/adaption.py`

 * *Files identical despite different names*

### Comparing `pure_interface-7.0.1/pure_interface/data_classes.py` & `pure_interface-7.0.2/pure_interface/data_classes.py`

 * *Files identical despite different names*

### Comparing `pure_interface-7.0.1/pure_interface/delegation.py` & `pure_interface-7.0.2/pure_interface/delegation.py`

 * *Files identical despite different names*

### Comparing `pure_interface-7.0.1/pure_interface/interface.py` & `pure_interface-7.0.2/pure_interface/interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,20 +2,19 @@
 pure_interface enforces empty functions and properties on interfaces and provides adaption and structural type checking.
 """
 from __future__ import division, print_function, absolute_import
 
 import abc
 from abc import abstractmethod, abstractclassmethod, abstractstaticmethod
 import collections
-import dataclasses
 import dis
 import inspect
 from inspect import signature, Signature, Parameter
 import types
-from typing import Any, Callable, List, Optional, Iterable, FrozenSet, Type, TypeVar
+from typing import Any, Callable, List, Optional, Iterable, FrozenSet, Type, TypeVar, Generic
 import sys
 import warnings
 import weakref
 
 from .errors import InterfaceError, AdaptionError
 
 is_development = not hasattr(sys, 'frozen')
@@ -101,14 +100,16 @@
 
 def _type_is_interface(cls):
     """ Return True if cls is a pure interface or an empty ABC class"""
     if cls is object:
         return False
     if hasattr(cls, '_pi'):
         return cls._pi.type_is_interface
+    if cls is Generic:
+        return True  # this class is just for type hinting
     if issubclass(type(cls), abc.ABCMeta):
         for attr, value in cls.__dict__.items():
             if _builtin_attrs(attr):
                 continue
             if callable(value):
                 if not _is_empty_function(value):
                     return False
@@ -541,19 +542,14 @@
             return cls
 
         base_types = [(cls, _type_is_interface(cls)) for cls in bases]
         type_is_interface = all(is_interface for cls, is_interface in base_types)
 
         if clsname == 'Interface' and attributes.get('__module__', '') == 'pure_interface':
             type_is_interface = True
-        if len(bases) > 1 and bases[0] is object:
-            warnings.warn('object should come after {} in base list of {}. '
-                          'Fixing inconsistent MRO is deprecated'.format(bases[1].__name__, clsname))
-            bases = bases[1:]  # create a consistent MRO order
-            base_types = base_types[1:]
 
         interface_method_signatures = dict()
         interface_attribute_names = set()
         abstract_properties = set()
         for i in range(len(bases) - 1, -1, -1):  # start at back end
             base, base_is_interface = base_types[i]
             if base is object:
```

### Comparing `pure_interface-7.0.1/pure_interface.egg-info/PKG-INFO` & `pure_interface-7.0.2/pure_interface.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pure-interface
-Version: 7.0.1
+Version: 7.0.2
 Summary: A Python interface library that disallows function body content on interfaces and supports adaption.
 Home-page: https://github.com/seequent/pure_interface
 Download-URL: https://pypi.org/project/pure-interface/
 Author: Tim Mitchell
 Author-email: tim.mitchell@seequent.com
 License: MIT
 Keywords: abc interface adapt adaption mapper structural typing dataclass
```

### Comparing `pure_interface-7.0.1/pure_interface.egg-info/SOURCES.txt` & `pure_interface-7.0.2/pure_interface.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pure_interface-7.0.1/setup.cfg` & `pure_interface-7.0.2/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 7572 655f 696e 7465 7266 6163   = pure_interfac
 00000020: 650d 0a76 6572 7369 6f6e 203d 2037 2e30  e..version = 7.0
-00000030: 2e31 0d0a 6465 7363 7269 7074 696f 6e20  .1..description 
+00000030: 2e32 0d0a 6465 7363 7269 7074 696f 6e20  .2..description 
 00000040: 3d20 4120 5079 7468 6f6e 2069 6e74 6572  = A Python inter
 00000050: 6661 6365 206c 6962 7261 7279 2074 6861  face library tha
 00000060: 7420 6469 7361 6c6c 6f77 7320 6675 6e63  t disallows func
 00000070: 7469 6f6e 2062 6f64 7920 636f 6e74 656e  tion body conten
 00000080: 7420 6f6e 2069 6e74 6572 6661 6365 7320  t on interfaces 
 00000090: 616e 6420 7375 7070 6f72 7473 2061 6461  and supports ada
 000000a0: 7074 696f 6e2e 0d0a 6b65 7977 6f72 6473  ption...keywords
```

### Comparing `pure_interface-7.0.1/tests/test_adapt_args_anno.py` & `pure_interface-7.0.2/tests/test_adapt_args_anno.py`

 * *Files identical despite different names*

### Comparing `pure_interface-7.0.1/tests/test_adapt_args_no_anno.py` & `pure_interface-7.0.2/tests/test_adapt_args_no_anno.py`

 * *Files identical despite different names*

### Comparing `pure_interface-7.0.1/tests/test_adaption.py` & `pure_interface-7.0.2/tests/test_adaption.py`

 * *Files identical despite different names*

### Comparing `pure_interface-7.0.1/tests/test_dataclass_support.py` & `pure_interface-7.0.2/tests/test_dataclass_support.py`

 * *Files identical despite different names*

### Comparing `pure_interface-7.0.1/tests/test_delegate.py` & `pure_interface-7.0.2/tests/test_delegate.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,18 @@
 from pure_interface import delegation
 
 
 class ITalker(pure_interface.Interface):
     def talk(self):
         pass
 
+class ISubTalker(ITalker):
+    def chat(self):
+        pass
+
 
 class ISpeaker(pure_interface.Interface):
     def speak(self, volume):
         pass
 
 
 class Speaker(ISpeaker, object):
@@ -22,14 +26,17 @@
         return 'speak'
 
 
 class Talker(ITalker, object):
     def talk(self):
         return 'talk'
 
+    def chat(self):
+        return 'chat'
+
 
 class IPoint(pure_interface.Interface):
     x: int
     y: int
 
     def to_str(self) -> str:
         pass
@@ -58,14 +65,18 @@
 class DFallback(delegation.Delegate, ITalker):
     pi_attr_fallback = 'impl'
 
     def __init__(self, impl):
         self.impl = impl
 
 
+class DSubFallback(DFallback, ISubTalker):
+    pass
+
+
 class DAttrMap(delegation.Delegate, IPoint):
     pi_attr_mapping = {'x': 'a.x',
                        'y': 'b.y',
                        'to_str': 'b.to_str',
                        }
 
     def __init__(self, a, b):
@@ -271,14 +282,19 @@
         d3 = ScaledPoint3(p)
         self.assertEqual(4, d3.y)
         self.assertEqual('1, 4', d3.to_str())
         d3.y = 8  # delegates to p
         self.assertEqual(4, p.y)
         self.assertEqual(3, d3.z)
 
+    def test_delegate_subclass_fallback(self):
+        """Fallback delegates are used for subclass interface attributes too."""
+        d = DSubFallback(Talker())
+        self.assertEqual('chat', d.chat())
+
 
 class CompositionTest(unittest.TestCase):
 
     def test_type_composition(self):
         a = Point(1, 2)
         b = Talker()
```

### Comparing `pure_interface-7.0.1/tests/test_func_sigs3.py` & `pure_interface-7.0.2/tests/test_func_sigs3.py`

 * *Files identical despite different names*

### Comparing `pure_interface-7.0.1/tests/test_function_sigs.py` & `pure_interface-7.0.2/tests/test_function_sigs.py`

 * *Files identical despite different names*

### Comparing `pure_interface-7.0.1/tests/test_generic_support.py` & `pure_interface-7.0.2/tests/test_generic_support.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,41 @@
 import unittest
 import pure_interface
 from typing import TypeVar, List, Iterable
 
 T = TypeVar('T')
 
-class MyInterface(pure_interface.Interface, Iterable[str]):
+class IMyInterface(pure_interface.Interface, Iterable[str]):
     def foo(self) -> T:
         pass
 
-class MyGenericInterface(pure_interface.Interface, Iterable[T]):
+class IMyGenericInterface(pure_interface.Interface, Iterable[T]):
     def foo(self) -> T:
         pass
 
-class Impl(List[str], MyInterface):
+class Impl(List[str], IMyInterface):
     def foo(self):
         return 'foo'
 
-class StrImpl(List[str], MyGenericInterface[str]):
+class StrImpl(List[str], IMyGenericInterface[str]):
     def foo(self):
         return 'foo'
 
 
-class GenericImpl(List[T], MyGenericInterface[T]):
+class GenericImpl(List[T], IMyGenericInterface[T]):
     def foo(self):
         return T('foo')
 
 
 class TestGenericSupport(unittest.TestCase):
+
+    def test_generics_are_interfaces(self):
+        self.assertTrue(pure_interface.type_is_interface(IMyInterface))
+        self.assertTrue(pure_interface.type_is_interface(IMyGenericInterface))
+
     def test_can_use_iterable(self):
         imp = Impl()
         imp.append('hello')
         imp = StrImpl()
         imp.append('hello')
         imp = GenericImpl[int]()
         imp.append(34)
```

### Comparing `pure_interface-7.0.1/tests/test_implementation_checks.py` & `pure_interface-7.0.2/tests/test_implementation_checks.py`

 * *Files 2% similar despite different names*

```diff
@@ -235,26 +235,14 @@
 
         # assert
         self.assertEqual(len(interface.missing_method_warnings), 1)
         msg = interface.missing_method_warnings[0]
         self.assertIn('SimpleSimon', msg)
         self.assertIn('foo', msg)
 
-    def test_inconsistent_mro_warning(self):
-        interface.is_development = True
-
-        warn = mock.MagicMock()
-        with mock.patch('warnings.warn', warn):
-            class SimpleSimon(object, ISimple):
-                def foo(self):
-                    pass
-
-        self.assertEqual(warn.call_count, 1)
-        self.assertTrue(warn.call_args[0][0].startswith('object should come after ISimple'))
-
     def test_is_development_flag_stops_warnings(self):
         interface.is_development = False
 
         warn = mock.MagicMock()
         with mock.patch('warnings.warn', warn):
             class SimpleSimon(ISimple, object):
                 pass
```

### Comparing `pure_interface-7.0.1/tests/test_inheritance.py` & `pure_interface-7.0.2/tests/test_inheritance.py`

 * *Files identical despite different names*

### Comparing `pure_interface-7.0.1/tests/test_isinstance.py` & `pure_interface-7.0.2/tests/test_isinstance.py`

 * *Files identical despite different names*

### Comparing `pure_interface-7.0.1/tests/test_meta_classes.py` & `pure_interface-7.0.2/tests/test_meta_classes.py`

 * *Files identical despite different names*

### Comparing `pure_interface-7.0.1/tests/test_module_funcs.py` & `pure_interface-7.0.2/tests/test_module_funcs.py`

 * *Files identical despite different names*

### Comparing `pure_interface-7.0.1/tests/test_no_content_checks.py` & `pure_interface-7.0.2/tests/test_no_content_checks.py`

 * *Files identical despite different names*

### Comparing `pure_interface-7.0.1/tests/test_tracker.py` & `pure_interface-7.0.2/tests/test_tracker.py`

 * *Files identical despite different names*

### Comparing `pure_interface-7.0.1/tests/test_versions_in_sync.py` & `pure_interface-7.0.2/tests/test_versions_in_sync.py`

 * *Files identical despite different names*

