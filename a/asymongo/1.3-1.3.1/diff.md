# Comparing `tmp/asymongo-1.3.tar.gz` & `tmp/asymongo-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asymongo-1.3.tar", last modified: Mon Apr 10 14:23:32 2023, max compression
+gzip compressed data, was "asymongo-1.3.1.tar", last modified: Mon May  1 01:47:53 2023, max compression
```

## Comparing `asymongo-1.3.tar` & `asymongo-1.3.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    10953 2023-02-13 16:22:52.569575 asymongo-1.3/LICENSE
--rw-r--r--   0        0        0     5171 2023-04-09 11:20:55.368262 asymongo-1.3/README.md
--rw-r--r--   0        0        0       28 2023-04-10 03:40:07.519027 asymongo-1.3/asymongo.py
--rw-r--r--   0        0        0      563 2023-04-10 09:19:58.801930 asymongo-1.3/pyproject.toml
--rw-r--r--   0        0        0     5423 1970-01-01 00:00:00.000000 asymongo-1.3/PKG-INFO
+-rw-r--r--   0        0        0    10953 2023-02-13 16:22:52.569575 asymongo-1.3.1/LICENSE
+-rw-r--r--   0        0        0     5175 2023-04-16 20:01:06.324279 asymongo-1.3.1/README.md
+-rw-r--r--   0        0        0       28 2023-04-10 03:40:07.519027 asymongo-1.3.1/asymongo.py
+-rw-r--r--   0        0        0      583 2023-05-01 01:47:43.619310 asymongo-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0     5447 1970-01-01 00:00:00.000000 asymongo-1.3.1/PKG-INFO
```

### Comparing `asymongo-1.3/LICENSE` & `asymongo-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `asymongo-1.3/README.md` & `asymongo-1.3.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 ```
 
 创建ORM：
 
 ```python
 mkconn = lambda: MongoClient(host='localhost', port=27017)
 
-orm = mg.ORM(mkconn=mkconn)  # 账户ORM
+orm = mg.ORM(mkconn)  # 账户ORM
 db = orm['泉州市']  # 库ORM
 sheet = db['希望小学']  # 表ORM
 ```
 
 新增数据：
 
 ```python
@@ -111,25 +111,25 @@
 | mc.年级 == mg.isin('初三', '高二')       | 若字段值是传入值的成员，则符合       |
 | mc.年龄 == mg.notin(10, 30, 45)          | 若字段值不是传入值的成员，则符合     |
 | mc.爱好 == mg.containAll('画画', '足球') | 若字段值包含传入值的所有元素，则符合 |
 | ...                                      | ...                                  |
 
 过滤器的集合运算：
 
-| **代码**                                                      | **解释** |
-| ------------------------------------------------------------------- | -------------- |
-| [ mc.年龄>3 ][ mc.年龄<100 ]                                        | 交集           |
-| [ (mc.年龄==30)\| (mc.年龄>30) \| (mc.年龄<30) \| (mc.年龄==None) ] | 并集           |
-| [ (mc.年龄>3) - (mc.年龄>100) ]                                     | 差集           |
-| [ ~(mc.年龄>100) ]                                                  | 补集           |
+| **代码**                                                         | **解释** |
+| ---------------------------------------------------------------------- | -------------- |
+| [ mc.年龄>3 ][ mc.年龄<100 ]                                           | 交集           |
+| [ (mc.年龄<30) \| (mc.年龄>30) \| (mc.年龄==30) \| (mc.年龄==None) ] | 并集           |
+| [ (mc.年龄>3) - (mc.年龄>100) ]                                        | 差集           |
+| [ ~(mc.年龄>100) ]                                                     | 补集           |
 
 只返回姓名、年龄这2个字段：
 
 ```python
-await sheet[mc.年龄>11][mc.年龄<30]['姓名','年龄'][:]
+await sheet[mc.年级=='高一']['姓名','年龄'][:]
 ```
 
 特殊操作：
 
 | 代码             | 解释                                               |
 | ---------------- | -------------------------------------------------- |
 | mup.inc(1)       | 自增1                                              |
```

### Comparing `asymongo-1.3/pyproject.toml` & `asymongo-1.3.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "asymongo"
-version = "1.3"
+version = "1.3.1"
 description = "异步的 MongoDB ORM"
-dependencies = ["lccpy >=1.3"]
+dependencies = ["lccpy >=1.3.1"]
 keywords = ["asymongo", "motor", "mongodb", "pymongo"]
 
 readme = "README.md"
 authors = [{name = "许灿标", email = "lcctoor@outlook.com"}]
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: Apache Software License"]
 requires-python = ">=3.7"
 
 [project.urls]
-HomePage = "https://github.com/lcctoor/lccpy/tree/main/asymongo"
+HomePage = "https://github.com/lcctoor/lccpy/tree/main/packages/asymongo#readme"
```

### Comparing `asymongo-1.3/PKG-INFO` & `asymongo-1.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: asymongo
-Version: 1.3
+Version: 1.3.1
 Summary: 异步的 MongoDB ORM
 Keywords: asymongo,motor,mongodb,pymongo
 Author-email: 许灿标 <lcctoor@outlook.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Dist: lccpy >=1.3
-Project-URL: HomePage, https://github.com/lcctoor/lccpy/tree/main/asymongo
+Requires-Dist: lccpy >=1.3.1
+Project-URL: HomePage, https://github.com/lcctoor/lccpy/tree/main/packages/asymongo#readme
 
 # 项目描述
 
 异步的 MongoDB ORM 。
 
 # 安装与教程
 
@@ -45,15 +45,15 @@
 ```
 
 创建ORM：
 
 ```python
 mkconn = lambda: MongoClient(host='localhost', port=27017)
 
-orm = mg.ORM(mkconn=mkconn)  # 账户ORM
+orm = mg.ORM(mkconn)  # 账户ORM
 db = orm['泉州市']  # 库ORM
 sheet = db['希望小学']  # 表ORM
 ```
 
 新增数据：
 
 ```python
@@ -123,25 +123,25 @@
 | mc.年级 == mg.isin('初三', '高二')       | 若字段值是传入值的成员，则符合       |
 | mc.年龄 == mg.notin(10, 30, 45)          | 若字段值不是传入值的成员，则符合     |
 | mc.爱好 == mg.containAll('画画', '足球') | 若字段值包含传入值的所有元素，则符合 |
 | ...                                      | ...                                  |
 
 过滤器的集合运算：
 
-| **代码**                                                      | **解释** |
-| ------------------------------------------------------------------- | -------------- |
-| [ mc.年龄>3 ][ mc.年龄<100 ]                                        | 交集           |
-| [ (mc.年龄==30)\| (mc.年龄>30) \| (mc.年龄<30) \| (mc.年龄==None) ] | 并集           |
-| [ (mc.年龄>3) - (mc.年龄>100) ]                                     | 差集           |
-| [ ~(mc.年龄>100) ]                                                  | 补集           |
+| **代码**                                                         | **解释** |
+| ---------------------------------------------------------------------- | -------------- |
+| [ mc.年龄>3 ][ mc.年龄<100 ]                                           | 交集           |
+| [ (mc.年龄<30) \| (mc.年龄>30) \| (mc.年龄==30) \| (mc.年龄==None) ] | 并集           |
+| [ (mc.年龄>3) - (mc.年龄>100) ]                                        | 差集           |
+| [ ~(mc.年龄>100) ]                                                     | 补集           |
 
 只返回姓名、年龄这2个字段：
 
 ```python
-await sheet[mc.年龄>11][mc.年龄<30]['姓名','年龄'][:]
+await sheet[mc.年级=='高一']['姓名','年龄'][:]
 ```
 
 特殊操作：
 
 | 代码             | 解释                                               |
 | ---------------- | -------------------------------------------------- |
 | mup.inc(1)       | 自增1                                              |
```

