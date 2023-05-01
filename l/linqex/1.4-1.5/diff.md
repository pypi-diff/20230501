# Comparing `tmp/linqex-1.4.tar.gz` & `tmp/linqex-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linqex-1.4.tar", last modified: Wed Apr 19 00:13:24 2023, max compression
+gzip compressed data, was "linqex-1.5.tar", last modified: Mon May  1 00:27:34 2023, max compression
```

## Comparing `linqex-1.4.tar` & `linqex-1.5.tar`

### file list

```diff
@@ -1,24 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 00:13:24.034762 linqex-1.4/
--rw-rw-rw-   0        0        0     1084 2023-02-12 13:59:17.000000 linqex-1.4/LICENSE
--rw-rw-rw-   0        0        0     4334 2023-04-19 00:13:24.033728 linqex-1.4/PKG-INFO
--rw-rw-rw-   0        0        0     3800 2023-03-26 21:48:17.000000 linqex-1.4/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-19 00:13:23.982292 linqex-1.4/linqex/
--rw-rw-rw-   0        0        0       55 2023-04-10 13:14:49.000000 linqex-1.4/linqex/__init__.py
--rw-rw-rw-   0        0        0      478 2023-04-18 21:14:02.000000 linqex-1.4/linqex/_typing.py
-drwxrwxrwx   0        0        0        0 2023-04-19 00:13:24.023729 linqex-1.4/linqex/build/
--rw-rw-rw-   0        0        0      373 2023-04-10 13:52:19.000000 linqex-1.4/linqex/build/__init__.py
--rw-rw-rw-   0        0        0     1470 2023-04-10 21:41:43.000000 linqex-1.4/linqex/build/iterablebase.py
--rw-rw-rw-   0        0        0    15180 2023-04-18 23:38:32.000000 linqex-1.4/linqex/build/iterdictbase.py
--rw-rw-rw-   0        0        0    13262 2023-04-18 23:25:08.000000 linqex-1.4/linqex/build/iterlistbase.py
-drwxrwxrwx   0        0        0        0 2023-04-19 00:13:24.031726 linqex-1.4/linqex/linq/
--rw-rw-rw-   0        0        0      334 2023-04-10 13:52:07.000000 linqex-1.4/linqex/linq/__init__.py
--rw-rw-rw-   0        0        0     1402 2023-04-10 21:41:47.000000 linqex-1.4/linqex/linq/iterable.py
--rw-rw-rw-   0        0        0    15402 2023-04-18 23:19:40.000000 linqex-1.4/linqex/linq/iterdict.py
--rw-rw-rw-   0        0        0    15046 2023-04-18 23:11:20.000000 linqex-1.4/linqex/linq/iterlist.py
-drwxrwxrwx   0        0        0        0 2023-04-19 00:13:24.015725 linqex-1.4/linqex.egg-info/
--rw-rw-rw-   0        0        0     4334 2023-04-19 00:13:23.000000 linqex-1.4/linqex.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      392 2023-04-19 00:13:23.000000 linqex-1.4/linqex.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 00:13:23.000000 linqex-1.4/linqex.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-04-19 00:13:23.000000 linqex-1.4/linqex.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-19 00:13:24.035731 linqex-1.4/setup.cfg
--rw-rw-rw-   0        0        0     1240 2023-04-10 13:11:55.000000 linqex-1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 00:27:34.531782 linqex-1.5/
+-rw-rw-rw-   0        0        0     1084 2023-02-12 13:59:17.000000 linqex-1.5/LICENSE
+-rw-rw-rw-   0        0        0     5936 2023-05-01 00:27:34.530780 linqex-1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     5402 2023-04-30 23:59:14.000000 linqex-1.5/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-01 00:27:34.475268 linqex-1.5/linqex/
+-rw-rw-rw-   0        0        0       55 2023-04-10 13:14:49.000000 linqex-1.5/linqex/__init__.py
+-rw-rw-rw-   0        0        0      478 2023-04-18 21:14:02.000000 linqex-1.5/linqex/_typing.py
+drwxrwxrwx   0        0        0        0 2023-05-01 00:27:34.519896 linqex-1.5/linqex/build/
+-rw-rw-rw-   0        0        0      373 2023-04-10 13:52:19.000000 linqex-1.5/linqex/build/__init__.py
+-rw-rw-rw-   0        0        0     1419 2023-04-19 22:25:23.000000 linqex-1.5/linqex/build/iterablebase.py
+-rw-rw-rw-   0        0        0    15234 2023-04-30 22:40:47.000000 linqex-1.5/linqex/build/iterdictbase.py
+-rw-rw-rw-   0        0        0    12940 2023-04-30 23:28:45.000000 linqex-1.5/linqex/build/iteritembase.py
+-rw-rw-rw-   0        0        0    13272 2023-04-30 23:05:53.000000 linqex-1.5/linqex/build/iterlistbase.py
+drwxrwxrwx   0        0        0        0 2023-05-01 00:27:34.528541 linqex-1.5/linqex/linq/
+-rw-rw-rw-   0        0        0      334 2023-04-10 13:52:07.000000 linqex-1.5/linqex/linq/__init__.py
+-rw-rw-rw-   0        0        0     1350 2023-04-30 23:37:35.000000 linqex-1.5/linqex/linq/iterable.py
+-rw-rw-rw-   0        0        0    15400 2023-04-20 17:18:12.000000 linqex-1.5/linqex/linq/iterdict.py
+-rw-rw-rw-   0        0        0    14391 2023-04-30 23:27:34.000000 linqex-1.5/linqex/linq/iteritem.py
+-rw-rw-rw-   0        0        0    15035 2023-04-20 17:17:26.000000 linqex-1.5/linqex/linq/iterlist.py
+drwxrwxrwx   0        0        0        0 2023-05-01 00:27:34.511999 linqex-1.5/linqex.egg-info/
+-rw-rw-rw-   0        0        0     5936 2023-05-01 00:27:34.000000 linqex-1.5/linqex.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      445 2023-05-01 00:27:34.000000 linqex-1.5/linqex.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 00:27:34.000000 linqex-1.5/linqex.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-05-01 00:27:34.000000 linqex-1.5/linqex.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-01 00:27:34.531782 linqex-1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1240 2023-05-01 00:00:05.000000 linqex-1.5/setup.py
```

### Comparing `linqex-1.4/LICENSE` & `linqex-1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `linqex-1.4/linqex/build/iterablebase.py` & `linqex-1.5/linqex/build/iterablebase.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,38 @@
 from linqex._typing import *
 from linqex.build.iterdictbase import EnumerableDictBase
 from linqex.build.iterlistbase import EnumerableListBase
+from linqex.build.iteritembase import EnumerableItemBase
 
 from typing import Dict, List, Union, Generic
 
 
 class EnumerableBase(Generic[_TK,_TV]):
     def __new__(cls, iterable:Union[List[_TV],Dict[_TK,_TV]]):
         return cls.Iterable(iterable)
     @classmethod
-    def Iterable(cls, iterable:Union[List[_TV],Dict[_TK,_TV]]) -> Union[EnumerableListBase[_TV], EnumerableDictBase[_TK,_TV]]:
+    def Iterable(cls, iterable:Union[List[_TV],Dict[_TK,_TV]]) -> Union[EnumerableItemBase[_TV], EnumerableDictBase[_TK,_TV]]:
         if isinstance(iterable, list):
-            return cls.List(iterable)
+            return cls.Item(iterable)
         elif isinstance(iterable, dict):
             return cls.Dict(iterable)
         else:
             raise TypeError()
 
     @classmethod
+    def Item(cls, iteritem:List[_TV]=None) -> EnumerableItemBase[_TV]:
+        if iteritem is None:
+            iteritem:List[_TV]=list()
+        return EnumerableItemBase(iteritem)
+
+    @classmethod
     def List(cls, iterlist:List[_TV]=None) -> EnumerableListBase[_TV]:
         if iterlist is None:
             iterlist:List[_TV]=list()
         return EnumerableListBase(iterlist)
-    
-    @staticmethod
-    def Range(start:int, stop:int, step:int=1) -> "EnumerableListBase[int]":
-        return EnumerableListBase.Range(start, stop, step)
-    
-    @staticmethod
-    def Repeat(value:_Value, count:int) -> "EnumerableListBase[int]":
-        return EnumerableListBase.Repeat(value, count)
 
     @classmethod
     def Dict(cls, iterdict:Dict[_TK,_TV]=None) -> EnumerableDictBase[_TK,_TV]:
         if iterdict is None:
             iterdict:Dict[_TK,_TV]=dict()
         return EnumerableDictBase(iterdict)
```

### Comparing `linqex-1.4/linqex/build/iterdictbase.py` & `linqex-1.5/linqex/build/iterdictbase.py`

 * *Files 0% similar despite different names*

```diff
@@ -95,17 +95,17 @@
                 else:
                     newIterdict.append((inKey, inValue, outer[0], outer[1]))
         def rightJoin(innerIterdict:Dict[_TK,_TV], outerIterdict:Dict[_TK2,_TV2], newIterdict:List[Tuple[_TK,_TV,_TK2,_TV2]]):
             nonlocal outerFunc, innerFunc
             for outKey, outValue in EnumerableDictBase(outerIterdict).GetItems():
                 inner = EnumerableDictBase(innerIterdict).First(lambda inKey, inValue: outerFunc(outKey, outValue) == innerFunc(inKey, inValue))
                 if inner is None:
-                    newIterdict.append((outKey, outValue, None, None))
+                    newIterdict.append((None, None, outKey, outValue))
                 else:
-                    newIterdict.append((outKey, outValue, inner[0], inner[1]))        
+                    newIterdict.append((inner[0], inner[1], outKey, outValue))        
         newIterdict:List[Tuple[_TK,_TV,_TK2,_TV2]] = []
         if joinType == JoinType.INNER:
             joinTypeFunc = innerJoin
         elif joinType == JoinType.LEFT:
             joinTypeFunc = leftJoin
         elif joinType == JoinType.RIGHT:
             joinTypeFunc = rightJoin
@@ -113,15 +113,15 @@
         joinKeys = list(map(lambda value: joinFuncByKey(value[0], value[1], value[2], value[3]), newIterdict))
         joinValues = list(map(lambda value: joinFunc(value[0], value[1], value[2], value[3]), newIterdict))
         joinItems = list(zip(joinKeys, joinValues))
         return dict(joinItems)        
       
     def OrderBy(self, *orderByFunc:Tuple[Callable[[_TK,_TV],_Union[Tuple[_TFV],_TFV]],_Desc]) -> Dict[_TK,_TV]:
         if orderByFunc == ():
-            orderByFunc = (lambda key, value: value)
+            orderByFunc = ((lambda key, value: value, False))
         iterdict = self.GetItems()
         orderByFunc:list = list(reversed(orderByFunc))
         for func, desc in orderByFunc:
             iterdict = sorted(iterdict, key=lambda x: func(x[0],x[1]), reverse=desc)
         return dict(iterdict)
         
     def GroupBy(self, groupByFunc:Callable[[_TK,_TV],_Union[Tuple[_TFV],_TFV]]=lambda key, value: value) -> Dict[_Union[Tuple[_TFV],_TFV], Dict[_TK,_TV]]:
@@ -214,15 +214,16 @@
                 return temp[1]
             else:
                 return temp
         if not self.IsEmpty():
             result = dict([self.GetItems()[0]])
             result.update(dict(zip(self.GetKeys()[1:], list(itertools.accumulate(self.GetItems(), lambda temp, next: accumulateFunc(FirstTemp(temp), next[0], next[1])))[1:])))
             return result
-        return None
+        else:
+            return {}
         
     def Aggregate(self, accumulateFunc:Callable[[_TV,_TK,_TV],_TFV]=lambda temp, key, nextValue: temp + nextValue) -> _TFV:
         return EnumerableDictBase(self.Accumulate(accumulateFunc)).GetValues()[-1]
 
 
 
     def Count(self, value:_TV) -> int:
@@ -370,15 +371,15 @@
         return not self.IsEmpty()
     
     def __len__(self) -> int:
         return self.Lenght()
 
 
 
-    def __iter__(self):
+    def __iter__(self) -> Iterable[Tuple[int,_TV]]:
         return iter(self.GetItems())
     
     def __getitem__(self, key:_TK) -> _TV:
         return self.Get(key)
     
     def __setitem__(self, key:_TK, value:_Value):
         if key in self.Get():
```

### Comparing `linqex-1.4/linqex/build/iterlistbase.py` & `linqex-1.5/linqex/build/iterlistbase.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from linqex._typing import *
 
 from typing import Dict, List, Callable, Union as _Union, NoReturn, Optional, Tuple, Type, Generic
 from numbers import Number
 from collections.abc import Iterable
 import itertools
 
-class EnumerableListBase(Iterable[Tuple[int,_TV]],Generic[_TV]):
+class EnumerableListBase(Iterable[_TV],Generic[_TV]):
     
     def __init__(self, iterlist:Optional[List[_TV]]=None):
         if iterlist is None:
             iterlist:List[_TV] = list()
         if isinstance(iterlist, list):
             self.iterlist:List[_TV] = iterlist
         elif isinstance(iterlist, (tuple, set)):
@@ -94,38 +94,39 @@
                 else:
                     newIterlist.Add((inValue, outer[1]))
         def rightJoin(innerIterlist:List[_TV], outerIterlist:List[_TV2], newIterlist:EnumerableListBase[Tuple[_TV2,Optional[_TV]]]):
             nonlocal outerFunc, innerFunc
             for outValue in outerIterlist:
                 inner = EnumerableListBase(innerIterlist).First(lambda inValue: outerFunc(outValue) == innerFunc(inValue))
                 if inner is None:
-                    newIterlist.Add((outValue, None))
+                    newIterlist.Add((None, outValue))
                 else:
-                    newIterlist.Add((outValue, inner[1]))
+                    newIterlist.Add((inner[1], outValue))
         newIterlist = EnumerableListBase()
         if joinType == JoinType.INNER:
             joinTypeFunc = innerJoin
         elif joinType == JoinType.LEFT:
             joinTypeFunc = leftJoin
         elif joinType == JoinType.RIGHT:
             joinTypeFunc = rightJoin
         joinTypeFunc(self.Get(), iterlist, newIterlist)
         return newIterlist.Select(lambda value: joinFunc(value[0], value[1]))         
       
     def OrderBy(self, *orderByFunc:Tuple[Callable[[_TV],_Union[Tuple[_TFV],_TFV]],_Desc]) -> List[_TV]:
         if orderByFunc == ():
-            orderByFunc = ((lambda key, value: value, False))
+            orderByFunc = ((lambda value: value, False))
         iterlist = self.Get()
         orderByFunc:list = list(reversed(orderByFunc))
         for func, desc in orderByFunc:
-            iterlist = list(sorted(iterlist, key=func, reverse=desc))
-        return iterlist
+            iterlist = sorted(iterlist, key=func, reverse=desc)
+        return list(iterlist)
         
     def GroupBy(self, groupByFunc:Callable[[_TV],_Union[Tuple[_TFV],_TFV]]=lambda value: value) -> List[Tuple[_Union[Tuple[_TFV],_TFV], List[_TV]]]:
-        iterlist = itertools.groupby(self.OrderBy((groupByFunc, False)), groupByFunc)
+        iterlist = self.OrderBy((groupByFunc, False))
+        iterlist = itertools.groupby(iterlist, groupByFunc)
         return [(keys, list(group)) for keys, group in iterlist]
 
     def Reverse(self) -> List[_TV]:
         return list(reversed(self.Get()))
         
     def Zip(self, iterlist:List[_TV2], zipFunc:Callable[[_TV,_TV2],_TFV]=lambda inValue, outValue: (inValue, outValue)) -> List[_TFV]:
         newIterlist = EnumerableListBase(list(zip(self.GetValues(), EnumerableListBase(iterlist).GetValues())))
@@ -222,22 +223,21 @@
         if self.OfType(Number):
             return max(self.Get())
         else:
             return None
         
     def Min(self) -> Optional[_TV]:
         iterlist = self.GetValues()
-        if EnumerableListBase(iterlist).OfType(Number):
+        if self.OfType(Number):
             return min(iterlist)
         else:
             return None
 
 
 
-
     def Add(self, value:_Value):
         self.Get().append(value)
 
     def Prepend(self, value:_Value):
         newIterlist = [value]
         self.Clear()
         self.Concat(newIterlist)
@@ -358,16 +358,16 @@
         return not self.IsEmpty()
     
     def __len__(self) -> int:
         return self.Lenght()
 
 
 
-    def __iter__(self):
-        return iter(self.Get())
+    def __iter__(self) -> Iterable[_TV]:
+        return iter(self.GetValues())
     
     def __getitem__(self, key:int) -> _TV:
         return self.Get(key)
     
     def __setitem__(self, key:int, value:_Value):
         self.Update(key, value)
```

### Comparing `linqex-1.4/linqex/linq/iterable.py` & `linqex-1.5/linqex/linq/iterable.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,39 +1,38 @@
 from linqex._typing import *
 from linqex.linq.iterdict import EnumerableDict
 from linqex.linq.iterlist import EnumerableList
+from linqex.linq.iteritem import EnumerableItem
 
 from typing import Dict, List, Union, Generic
 
 
 class Enumerable(Generic[_TK,_TV]):
     def __new__(cls, iterable:Union[List[_TV],Dict[_TK,_TV]]):
         return cls.Iterable(iterable)
     @classmethod
-    def Iterable(cls, iterable:Union[List[_TV],Dict[_TK,_TV]]) -> Union[EnumerableList[_TV], EnumerableDict[_TK,_TV]]:
+    def Iterable(cls, iterable:Union[List[_TV],Dict[_TK,_TV]]) -> Union[EnumerableItem[_TV], EnumerableDict[_TK,_TV]]:
         if isinstance(iterable, list):
-            return cls.List(iterable)
+            return cls.Item(iterable)
         elif isinstance(iterable, dict):
             return cls.Dict(iterable)
         else:
             raise TypeError()
 
     @classmethod
+    def Item(cls, iteritem:List[_TV]=None) -> EnumerableItem[_TV]:
+        if iteritem is None:
+            iteritem:List[_TV]=list()
+        return EnumerableItem(iteritem)
+
+    @classmethod
     def List(cls, iterlist:List[_TV]=None) -> EnumerableList[_TV]:
         if iterlist is None:
             iterlist:List[_TV]=list()
         return EnumerableList(iterlist)
-    
-    @staticmethod
-    def Range(start:int, stop:int, step:int=1) -> "EnumerableList[int]":
-        return EnumerableList.Range(start, stop, step)
-    
-    @staticmethod
-    def Repeat(value:_Value, count:int) -> "EnumerableList[int]":
-        return EnumerableList.Repeat(value, count)
 
     @classmethod
     def Dict(cls, iterdict:Dict[_TK,_TV]=None) -> EnumerableDict[_TK,_TV]:
         if iterdict is None:
             iterdict:Dict[_TK,_TV]=dict()
         return EnumerableDict(iterdict)
```

### Comparing `linqex-1.4/linqex/linq/iterdict.py` & `linqex-1.5/linqex/linq/iterdict.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,29 +28,29 @@
         return enumerableDictOrValue.ToValue
     else:
         return enumerableDictOrValue
 
 class EnumerableDict(Iterable[Tuple[_TK,_TV]],Generic[_TK,_TV]):
     
     def __init__(self, iterdict:Dict[_TK,_TV]=None):
-        self.iterdict = EnumerableDictBase(EnumerableDictToValue(iterdict)).Get()
+        self.iterdict:Dict[_TK,_TV] = EnumerableDictBase(EnumerableDictToValue(iterdict)).Get()
         self.keyHistory:list = list()
         self._main:EnumerableDict = self
         self._orderby:list = list()
         self._oneValue:bool = False
 
     def __call__(self, iterdict:Dict[_TK,_TV]=None):
         self.__init__(iterdict)
 
     def Get(self, *key:_TK) -> _Union["EnumerableDict[_TK,_TV]",_TV]:
         iterdict = EnumerableDictBase(self.iterdict).Get(*key)
         if isinstance(iterdict,dict):
             return EnumerableDictCatch(self, iterdict, key)
         else:
-            return EnumerableDictCatch(self, {None:iterdict}, key, oneValue=True)
+            return iterdict
     
     def GetKey(self, value:_TV) -> _TK:
         return EnumerableDictBase(self.iterdict).GetKey(EnumerableDictToValue(value))
     
     def GetKeys(self) -> EnumerableList[_TK]:
         return EnumerableListCatch(self, EnumerableDictBase(self.iterdict).GetKeys())
     
@@ -322,16 +322,16 @@
         return EnumerableDictBase(self.iterdict).__bool__()
     
     def __len__(self) -> int:
         return EnumerableDictBase(self.iterdict).__len__()
 
 
 
-    def __iter__(self):
-        return EnumerableDictBase(self.iterdict).__iter__()
+    def __iter__(self) -> Iterable[Tuple[_TK,_TV]]:
+        return EnumerableDictBase(self.GetItems().ToValue).__iter__()
     
     def __getitem__(self, key:_TK) -> _TV:
         return EnumerableDictBase(self.iterdict).__getitem__(key)
     
     def __setitem__(self, key:_TK, value:_Value):
         return EnumerableDictBase(self.iterdict).__setitem__(key, EnumerableDictToValue(value))
```

### Comparing `linqex-1.4/linqex/linq/iterlist.py` & `linqex-1.5/linqex/linq/iterlist.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,32 +25,32 @@
 
 def EnumerableListToValue(enumerableListOrValue:_Union["EnumerableList[_TV2]",_TV]) -> _TV:
     if isinstance(enumerableListOrValue, EnumerableList):
         return enumerableListOrValue.ToValue
     else:
         return enumerableListOrValue
 
-class EnumerableList(Iterable[Tuple[int,_TV]],Generic[_TV]):
+class EnumerableList(Iterable[_TV],Generic[_TV]):
     
     def __init__(self, iterlist:List[_TV]=None):
-        self.iterlist = EnumerableListBase(EnumerableListToValue(iterlist)).Get()
+        self.iterlist:List[_TV] = EnumerableListBase(EnumerableListToValue(iterlist)).Get()
         self.keyHistory:list = list()
         self._main:EnumerableList = self
         self._orderby:list = list()
         self._oneValue:bool = False
 
     def __call__(self, iterlist:List[_TV]=None):
         self.__init__(iterlist)
 
     def Get(self, *key:int) -> _Union["EnumerableList[_TV]",_TV]:
         iterlist = EnumerableListBase(self.iterlist).Get(*key)
         if isinstance(iterlist,list):
             return EnumerableListCatch(self, iterlist, key)
         else:
-            return EnumerableListCatch(self, [iterlist], key, oneValue=True)
+            return iterlist
     
     def GetKey(self, value:_TV) -> int:
         return EnumerableListBase(self.iterlist).GetKey(EnumerableListToValue(value))
     
     def GetKeys(self) -> "EnumerableList[int]":
         return EnumerableListCatch(self,EnumerableListBase(self.iterlist).GetKeys())
     
@@ -320,16 +320,16 @@
         return EnumerableListBase(self.iterlist).__bool__()
     
     def __len__(self) -> int:
         return EnumerableListBase(self.iterlist).__len__()
 
 
 
-    def __iter__(self):
-        return EnumerableListBase(self.iterlist).__iter__()
+    def __iter__(self) -> Iterable[Tuple[int,_TV]]:
+        return EnumerableListBase(self.GetValues().ToValue).__iter__()
     
     def __getitem__(self, key:int) -> _TV:
         return EnumerableListBase(self.iterlist).__getitem__(key)
     
     def __setitem__(self, key:int, value:_Value):
         return EnumerableListBase(self.iterlist).__setitem__(key, EnumerableListToValue(value))
```

### Comparing `linqex-1.4/setup.py` & `linqex-1.5/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from setuptools import setup, find_packages
 
 with open('README.rst', 'r', encoding='utf-8') as file:
     LONG_DESCRIPTION = file.read() 
 LONG_DESCRIPTION_CONTENT_TYPE = "text/markdown"
 
 NAME = 'linqex'
-VERSION = '1.4'
+VERSION = '1.5'
 DESCRIPTION = 'The linq module in C# has been adapted for python with some modifications.'
 URL = 'https://github.com/TahsinCr/python-linqex'
 AUTHOR = 'TahsinCr'
 AUTHOR_EMAIL = 'TahsinCr@outlook.com'
 LICENSE = 'MIT'
 KEYWORDS = ['linq', 'linqex', 'ex', 'enumerable']
 SRC = 'linqex'
```

