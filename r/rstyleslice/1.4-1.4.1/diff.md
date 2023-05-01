# Comparing `tmp/rstyleslice-1.4.tar.gz` & `tmp/rstyleslice-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rstyleslice-1.4.tar", last modified: Mon Apr 10 14:16:31 2023, max compression
+gzip compressed data, was "rstyleslice-1.4.1.tar", last modified: Mon May  1 02:02:15 2023, max compression
```

## Comparing `rstyleslice-1.4.tar` & `rstyleslice-1.4.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    10951 2023-02-13 16:30:40.665398 rstyleslice-1.4/LICENSE
--rw-r--r--   0        0        0     3293 2023-04-09 11:36:38.368832 rstyleslice-1.4/README.md
--rw-r--r--   0        0        0      571 2023-04-10 09:28:33.061542 rstyleslice-1.4/pyproject.toml
--rw-r--r--   0        0        0       31 2023-04-10 04:03:01.139197 rstyleslice-1.4/rstyleslice.py
--rw-r--r--   0        0        0     3606 1970-01-01 00:00:00.000000 rstyleslice-1.4/PKG-INFO
+-rw-r--r--   0        0        0    10951 2023-02-13 16:30:40.665398 rstyleslice-1.4.1/LICENSE
+-rw-r--r--   0        0        0     3373 2023-05-01 01:52:54.980777 rstyleslice-1.4.1/README.md
+-rw-r--r--   0        0        0      589 2023-04-30 19:31:48.020869 rstyleslice-1.4.1/pyproject.toml
+-rw-r--r--   0        0        0       31 2023-04-10 04:03:01.139197 rstyleslice-1.4.1/rstyleslice.py
+-rw-r--r--   0        0        0     3704 1970-01-01 00:00:00.000000 rstyleslice-1.4.1/PKG-INFO
```

### Comparing `rstyleslice-1.4/LICENSE` & `rstyleslice-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rstyleslice-1.4/README.md` & `rstyleslice-1.4.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # 项目描述
 
 一套符合直觉的索引和切片语法。
 
-|                                        | **Python**                                               | **rstyleslice**                                          |
-| -------------------------------------- | -------------------------------------------------------------- | -------------------------------------------------------------- |
-| **索引**                         | 从 0 开始<br />0 表示第 1 个元素<br />-1 表示倒数第 1 个元素（相同点） | 从 1 开始<br />1 表示第 1 个元素<br />-1 表示倒数第 1 个元素（相同点）   |
-| **切片**                         | 左闭右开区间，例如：<br />[3: 5] 表示提取第 4、5 这 2 个元素           | 双闭区间，例如：<br />[3: 5] 表示提取第 3、4、5 这 3 个元素              |
-| **从右往**<br />**左切片** | step（步长）为负值，例如：<br />[9: 1: -1] 表示提取第 9~3 这 7 个元素  | step（步长）始终为正值，例如：<br />[9: 1: 1] 表示提取第 9~1 这 9 个元素 |
+|                                        | **Python**                                                           | **rstyleslice**                                                      |
+| -------------------------------------- | -------------------------------------------------------------------------- | -------------------------------------------------------------------------- |
+| **索引**                         | 从 0 开始（0 表示第 1 个元素）<br /><br />-1 表示倒数第 1 个元素（相同点） | 从 1 开始（1 表示第 1 个元素）<br /><br />-1 表示倒数第 1 个元素（相同点） |
+| **切片**                         | 左闭右开区间，例如：<br />[3: 5] 表示提取第 4、5 这 2 个元素               | 双闭区间，例如：<br />[3: 5] 表示提取第 3、4、5 这 3 个元素                |
+| **从右往**<br />**左切片** | step（步长）为负值，例如：<br />[9: 1: -1] 表示提取第 9~3 这 7 个元素      | step（步长）始终为正值，例如：<br />[9: 1: 1] 表示提取第 9~1 这 9 个元素   |
 
-切片格式为  [start: stop: step]  ，start 表示从哪条开始，stop 表示到哪条停止，step 表示步长。当  step>1  时表示间隔式切片。
+切片格式为  [start: stop: step]  ，start 表示从哪条开始，stop 表示到哪条停止，step 表示步长。当  step>=2  时表示间隔式切片。
 
 # 安装与教程
 
 安装：`pip install rstyleslice`
 
-[教程](https://github.com/lcctoor/lccpy/blob/main/rstyleslice/docs/doc.md)
+[教程](https://github.com/lcctoor/lccpy/blob/main/packages/rstyleslice/docs/doc.md)
 
 # Bug提交、功能提议
 
 您可以通过 [Github-Issues](https://github.com/lcctoor/lccpy/issues)、[微信](https://raw.githubusercontent.com/lcctoor/me/main/author/WeChatQR.jpg)、[技术交流群](https://raw.githubusercontent.com/lcctoor/me/main/ExchangeGroup/PythonTecQR.jpg) 与我联系。
 
 # 关于作者
```

### Comparing `rstyleslice-1.4/pyproject.toml` & `rstyleslice-1.4.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "rstyleslice"
-version = "1.4"
+version = "1.4.1"
 description = "一套符合直觉的索引和切片语法"
 dependencies = ["lccpy >=1.3"]
 keywords = ["rstyleslice", "slice"]
 
 readme = "README.md"
 authors = [{name = "许灿标", email = "lcctoor@outlook.com"}]
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: Apache Software License"]
 requires-python = ">=3.7"
 
 [project.urls]
-HomePage = "https://github.com/lcctoor/lccpy/tree/main/rstyleslice"
+HomePage = "https://github.com/lcctoor/lccpy/tree/main/packages/rstyleslice#readme"
```

### Comparing `rstyleslice-1.4/PKG-INFO` & `rstyleslice-1.4.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: rstyleslice
-Version: 1.4
+Version: 1.4.1
 Summary: 一套符合直觉的索引和切片语法
 Keywords: rstyleslice,slice
 Author-email: 许灿标 <lcctoor@outlook.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Dist: lccpy >=1.3
-Project-URL: HomePage, https://github.com/lcctoor/lccpy/tree/main/rstyleslice
+Project-URL: HomePage, https://github.com/lcctoor/lccpy/tree/main/packages/rstyleslice#readme
 
 # 项目描述
 
 一套符合直觉的索引和切片语法。
 
-|                                        | **Python**                                               | **rstyleslice**                                          |
-| -------------------------------------- | -------------------------------------------------------------- | -------------------------------------------------------------- |
-| **索引**                         | 从 0 开始<br />0 表示第 1 个元素<br />-1 表示倒数第 1 个元素（相同点） | 从 1 开始<br />1 表示第 1 个元素<br />-1 表示倒数第 1 个元素（相同点）   |
-| **切片**                         | 左闭右开区间，例如：<br />[3: 5] 表示提取第 4、5 这 2 个元素           | 双闭区间，例如：<br />[3: 5] 表示提取第 3、4、5 这 3 个元素              |
-| **从右往**<br />**左切片** | step（步长）为负值，例如：<br />[9: 1: -1] 表示提取第 9~3 这 7 个元素  | step（步长）始终为正值，例如：<br />[9: 1: 1] 表示提取第 9~1 这 9 个元素 |
+|                                        | **Python**                                                           | **rstyleslice**                                                      |
+| -------------------------------------- | -------------------------------------------------------------------------- | -------------------------------------------------------------------------- |
+| **索引**                         | 从 0 开始（0 表示第 1 个元素）<br /><br />-1 表示倒数第 1 个元素（相同点） | 从 1 开始（1 表示第 1 个元素）<br /><br />-1 表示倒数第 1 个元素（相同点） |
+| **切片**                         | 左闭右开区间，例如：<br />[3: 5] 表示提取第 4、5 这 2 个元素               | 双闭区间，例如：<br />[3: 5] 表示提取第 3、4、5 这 3 个元素                |
+| **从右往**<br />**左切片** | step（步长）为负值，例如：<br />[9: 1: -1] 表示提取第 9~3 这 7 个元素      | step（步长）始终为正值，例如：<br />[9: 1: 1] 表示提取第 9~1 这 9 个元素   |
 
-切片格式为  [start: stop: step]  ，start 表示从哪条开始，stop 表示到哪条停止，step 表示步长。当  step>1  时表示间隔式切片。
+切片格式为  [start: stop: step]  ，start 表示从哪条开始，stop 表示到哪条停止，step 表示步长。当  step>=2  时表示间隔式切片。
 
 # 安装与教程
 
 安装：`pip install rstyleslice`
 
-[教程](https://github.com/lcctoor/lccpy/blob/main/rstyleslice/docs/doc.md)
+[教程](https://github.com/lcctoor/lccpy/blob/main/packages/rstyleslice/docs/doc.md)
 
 # Bug提交、功能提议
 
 您可以通过 [Github-Issues](https://github.com/lcctoor/lccpy/issues)、[微信](https://raw.githubusercontent.com/lcctoor/me/main/author/WeChatQR.jpg)、[技术交流群](https://raw.githubusercontent.com/lcctoor/me/main/ExchangeGroup/PythonTecQR.jpg) 与我联系。
 
 # 关于作者
```

