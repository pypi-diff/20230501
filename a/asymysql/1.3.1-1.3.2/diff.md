# Comparing `tmp/asymysql-1.3.1.tar.gz` & `tmp/asymysql-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asymysql-1.3.1.tar", last modified: Sat Apr 22 15:49:31 2023, max compression
+gzip compressed data, was "asymysql-1.3.2.tar", last modified: Mon May  1 01:58:53 2023, max compression
```

## Comparing `asymysql-1.3.1.tar` & `asymysql-1.3.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    10953 2023-02-13 16:22:52.569575 asymysql-1.3.1/LICENSE
--rw-r--r--   0        0        0     4815 2023-04-16 20:01:06.324279 asymysql-1.3.1/README.md
--rw-r--r--   0        0        0       28 2023-04-10 03:48:57.281686 asymysql-1.3.1/asymysql.py
--rw-r--r--   0        0        0      566 2023-04-22 15:49:10.106710 asymysql-1.3.1/pyproject.toml
--rw-r--r--   0        0        0     5052 1970-01-01 00:00:00.000000 asymysql-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0    10953 2023-02-13 16:22:52.569575 asymysql-1.3.2/LICENSE
+-rw-r--r--   0        0        0     4824 2023-05-01 01:52:20.933849 asymysql-1.3.2/README.md
+-rw-r--r--   0        0        0       28 2023-04-10 03:48:57.281686 asymysql-1.3.2/asymysql.py
+-rw-r--r--   0        0        0      582 2023-05-01 01:58:30.169274 asymysql-1.3.2/pyproject.toml
+-rw-r--r--   0        0        0     5077 1970-01-01 00:00:00.000000 asymysql-1.3.2/PKG-INFO
```

### Comparing `asymysql-1.3.1/LICENSE` & `asymysql-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `asymysql-1.3.1/README.md` & `asymysql-1.3.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 异步的 mysql ORM 。
 
 # 安装与教程
 
 安装：`pip install asymysql`
 
-[教程](https://github.com/lcctoor/lccpy/blob/main/asymysql/docs/doc.md)
+[教程](https://github.com/lcctoor/lccpy/blob/main/packages/asymysql/docs/doc.md)
 
 # Bug提交、功能提议
 
 您可以通过 [Github-Issues](https://github.com/lcctoor/lccpy/issues)、[微信](https://raw.githubusercontent.com/lcctoor/me/main/author/WeChatQR.jpg)、[技术交流群](https://raw.githubusercontent.com/lcctoor/me/main/ExchangeGroup/PythonTecQR.jpg) 与我联系。
 
 # 关于作者
```

### Comparing `asymysql-1.3.1/pyproject.toml` & `asymysql-1.3.2/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "asymysql"
-version = "1.3.1"
+version = "1.3.2"
 description = "异步的 mysql ORM"
-dependencies = ["lccpy >=1.4.5"]
+dependencies = ["lccpy >=1.4.6"]
 keywords = ["asymysql", "aiomysql", "mysql", "pymysql"]
 
 readme = "README.md"
 authors = [{name = "许灿标", email = "lcctoor@outlook.com"}]
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: Apache Software License"]
 requires-python = ">=3.7"
 
 [project.urls]
-HomePage = "https://github.com/lcctoor/lccpy/tree/main/asymysql"
+HomePage = "https://github.com/lcctoor/lccpy/tree/main/packages/asymysql#readme"
```

### Comparing `asymysql-1.3.1/PKG-INFO` & `asymysql-1.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: asymysql
-Version: 1.3.1
+Version: 1.3.2
 Summary: 异步的 mysql ORM
 Keywords: asymysql,aiomysql,mysql,pymysql
 Author-email: 许灿标 <lcctoor@outlook.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Dist: lccpy >=1.4.5
-Project-URL: HomePage, https://github.com/lcctoor/lccpy/tree/main/asymysql
+Requires-Dist: lccpy >=1.4.6
+Project-URL: HomePage, https://github.com/lcctoor/lccpy/tree/main/packages/asymysql#readme
 
 # 项目描述
 
 异步的 mysql ORM 。
 
 # 安装与教程
 
 安装：`pip install asymysql`
 
-[教程](https://github.com/lcctoor/lccpy/blob/main/asymysql/docs/doc.md)
+[教程](https://github.com/lcctoor/lccpy/blob/main/packages/asymysql/docs/doc.md)
 
 # Bug提交、功能提议
 
 您可以通过 [Github-Issues](https://github.com/lcctoor/lccpy/issues)、[微信](https://raw.githubusercontent.com/lcctoor/me/main/author/WeChatQR.jpg)、[技术交流群](https://raw.githubusercontent.com/lcctoor/me/main/ExchangeGroup/PythonTecQR.jpg) 与我联系。
 
 # 关于作者
```

