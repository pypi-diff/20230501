# Comparing `tmp/Zeraora-0.2.4.tar.gz` & `tmp/Zeraora-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Zeraora-0.2.4.tar", last modified: Mon Apr 24 09:14:35 2023, max compression
+gzip compressed data, was "dist/Zeraora-0.2.5.tar", last modified: Mon May  1 16:42:20 2023, max compression
```

## Comparing `Zeraora-0.2.4.tar` & `Zeraora-0.2.5.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:35.000000 Zeraora-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-04-24 09:14:35.000000 Zeraora-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-04-24 09:14:10.000000 Zeraora-0.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:35.000000 Zeraora-0.2.4/Zeraora.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-04-24 09:14:34.000000 Zeraora-0.2.4/Zeraora.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-24 09:14:35.000000 Zeraora-0.2.4/Zeraora.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 09:14:34.000000 Zeraora-0.2.4/Zeraora.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-24 09:14:34.000000 Zeraora-0.2.4/Zeraora.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 09:14:35.000000 Zeraora-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-04-24 09:14:10.000000 Zeraora-0.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:35.000000 Zeraora-0.2.4/zeraora/
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-24 09:14:10.000000 Zeraora-0.2.4/zeraora/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-24 09:14:10.000000 Zeraora-0.2.4/zeraora/charsets.py
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-04-24 09:14:10.000000 Zeraora-0.2.4/zeraora/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:35.000000 Zeraora-0.2.4/zeraora/djangobase/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-24 09:14:10.000000 Zeraora-0.2.4/zeraora/djangobase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-04-24 09:14:10.000000 Zeraora-0.2.4/zeraora/djangobase/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)     5236 2023-04-24 09:14:10.000000 Zeraora-0.2.4/zeraora/generators.py
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-24 09:14:10.000000 Zeraora-0.2.4/zeraora/math.py
--rw-r--r--   0 runner    (1001) docker     (123)     5935 2023-04-24 09:14:10.000000 Zeraora-0.2.4/zeraora/time.py
--rw-r--r--   0 runner    (1001) docker     (123)    10314 2023-04-24 09:14:10.000000 Zeraora-0.2.4/zeraora/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:42:20.000000 Zeraora-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-05-01 16:42:20.000000 Zeraora-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-05-01 16:42:09.000000 Zeraora-0.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:42:20.000000 Zeraora-0.2.5/Zeraora.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-05-01 16:42:19.000000 Zeraora-0.2.5/Zeraora.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-01 16:42:20.000000 Zeraora-0.2.5/Zeraora.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 16:42:19.000000 Zeraora-0.2.5/Zeraora.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-01 16:42:19.000000 Zeraora-0.2.5/Zeraora.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 16:42:20.000000 Zeraora-0.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-05-01 16:42:09.000000 Zeraora-0.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:42:20.000000 Zeraora-0.2.5/zeraora/
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-01 16:42:09.000000 Zeraora-0.2.5/zeraora/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-01 16:42:09.000000 Zeraora-0.2.5/zeraora/charsets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-05-01 16:42:09.000000 Zeraora-0.2.5/zeraora/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-05-01 16:42:09.000000 Zeraora-0.2.5/zeraora/divisions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:42:20.000000 Zeraora-0.2.5/zeraora/djangobase/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-01 16:42:09.000000 Zeraora-0.2.5/zeraora/djangobase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-05-01 16:42:09.000000 Zeraora-0.2.5/zeraora/djangobase/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5239 2023-05-01 16:42:09.000000 Zeraora-0.2.5/zeraora/generators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-01 16:42:09.000000 Zeraora-0.2.5/zeraora/math.py
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-01 16:42:09.000000 Zeraora-0.2.5/zeraora/shortcuts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6508 2023-05-01 16:42:09.000000 Zeraora-0.2.5/zeraora/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13305 2023-05-01 16:42:09.000000 Zeraora-0.2.5/zeraora/typing.py
```

### Comparing `Zeraora-0.2.4/PKG-INFO` & `Zeraora-0.2.5/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Zeraora
-Version: 0.2.4
+Version: 0.2.5
 Summary: 一个包含原创工具类及快捷函数的工具库。A original utility Python package.
 Home-page: https://github.com/aixcyi/zeraora
 Author: aixcyi
 Author-email: 75880483+aixcyi@users.noreply.github.com
 License: MIT
 Project-URL: Source, https://github.com/aixcyi/zeraora
 Project-URL: Tracker, https://github.com/aixcyi/zeraora/issues
@@ -18,22 +18,24 @@
         </div>
         <div align="center">
             <i>长期维护的个人开源工具库</i>
             <br>
             <i>An utility Python package supports for my personal and company projects</i>
         </div>
         
-        ## Usage
+        ## 安装
         
         使用 pip 直接安装：
         
         ```shell
         pip install zeraora
         ```
         
+        ## 用法
+        
         不能保证所有工具类和快捷函数自始至终都放在同一个子包，因此应该直接从根目录导入：
         
         ```python
         from zeraora import BearTimer
         
         with BearTimer() as bear:
             summary = 0
@@ -43,15 +45,15 @@
         ```
         
         亦或者：
         
         ```python
         import zeraora
         
-        with BearTimer.BearTimer() as bear:
+        with zeraora.BearTimer() as bear:
             summary = 0
             for i in range(1000000):
                 bear.step(f'loop to {i} now.')
                 summary += i
         ```
         
         但对于 `charsets` 和 `djangobase` 可以放心从子包导入：
@@ -65,26 +67,37 @@
         
         if __name__ == '__main__':
             [
                 print(make_pwd(16)) for _ in range(20)
             ]
         ```
         
-        ## Compatibility
+        ## 文档
+        
+        部分文档以 Markdown 格式存放在 [docs](./docs/README.md) 目录下。
+        
+        源代码多数附带[类型标注](https://docs.python.org/zh-cn/3/glossary.html#term-type-hint)和[文档字符串](https://docs.python.org/zh-cn/3/glossary.html#term-docstring)（[reStructuredText](https://zh.wikipedia.org/wiki/ReStructuredText)格式），文档未尽事宜请移步源代码浏览。
         
-        > 目前仍处于早期开发阶段。
+        ## 兼容性
         
         [Python 3.7](https://docs.python.org/zh-cn/3/whatsnew/3.7.html#summary-release-highlights) 开始 `dict` 正式按照插入顺序存储，考虑到 `dict` 是 Python 的基石，为了避免出现难以察觉的错误，因而将该版本定为兼容下限。这也是我接触过的项目中的最低运行版本，故而不太希望维护对更低版本的兼容。
         
-        项目会尽力保证向后兼容性，但还是建议在requirements中写明特定的版本号，避免因为版本更新或回退而出现难以解决的错误。
+        项目会尽力保证向后兼容性，但还是建议在requirements中写明特定的版本号，避免因为版本更新或回退而出现棘手的错误。
         
-        ## Change
+        ## 更新
         
         > 仅列出不兼容旧版的修改，其余变动见git历史。
         
+        ### 0.2.5（2023-5-02）
+        
+        - `OnionObject.__repr__()` 不再进行嵌套递归，现在嵌套的OnionObject对象会显示为 `OnionObject(...)` 。
+        - 去除 `OnionObject.__str__()` 方法，可以用 `import json` 后 `json.dumps(OnionObject())` 实现原来的效果。
+        - 更改 `BearTimer` 的默认打印格式。
+        - 将 `BearTimer.output()` 拆分为负责准备打印的 `record()` 和实现打印的 `handle()` 。
+        
         ### 0.2.0（2023-4-12）
         
         - 将 `JSONObject` 与 `JsonObject` 合并为 `OnionObject` ，并删去前述两个类。
         
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Zeraora-0.2.4/README.md` & `Zeraora-0.2.5/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -8,22 +8,24 @@
 </div>
 <div align="center">
     <i>长期维护的个人开源工具库</i>
     <br>
     <i>An utility Python package supports for my personal and company projects</i>
 </div>
 
-## Usage
+## 安装
 
 使用 pip 直接安装：
 
 ```shell
 pip install zeraora
 ```
 
+## 用法
+
 不能保证所有工具类和快捷函数自始至终都放在同一个子包，因此应该直接从根目录导入：
 
 ```python
 from zeraora import BearTimer
 
 with BearTimer() as bear:
     summary = 0
@@ -33,15 +35,15 @@
 ```
 
 亦或者：
 
 ```python
 import zeraora
 
-with BearTimer.BearTimer() as bear:
+with zeraora.BearTimer() as bear:
     summary = 0
     for i in range(1000000):
         bear.step(f'loop to {i} now.')
         summary += i
 ```
 
 但对于 `charsets` 和 `djangobase` 可以放心从子包导入：
@@ -55,22 +57,33 @@
 
 if __name__ == '__main__':
     [
         print(make_pwd(16)) for _ in range(20)
     ]
 ```
 
-## Compatibility
+## 文档
+
+部分文档以 Markdown 格式存放在 [docs](./docs/README.md) 目录下。
+
+源代码多数附带[类型标注](https://docs.python.org/zh-cn/3/glossary.html#term-type-hint)和[文档字符串](https://docs.python.org/zh-cn/3/glossary.html#term-docstring)（[reStructuredText](https://zh.wikipedia.org/wiki/ReStructuredText)格式），文档未尽事宜请移步源代码浏览。
 
-> 目前仍处于早期开发阶段。
+## 兼容性
 
 [Python 3.7](https://docs.python.org/zh-cn/3/whatsnew/3.7.html#summary-release-highlights) 开始 `dict` 正式按照插入顺序存储，考虑到 `dict` 是 Python 的基石，为了避免出现难以察觉的错误，因而将该版本定为兼容下限。这也是我接触过的项目中的最低运行版本，故而不太希望维护对更低版本的兼容。
 
-项目会尽力保证向后兼容性，但还是建议在requirements中写明特定的版本号，避免因为版本更新或回退而出现难以解决的错误。
+项目会尽力保证向后兼容性，但还是建议在requirements中写明特定的版本号，避免因为版本更新或回退而出现棘手的错误。
 
-## Change
+## 更新
 
 > 仅列出不兼容旧版的修改，其余变动见git历史。
 
+### 0.2.5（2023-5-02）
+
+- `OnionObject.__repr__()` 不再进行嵌套递归，现在嵌套的OnionObject对象会显示为 `OnionObject(...)` 。
+- 去除 `OnionObject.__str__()` 方法，可以用 `import json` 后 `json.dumps(OnionObject())` 实现原来的效果。
+- 更改 `BearTimer` 的默认打印格式。
+- 将 `BearTimer.output()` 拆分为负责准备打印的 `record()` 和实现打印的 `handle()` 。
+
 ### 0.2.0（2023-4-12）
 
 - 将 `JSONObject` 与 `JsonObject` 合并为 `OnionObject` ，并删去前述两个类。
```

### Comparing `Zeraora-0.2.4/Zeraora.egg-info/PKG-INFO` & `Zeraora-0.2.5/Zeraora.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Zeraora
-Version: 0.2.4
+Version: 0.2.5
 Summary: 一个包含原创工具类及快捷函数的工具库。A original utility Python package.
 Home-page: https://github.com/aixcyi/zeraora
 Author: aixcyi
 Author-email: 75880483+aixcyi@users.noreply.github.com
 License: MIT
 Project-URL: Source, https://github.com/aixcyi/zeraora
 Project-URL: Tracker, https://github.com/aixcyi/zeraora/issues
@@ -18,22 +18,24 @@
         </div>
         <div align="center">
             <i>长期维护的个人开源工具库</i>
             <br>
             <i>An utility Python package supports for my personal and company projects</i>
         </div>
         
-        ## Usage
+        ## 安装
         
         使用 pip 直接安装：
         
         ```shell
         pip install zeraora
         ```
         
+        ## 用法
+        
         不能保证所有工具类和快捷函数自始至终都放在同一个子包，因此应该直接从根目录导入：
         
         ```python
         from zeraora import BearTimer
         
         with BearTimer() as bear:
             summary = 0
@@ -43,15 +45,15 @@
         ```
         
         亦或者：
         
         ```python
         import zeraora
         
-        with BearTimer.BearTimer() as bear:
+        with zeraora.BearTimer() as bear:
             summary = 0
             for i in range(1000000):
                 bear.step(f'loop to {i} now.')
                 summary += i
         ```
         
         但对于 `charsets` 和 `djangobase` 可以放心从子包导入：
@@ -65,26 +67,37 @@
         
         if __name__ == '__main__':
             [
                 print(make_pwd(16)) for _ in range(20)
             ]
         ```
         
-        ## Compatibility
+        ## 文档
+        
+        部分文档以 Markdown 格式存放在 [docs](./docs/README.md) 目录下。
+        
+        源代码多数附带[类型标注](https://docs.python.org/zh-cn/3/glossary.html#term-type-hint)和[文档字符串](https://docs.python.org/zh-cn/3/glossary.html#term-docstring)（[reStructuredText](https://zh.wikipedia.org/wiki/ReStructuredText)格式），文档未尽事宜请移步源代码浏览。
         
-        > 目前仍处于早期开发阶段。
+        ## 兼容性
         
         [Python 3.7](https://docs.python.org/zh-cn/3/whatsnew/3.7.html#summary-release-highlights) 开始 `dict` 正式按照插入顺序存储，考虑到 `dict` 是 Python 的基石，为了避免出现难以察觉的错误，因而将该版本定为兼容下限。这也是我接触过的项目中的最低运行版本，故而不太希望维护对更低版本的兼容。
         
-        项目会尽力保证向后兼容性，但还是建议在requirements中写明特定的版本号，避免因为版本更新或回退而出现难以解决的错误。
+        项目会尽力保证向后兼容性，但还是建议在requirements中写明特定的版本号，避免因为版本更新或回退而出现棘手的错误。
         
-        ## Change
+        ## 更新
         
         > 仅列出不兼容旧版的修改，其余变动见git历史。
         
+        ### 0.2.5（2023-5-02）
+        
+        - `OnionObject.__repr__()` 不再进行嵌套递归，现在嵌套的OnionObject对象会显示为 `OnionObject(...)` 。
+        - 去除 `OnionObject.__str__()` 方法，可以用 `import json` 后 `json.dumps(OnionObject())` 实现原来的效果。
+        - 更改 `BearTimer` 的默认打印格式。
+        - 将 `BearTimer.output()` 拆分为负责准备打印的 `record()` 和实现打印的 `handle()` 。
+        
         ### 0.2.0（2023-4-12）
         
         - 将 `JSONObject` 与 `JsonObject` 合并为 `OnionObject` ，并删去前述两个类。
         
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Zeraora-0.2.4/setup.py` & `Zeraora-0.2.5/setup.py`

 * *Files identical despite different names*

### Comparing `Zeraora-0.2.4/zeraora/charsets.py` & `Zeraora-0.2.5/zeraora/charsets.py`

 * *Files identical despite different names*

### Comparing `Zeraora-0.2.4/zeraora/decorators.py` & `Zeraora-0.2.5/zeraora/decorators.py`

 * *Files identical despite different names*

### Comparing `Zeraora-0.2.4/zeraora/djangobase/mixins.py` & `Zeraora-0.2.5/zeraora/djangobase/mixins.py`

 * *Files identical despite different names*

### Comparing `Zeraora-0.2.4/zeraora/generators.py` & `Zeraora-0.2.5/zeraora/generators.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from zeraora.charsets import BASE62, BASE64
 
 
 def randbytes(n: int) -> bytes:
     """
     生成 n 个随机字节。
 
-    此函数是对 Python 3.9 以前的 random.randbytes(n) 的替代。
+    此函数用于在 Python 3.9 以前代替 random.randbytes(n) 方法。
     """
     assert n >= 0
     return getrandbits(n * 8).to_bytes(n, 'little')
 
 
 def randb62(n: int) -> str:
     """
```

### Comparing `Zeraora-0.2.4/zeraora/time.py` & `Zeraora-0.2.5/zeraora/time.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,96 +2,98 @@
 时间相关的处理。包括日期时间类型转换和计时。
 """
 
 import sys
 from datetime import timedelta, datetime
 from functools import wraps
 from io import TextIOWrapper
+from logging import Logger, DEBUG, getLevelName
+from typing import Tuple, Optional, Union, NoReturn, TextIO
 
 
-def delta2hms(delta: timedelta) -> tuple:
+def delta2hms(delta: timedelta) -> Tuple[int, int, float]:
     """
-    将时间增量转换为时分秒格式。
+    将时间增量转换为时分秒格式，其中秒钟以小数形式包含毫秒和微秒。
 
     :param delta: 时间增量。
-    :return: 包含三个整数的元组，分别对应小时数、分钟数、秒钟数。
+    :return: 一个三元元组。
     """
     h = delta.seconds // 3600
     m = delta.seconds % 3600 // 60
     s = delta.seconds % 60 + delta.microseconds / 1000000
     return h, m, s
 
 
-def delta2ms(delta: timedelta) -> tuple:
+def delta2ms(delta: timedelta) -> Tuple[int, float]:
     """
-    将时间增量转换为分秒格式。
+    将时间增量转换为分秒格式，其中秒钟以小数形式包含毫秒和微秒。
 
     :param delta: 时间增量。
-    :return: 包含两个整数的元组，分别对应分钟数和秒钟数。
+    :return: 二元元组。前者用一个整数表示分钟数，
+             后者用一个小数表示秒钟数和纳秒数。
     """
     m = delta.seconds // 60
     s = delta.seconds % 60 + delta.microseconds / 1000000
     return m, s
 
 
-class BearTimer(object):
+def delta2s(delta: timedelta) -> float:
     """
-    熊牌计时器。
+    将时间增量转换为秒钟数，以小数形式包含毫秒和微秒。
 
-    这个类可以让你对代码进行计时功能并输出提示。
+    :param delta: 时间增量。
+    :return: 一个小数。
+    """
+    return delta.seconds + delta.microseconds / 1000000
 
-    最简单的用法是使用 with 语句包裹需要计时的代码：
 
-    >>> with BearTimer():
-    >>>     for i in range(1000000):
-    >>>         print(i)
+class BearTimer(object):
+    fmt = '[{head:%H:%M:%S.%f}] [{level}] [{title}] [{total:.6f} +{delta:.6f}]: {msg}'
+    level = DEBUG
 
-    如果不方便使用 with 包裹，可以直接实例化一个类对象：
+    def __init__(self, title: str = None, output: Union[TextIOWrapper, TextIO, Logger] = None):
+        """
+        熊牌计时器。对代码运行进行计时，并打印时间和提示。
 
-    >>> bear = BearTimer()
-    >>> bear.start()
-    >>> bear.stop()
+        比较简单的用法是使用 with 语句包裹需要计时的部分，
+        它会在开始执行前启动计时，在执行完毕或出现异常而离开with后停止计时。
 
-    计时开始后，如果需要打印提示，请使用 .step() 方法，例如：
+        >>> with BearTimer() as bear:
+        >>>     summary = 0
+        >>>     for i in range(1000):
+        >>>         if not i % 67:
+        >>>             bear.step(f'loop to {i} now.')
+        >>>         summary += i
 
-    >>> with BearTimer() as bear:
-    >>>     summary = 0
-    >>>     for i in range(1000000):
-    >>>         bear.step(f'loop to {i} now.')
-    >>>         summary += i
+        如果需要对一整个函数的运行进行计时，那么可以将计时器作为装饰器使用：
 
-    又或者是
+        >>> @BearTimer()
+        >>> def prepare_order(request, *args, **kwargs):
+        >>>     # 业务逻辑
+        >>>     pass
 
-    >>> bear = BearTimer()
-    >>> bear.start()
-    >>> bear.step('operate somethings now.')
-    >>> bear.stop()
-    """
-    file: TextIOWrapper = sys.stdout
+        如果不方便使用 with 包裹，可以直接实例化一个类对象。
+        每一个对象都是独立的计时器，互不影响。
 
-    @staticmethod
-    def get_context_name():
-        try:
-            return sys._getframe().f_back.f_code.co_name
-        except AttributeError:
-            raise RuntimeError(
-                'Current system NOT support this class.\n'
-                '当前操作系统不支持使用该工具类。'
-            ) from None
+        >>> bear = BearTimer()
+        >>> bear.start()
+        >>> bear.stop()
 
-    def __init__(self, title: str = None, file: TextIOWrapper = None):
-        """
-        :param title: 计时器的标题，用以标明输出信息归属于哪个计时器。默认从上下文中获取。
-        :param file: 消息打印到哪里去。默认是系统标准输出。
-        :raise RuntimeError: 当前操作系统不支持使用该工具类。仅当没有提供title且无法从上下文中获取时抛出。
+        :param title: 计时器的标题，用以标明输出信息归属于哪个计时器。默认从打印消息时的上下文中获取。
+        :param output: 消息打印到哪里去。默认是系统标准输出。可以是一个文件IO对象，也可以是一个日志记录器。
         """
         self._start = None  # 计时开始时间
         self._point = None  # 中途标记时间（用于计算距离上次标记过去了多久）
         self._title = title
-        self.file = self.file if file is None else file
+        self.output = output
+        if not self._title:
+            if hasattr(sys, '_getframe'):
+                self._title = sys._getframe().f_back.f_code.co_name
+            else:
+                self._title = '<UNTITLED>'
 
     def __call__(self, func):
         @wraps(func)
         def wrapper(*args, **kwargs):
             self._title = func.__name__
             self.start()
             returns = func(*args, **kwargs)
@@ -103,83 +105,89 @@
     def __enter__(self):
         self.start()
         return self
 
     def __exit__(self, exc_type, exc_val, traceback):
         self.stop()
 
-    def output(
-            self,
-            msg: str = '',
-            fmt: str = '{head:%H:%M:%S.%f}, {minutes:d}:{seconds:f}, {title} | {msg}',
-            *args,
-            end: str = '\n',
-            **kwargs,
-    ) -> datetime:
+    def handle(self, full_message: str) -> NoReturn:
         """
-        打印一行消息，标明此刻的时间、经历的时长、计时器标题，以及附加的消息。
+        将消息发送到指定位置。这个位置允许是文件IO对象，或者是日志记录器。
 
-        你不应该使用这个方法，它只应在自定义这个类时被重写。
+        不应直接使用此方法。
+
+        :param full_message: 完整的消息内容。
+        :return: 无。
+        """
+        if hasattr(self.output, 'log') and callable(self.output.log):
+            self.output: Logger
+            self.output.log(self.level, full_message)
+
+        elif hasattr(self.output, 'write') and callable(self.output.write):
+            self.output: TextIOWrapper
+            print(full_message, file=self.output)
+
+        else:
+            print(full_message)
+
+    def record(self, msg: str = '', *args, **kwargs) -> datetime:
+        """
+        打印一行消息，标明此刻的时间、经历的时长、距上次打印的时长、计时器标题，以及附加的消息。
+
+        不应直接使用这个方法。
 
         :param msg: 要附加的消息。默认为空文本。
-        :param fmt: 字符串的格式。具体参数见默认值。
-        :param end: 要以什么结尾。因为一般是单行打印的，故有此参数。默认是 ”\n“ 。
         :param args: 其它需要打印的位置参数。
         :param kwargs: 其它需要打印的关键字参数。
         :return: 此时的时刻。
         """
         now = datetime.now()
-        m, s = delta2ms(now - self._start) if self._start else (0, 0)
-        title = self._title if self._title else self.get_context_name()
-        print(
-            fmt.format(*args, head=now, minutes=m, seconds=s,
-                       title=title, msg=msg, **kwargs),
-            file=self.file,
-            end=end,
+        total = delta2s(now - self._start) if self._start else 0
+        delta = delta2s(now - self._point) if self._point else 0
+        title = self._title if self._title else ''
+        message = self.fmt.format(
+            head=now, total=total, delta=delta, title=title, msg=msg,
+            level=getLevelName(self.level), *args, **kwargs,
         )
+        self._point = now
+        self.handle(message)
         return now
 
     def start(self, msg='Starting...'):
         """
         开始计时。
 
-        如果计时器还没结束，会重新开始计时，中途的标记也会被清除。
+        如果计时尚未结束，会重新开始计时，中途记录的标记也会被清除。
 
         :param msg: 要附加的消息。
         :return: 计时器对象自身。
         """
         self._point = None
-        self._start = self.output(msg + ('＜计时已重新开始＞' if self._start else ''))
+        self._start = datetime.now()
+        self.record(msg)
         return self
 
-    def step(self, msg=None):
+    def step(self, msg='') -> Tuple[Optional[datetime], datetime]:
         """
         中途标记。
 
         用此方法可以计算出距离上一次标记/开始计时过去了多久。
 
         如果计时器尚未开始计时，那么过去的时间始终是 0 秒。
 
-        :param msg: 要附加的消息。留空则显示过了多久。
-        :return: 一个元组，包含上一次标记/开始计时的时刻，和此时的时刻。
+        :param msg: 要附加的消息。
+        :return: 二元元组。包含上一次标记/开始计时的时刻，和此时的时刻。
         """
-        if self._start is not None:
-            if self._point is None:
-                self._point = self._start
-            m, s = delta2ms(datetime.now() - self._point)
-        else:
-            m, s = 0, 0
         prev = self._point
-        curr = self.output(msg if msg else f'(+{m:d}:{s:f})')
-        self._point = curr
+        curr = self.record(msg)
         return prev, curr
 
     def stop(self, msg='Stopped.') -> datetime:
         """
         结束计时。
 
         :param msg: 要附加的消息。
         :return: 此时的时刻。
         """
-        curr = self.output(msg + ('' if self._start else '＜计时还未开始＞'))
+        curr = self.record(msg)
         self._start = None
         return curr
```

### Comparing `Zeraora-0.2.4/zeraora/typing.py` & `Zeraora-0.2.5/zeraora/typing.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,83 +1,81 @@
 """
 类型相关。
 """
 
 import datetime
-import json
+import enum
 import re
+from types import DynamicClassAttribute
 from typing import Callable, Type, Union
 from uuid import UUID
 
 
 class OnionObject(object):
 
     def __translate_list(self, items: list) -> list:
         return list(
             self.__translate_list(list(item)) if isinstance(item, tuple)
             else self.__translate_list(item) if isinstance(item, list)
-            else type(self)(item) if isinstance(item, dict) and self.__recurse
+            else type(self)(item, self.__depth - 1) if isinstance(item, dict)
             else item
             for item in items
         )
 
     # OnionObject()
-    def __init__(self, dictionary: dict = None, recurse: bool = True, **kvs):
+    def __new__(cls, dictionary: dict = None, depth: int = -1, **kvs):
         """
-        将字典转化为嵌套对象。
+        将字典转化为对象，使得可以用点分法代替下标访问内容。
 
         支持还原为字典：
 
-        >>> dictionary = ~OnionObject()
+        >>> data: dict = ~OnionObject()
 
         支持直接更新字典：
 
-        >>> oo = OnionObject()
-        >>> oo = oo | OnionObject()
-        >>> oo |= OnionObjet()
+        >>> obj: OnionObject = OnionObject()
+        >>> obj: OnionObject = obj | dict()  # 等价于 obj |= dict()
 
         :param dictionary: 包含数据的字典。不符合标识符命名要求，
                            或者以双下划线 “__” 开头的键不会被收录。
-        :param recurse: 是否递归转化。
-        :param kvs: 任意键值对。
+        :param depth: 递归转化的层数。负数表示无限递归转化，正数表示递归层数，0无意义。
         :return: OnionObject 的对象。
         :raise TypeError: 属性名称必须是字符串。
         """
-        self.__recurse = recurse
-        for k, v in {**(dictionary if dictionary else {}), **kvs}.items():
-            k = str(k)
-            if not k.isidentifier() or k.startswith('__'):
-                continue
-            if isinstance(v, tuple):
-                self.__setattr__(k, self.__translate_list(list(v[:])))
-            elif isinstance(v, list):
-                self.__setattr__(k, self.__translate_list(v[:]))
-            elif isinstance(v, dict):
-                self.__setattr__(k, self.__class__(v) if recurse else v)
-            else:
-                self.__setattr__(k, v)
+        if dictionary is None:
+            dictionary = {}
+        if not isinstance(dictionary, dict):
+            raise TypeError  # pragma: no cover
+        if depth == 0:
+            return dictionary
+        dictionary.update(kvs)
+
+        self = object.__new__(cls)
+        self.__depth = depth
+        self.__ior__(dictionary)
+        return self
 
-    # OnionObject() | OnionObject()
+    # OnionObject() | dict()
     def __or__(self, dictionary: dict) -> 'OnionObject':
         for k, v in dictionary.items():
             k = str(k)
             if not k.isidentifier() or k.startswith('__'):
                 continue
-            if v.__class__ is tuple:
+            if isinstance(v, tuple):
                 self.__setattr__(k, self.__translate_list(list(v[:])))
-            elif v.__class__ is list:
+            elif isinstance(v, list):
                 self.__setattr__(k, self.__translate_list(v[:]))
-            elif v.__class__ is dict:
-                self.__setattr__(k, self.__class__(v) if self.__recurse else v)
+            elif isinstance(v, dict) and self.__depth:
+                self.__setattr__(k, self.__class__(v, self.__depth - 1))
             else:
                 self.__setattr__(k, v)
         return self
 
-    # oo = OnionObject()
-    # oo |= OnionObject()
+    # obj = OnionObject()
+    # obj |= dict()
     __ior__ = __or__
 
     # ~OnionObject()
     def __invert__(self) -> dict:
         def obtain():
             prefix = f'_{type(self).__name__}__'
             for k, v in self.__dict__.items():
@@ -95,24 +93,22 @@
 
         return dict(obtain())
 
     # repr(OnionObject())
     def __repr__(self) -> str:
         prefix = f'_{type(self).__name__}__'
         attrs = ', '.join(
+            f'{attr}={type(value).__name__}(...)'
+            if isinstance(value, OnionObject) else
             f'{attr}={value!r}'
             for attr, value in self.__dict__.items()
             if not attr.startswith('__') or attr.startswith(prefix)
         )
         return f'OnionObject({attrs})'
 
-    # str(OnionObject())
-    def __str__(self) -> str:
-        return json.dumps(~self, ensure_ascii=False)
-
 
 def casting(
         mapper: Callable,
         raw,
         *errs: Union[Exception, Type[Exception]],
         default=None,
 ):
@@ -127,15 +123,15 @@
     :param mapper: 类型转换器。如果转换器不可调用，将直接返回默认值。
     :param raw: 被转换的值。
     :param errs: 需要捕获的其它异常类或异常对象。应当提供可被 except 语句接受的值。
     :param default: 默认值。即使不提供也会默认返回 None 而不会抛出异常。
     :return: 转换后的值。如若捕获到特定异常将返回默认值。
     """
     if not callable(mapper):
-        return default
+        return default  # pragma: no cover
     try:
         return mapper(raw)
     except (TypeError, ValueError, KeyboardInterrupt) + errs:
         return default
 
 
 def represent(value) -> str:
@@ -148,15 +144,15 @@
 
     :param value: 任意值。
     :return: 字符串。
     """
     if isinstance(value, str):
         return f'"{value}"'
     elif isinstance(value, datetime.timedelta):
-        return f'[{value.days}d,{value.seconds}s,{value.microseconds}μs]'
+        return f'[{value.days}d+{value.seconds}.{value.microseconds:06d}s]'
     elif isinstance(value, datetime.datetime):
         return f'[{value:%Y-%m-%d %H:%M:%S,%f}]'
     elif isinstance(value, datetime.date):
         return f'[{value:%Y-%m-%d}]'
     elif isinstance(value, UUID):
         return value.hex
     else:
@@ -281,22 +277,112 @@
     - 1 MiB == 1024 KiB
 
     :param literal: 一个整数后缀数据大小的单位。
     :return:
     """
     if not isinstance(literal, str):
         raise TypeError(
-            '不支持解析一个非字符串类型的值。'
+            '不支持解析一个非字符串类型的值。'  # pragma: no cover
         )
 
     pattern = re.compile(r'^([0-9]+)\s*([KMGTPEZY]?)(i?[Bb])$')
     result = re.fullmatch(pattern, literal)
 
     if result is None:
         return 0
 
     base = int(result.group(1))
     shift = 'BKMGTPEZY'.index(result.group(2))
     power = (1024 if 'i' in result.group(3) else 1000) ** shift
     power = (power / 8) if 'b' in result.group(3) else power
 
     return base * power
+
+
+# copy from https://github.com/django/django/blob/stable/4.2.x/django/db/models/enums.py
+class ChoicesMeta(enum.EnumMeta):
+    """用于创建带有标签文本的枚举的元类。"""
+
+    def __new__(metacls, classname, bases, classdict, **kwds):
+        labels = []
+        for key in classdict._member_names:
+            value = classdict[key]
+            if (
+                    isinstance(value, (list, tuple))
+                    and len(value) > 1
+                    and isinstance(value[-1], (str,))
+            ):
+                *value, label = value
+                value = tuple(value)
+            else:
+                label = key.replace("_", " ").title()
+            labels.append(label)
+            # Use dict.__setitem__() to suppress defenses against double
+            # assignment in enum's classdict.
+            dict.__setitem__(classdict, key, value)
+        cls = super().__new__(metacls, classname, bases, classdict, **kwds)
+        for member, label in zip(cls.__members__.values(), labels):
+            member._label_ = label
+        return enum.unique(cls)
+
+    def __contains__(cls, member):
+        if not isinstance(member, enum.Enum):
+            # Allow non-enums to match against member values.
+            return any(x.value == member for x in cls)
+        return super().__contains__(member)
+
+    @property
+    def names(cls):
+        empty = ["__empty__"] if hasattr(cls, "__empty__") else []
+        return empty + [member.name for member in cls]
+
+    @property
+    def choices(cls):
+        empty = [(None, cls.__empty__)] if hasattr(cls, "__empty__") else []
+        return empty + [(member.value, member.label) for member in cls]
+
+    @property
+    def labels(cls):
+        return [label for _, label in cls.choices]
+
+    @property
+    def values(cls):
+        return [value for value, _ in cls.choices]
+
+
+# copy from https://github.com/django/django/blob/stable/4.2.x/django/db/models/enums.py
+class Choices(enum.Enum, metaclass=ChoicesMeta):
+    """用于创建带有标签文本的枚举的类。"""
+
+    @DynamicClassAttribute
+    def label(self):
+        return self._label_
+
+    @property
+    def do_not_call_in_templates(self):
+        return True
+
+    def __str__(self):
+        """
+        Use value when cast to str, so that Choices set as model instance
+        attributes are rendered as expected in templates and similar contexts.
+        """
+        return str(self.value)
+
+    # A similar format was proposed for Python 3.10.
+    def __repr__(self):
+        return f"{self.__class__.__qualname__}.{self._name_}"
+
+
+# copy from https://github.com/django/django/blob/stable/4.2.x/django/db/models/enums.py
+class IntegerChoices(int, Choices):
+    """用于创建值是整数的带有标签文本的枚举的类。"""
+
+    pass
+
+
+# copy from https://github.com/django/django/blob/stable/4.2.x/django/db/models/enums.py
+class TextChoices(str, Choices):
+    """用于创建值是字符串的带有标签文本的枚举的类。"""
+
+    def _generate_next_value_(name, start, count, last_values):
+        return name
```

